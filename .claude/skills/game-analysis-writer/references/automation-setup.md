# 대량 자동화 셋업 (멈추지 않는 무한 생성)

게임 수십~수백 개를 사람 개입 없이, quota 만료를 견디며 자동 생성하는 시스템이다. Windows + Claude Code CLI 기준.

## 전체 그림

```
OS 스케줄러(15분 주기)
   └─ worker.ps1 실행
        ├─ 실제 .md 파일 스캔 → _progress.json 상태 재생성 (단일 진실)
        ├─ pending 6개 선택 → claude -p 로 sub-agent 병렬 dispatch
        │     └─ 각 sub-agent: 리서치 → 분석서 .md 저장 (progress.json은 안 건드림)
        └─ pending 0이면 → 새 후보 자동 발굴(augment) → 다음 사이클에 분석
```

이 구조가 멈추지 않는 이유: quota(5시간 한도)가 소진되면 워커의 `claude -p` 호출이 즉시 실패하고 워커는 그냥 종료한다. 다음 15분 사이클에서 다시 시도하고, quota가 리셋되면 자동으로 이어진다. OS 스케줄러는 Claude 세션과 독립이라 세션이 닫혀도 계속 돈다.

## 셋업 절차

### 1. 작업 디렉토리와 상태 파일
작업 폴더(예: `프로젝트/game_analyses/`)에 다음을 둔다:
- `_progress.json` — `assets/progress_template.json`을 복사해 분석할 게임 목록으로 채운다. 각 항목: `{id, title, year, slug, filename, status:"pending"}`.
- `_instructions.md` — `references/analysis-template.md` 내용을 복사해 둔다(sub-agent가 읽는다).
- `_logs/` — 워커 로그 디렉토리.

### 2. 워커 배치
`scripts/worker.ps1`을 작업 폴더에 복사하고, 상단 변수(`$workDir`, `$gameDir`, `$claudeExe`)를 환경에 맞게 수정한다. `claude.exe` 경로는 `(Get-Command claude).Source`로 확인한다.

### 3. 스케줄러 등록
`scripts/setup_scheduler.ps1`을 실행해 Task Scheduler에 15분 주기로 등록한다. 즉시 1회 실행도 트리거된다.

```powershell
powershell -ExecutionPolicy Bypass -File scripts\setup_scheduler.ps1 -Action register
```

## 워커 동작 (worker.ps1)

매 실행마다:
1. **lock 확인** — 다른 워커가 도는 중이면(lock 25분 이내) 종료. 중복 실행 방지.
2. **상태 재생성** — 모든 게임에 대해 실제 `.md` 파일이 존재하고 16KB 이상이면 `completed`, 아니면 `pending`. progress.json의 기존 status는 신뢰하지 않는다(오염 자가 교정).
3. **배치 dispatch** — pending을 id 순 6개 선택, `claude -p`에 "각 게임을 sub-agent로 병렬 분석하라"는 프롬프트를 stdin으로 전달.
4. **무한 발굴** — pending이 0이면 `claude -p`로 "기존 목록에 없는 성공 게임 10개를 발굴해 progress.json에 추가"시킨다. 다음 사이클이 그것들을 분석한다.

## sub-agent 프롬프트 (워커가 생성)

각 sub-agent에게는 다음을 지시한다:
- `_instructions.md`를 먼저 읽고 그대로 따를 것
- 담당 게임의 제목/연도/저장경로
- WebSearch 위주 8~12회 + WebFetch 3~5회, 영어권 자료
- 한국어 8000자 이상, 8개 섹션
- **`_progress.json`을 절대 읽거나 쓰지 말 것** (분석서 .md만 저장) — race condition 방지의 핵심
- 작품명은 《》 표기

## 제어 명령

```powershell
# 일시중지
Disable-ScheduledTask -TaskName "GameAnalysisWorker"

# 재개
Enable-ScheduledTask -TaskName "GameAnalysisWorker"
Start-ScheduledTask  -TaskName "GameAnalysisWorker"

# 완전 종료
Unregister-ScheduledTask -TaskName "GameAnalysisWorker" -Confirm:$false

# 진행 상태
(Get-Content .\_progress.json -Raw | ConvertFrom-Json).games | Group-Object status
```

## 실시간 모니터

워커가 백그라운드에서 무엇을 하는지 브라우저로 실시간 관찰할 수 있다. 프로젝트 루트의 `monitor/` 폴더에 Node.js 기반 대시보드가 있다(의존성 0, 내장 http만 사용).

- **열기**: `monitor/start-monitor.ps1` 실행. 멱등이라 서버가 이미 떠 있으면 브라우저만 연다. 바탕화면 바로가기(`게임 분석 모니터`)로도 연결돼 있다.
- **표시**: 워커 상태(Running/Disabled), 완성/작성중/대기/전체 카운트, 진행률, 지금 분석 중인 게임, 최근 완성, 전체 게임 타일 그리드, 워커 활동 로그. 5초마다 자동 갱신.
- **상태 판정**: 대시보드도 워커와 동일하게 실제 `.md` 파일(16KB+) 기준으로 재판정한다. progress.json의 stale 표시에 속지 않는다.
- **데이터 소스**: progress.json + `.md` 파일 + 워커 로그 + Task Scheduler 상태(PowerShell 자식 프로세스로 조회).

**대량 자동화를 시작하거나 제어(Enable/Start/Disable)할 때는 이 모니터를 함께 띄워** 사용자가 진행을 눈으로 볼 수 있게 한다 — `monitor/start-monitor.ps1` 한 줄 실행이면 된다(이미 떠 있으면 자동으로 브라우저만 연다).

## 트러블슈팅 (실전에서 겪은 것들)

- **워커가 "전부 완료"로 오판하고 멈춤** → sub-agent가 progress.json을 동시 수정해 오염된 경우. sub-agent 프롬프트에서 progress.json 접근을 금지하고, 워커는 실제 파일로만 판정하도록 한다(현재 worker.ps1은 그렇게 동작).
- **quota가 너무 빨리 소진됨** → 동시 실행 수가 많거나 WebFetch 남용. 배치 크기를 6으로 줄이고 WebFetch를 절제한다.
- **부분 파일(작은 .md)이 completed로 잡힘** → 크기 임계값(16KB)으로 거른다. 미달이면 pending으로 되돌려 재생성.
- **로그·프롬프트 한글 깨짐** → 근본 원인은 워커 스크립트(`worker.ps1`)가 BOM 없는 UTF-8로 저장된 것. Windows PowerShell 5.1은 BOM 없는 `.ps1`을 시스템 ANSI(한국어 환경은 CP949)로 읽기 때문에, 스크립트 안의 한글 리터럴이 **파싱 단계에서 이미 깨지고** 그게 로그와 sub-agent 프롬프트로 전파된다(가독성만이 아니라 프롬프트 품질에도 영향). **해결: `worker.ps1`을 UTF-8 with BOM으로 저장**한다(로직 변경 없이 인코딩만). 확인: 첫 3바이트가 `EF BB BF`인지. 이미 깨진 기존 로그는 원본 한글 정보가 손실되어 완전 복구가 불가능하다.
- **새 세션 인계** → 작업 폴더에 `_STATUS.md`를 두어 현재 완성 수·대기 목록·재개 명령을 적어두면, 새 세션의 Claude가 읽고 바로 이어갈 수 있다.
