---
name: queue-worker
description: >-
  게임 분석 큐(game_analyses/_progress.json)의 대기(pending) 게임을 subagent로 병렬 분석하고,
  완성된 .md를 검증해 큐 상태를 갱신한 뒤 결과를 git main에 커밋·푸시한다. 클라우드 routine이
  주기적으로 실행하거나, 사용자가 "큐 처리해줘", "대기 게임 분석해", "queue-worker 실행"이라고
  요청할 때 사용한다. 한 회차에 settings.batch_size개를 처리하고, 큐가 비면 queue-collector로
  신규 후보를 발굴한다. 분석 본문은 반드시 subagent에 위임해 메인 에이전트의 컨텍스트를 보호한다.
---

# queue-worker — 게임 분석 큐 소비 워커

클라우드 routine(또는 수동 트리거)이 한 회차(iteration)에 호출하는 메인 스킬이다. 큐에서 대기 게임을 꺼내 분석 subagent에 위임하고, 결과를 검증·기록·푸시한다. **이 스킬을 수행하는 너(메인 에이전트)는 큐 관리·오케스트레이션만 하고, 무거운 리서치·작성은 전부 subagent에 맡긴다**(메인 컨텍스트 보호).

## 실행 환경 전제

- 작업 디렉토리는 **git repo 루트**다(클라우드 routine은 매 run마다 main을 fresh clone한다). 모든 경로는 **repo 루트 기준 상대경로**(`game_analyses/...`)로 쓴다. 절대경로(`E:\...`)는 클라우드에서 깨지므로 금지.
- 큐: `game_analyses/_progress.json` · 분석 지침: `game_analyses/_instructions.md`.

## 절차

### 1. 상태 동기화 (큐를 실제 파일로 재생성)

`game_analyses/_progress.json`을 읽고 `game_analyses/`의 분석서 `.md`들을 스캔한다. 각 game 항목에 대해:

- 실제 `game_analyses/<filename>`이 존재하고 크기가 `settings.min_size_bytes`(기본 16000) 이상이면 → `status: "completed"`(+`completed_at` 타임스탬프)
- 아니면 → `status: "pending"`(`completed_at` 제거)

**큐의 기존 status는 신뢰하지 않는다**(교훈 ③). 매번 실제 파일로 재판정하므로 어떤 오염도 자가 교정된다. 재생성한 큐를 `_progress.json`에 다시 저장한다.

### 2. 배치 선정

`status == "pending"`인 게임을 `id` 오름차순으로 `settings.batch_size`(기본 4)개 고른다.

### 3a. pending이 있으면 — 분석 위임

고른 게임들을 **각각 별도의 subagent로 병렬 launch**한다. 단일 메시지에 모든 Agent 호출을 배치하고 `subagent_type: "general-purpose"`, `run_in_background: true`로 띄운다. 동시 실행은 `batch_size`개를 넘기지 않는다(교훈 ②: 사용량 폭주 방지).

각 subagent에 보낼 프롬프트(게임마다 `<TITLE>`·`<YEAR>`·`<FILENAME>` 치환):

```
당신은 게임 분석 전문 리서처다. 먼저 game_analyses/_instructions.md 를 Read로 읽고 그 지침을 완전히 따르라.

담당 게임: 《<TITLE>》 (<YEAR>)
저장 경로(repo 상대경로): game_analyses/<FILENAME>

작업:
1. WebSearch를 주력으로 8~12회 영어권 자료를 리서치하라. WebFetch는 꼭 필요한 핵심 출처만 3~5회로 절제한다(토큰 절약). 별도 리서치 노트 파일은 만들지 말고, 리서치 직후 곧바로 본문을 작성하라.
2. _instructions.md의 8개 섹션을 한국어 8000자 이상(목표 1.5만~2.5만자)으로 작성해 game_analyses/<FILENAME> 에 Write로 저장하라.

절대 규칙:
- _progress.json은 읽지도 쓰지도 마라. 완성 분석서 .md 단 한 개만 저장하고, 그 외 어떤 파일도 건드리지 마라.
- 경로는 위 repo 상대경로를 그대로 사용하라(절대경로 금지).
- 작품명·게임명·매체명은 겹화살괄호 《 》로 표기하라(꺾쇠 <> 금지 — 렌더링 시 깨진다).
- 사용자에게 질문하지 마라. 망설여지면 더 디테일하고 정보량 많은 쪽을 택하라.
- 완료 후 "저장완료 N자" 한 줄만 보고하라.
```

모든 subagent가 끝날 때까지 기다린다.

### 3b. pending이 0이면 — 큐 보충

`queue-collector` 스킬을 실행해 신규 후보를 발굴한다(기존 목록과 중복 금지). 발굴 후 이번 회차는 종료한다 — 다음 회차가 새 pending을 분석한다.

### 4. 완성 검증 + 큐 갱신

subagent들이 끝나면 `game_analyses/`를 다시 스캔한다. 이번 배치 게임 중 실제 `.md`가 `min_size_bytes` 이상인 것만 `status: "completed"`(+`completed_at`)로 갱신한다. 미달(부분 완성/실패)은 `pending`을 유지해 다음 회차가 재시도한다. **subagent의 보고 텍스트가 아니라 실제 파일 크기로 판정**한다(교훈 ③).

### 5. 커밋 · 푸시

변경분을 main에 반영해 다음 회차가 이어받게 한다:

```
git add game_analyses/
git commit -m "analyze: <이번에 완성한 게임들>"
git pull --rebase origin main   # 혹시 모를 동시 변경 대비
git push origin main
```

push가 실패하면 로그로 남기고 종료한다(다음 회차가 재시도). 완성된 게 하나도 없으면 커밋을 건너뛴다. git 사용자 설정이 없다는 오류가 나면 `git config user.email`·`user.name`을 임시값으로 설정한 뒤 재시도한다.

## 반드시 지킬 운영 교훈 (실전에서 두 번 망가지고 고친 것)

1. **subagent는 `_progress.json`을 절대 읽거나 쓰지 않는다.** 분석서 `.md`만 저장한다. 큐 상태 관리는 이 스킬을 수행하는 메인 에이전트가 **단독으로**, 실제 파일 기준으로만 한다(동시 수정 race가 큐를 "전부 완료"로 오염시켜 멈춘 적 있음).
2. **동시 실행은 `batch_size`(기본 4)로 제한하고 WebFetch를 절제한다.** 한 번에 너무 많이 띄우거나 WebFetch를 남발하면 사용량 한도를 순식간에 태워 대부분 미완성으로 끝난다. WebSearch를 주력으로 쓴다.
3. **완성 판정은 결과물(.md 크기 ≥ `min_size_bytes`)로 한다.** 큐의 기존 status를 믿지 말고 매번 실제 파일로 재판정한다.

## 마크다운 표기 규칙

- 작품명·게임명·매체명은 꺾쇠 `<>`가 아니라 겹화살괄호 《 》로 표기한다(렌더러가 `<단어>`를 HTML 태그로 먹어 깨뜨린다).
- 부등호는 "18kg 미만" 같은 자연어로 쓰거나 `&lt;`로 이스케이프한다.

## 조정 가능한 파라미터

회차당 처리량 등은 cron 프롬프트가 아니라 `_progress.json`의 `settings`에서 바꾼다:

- `batch_size` — 회차당 병렬 분석 개수(기본 4)
- `min_size_bytes` — 완성 판정 최소 바이트(기본 16000)
- `augment_count` — 큐가 빌 때 발굴할 신규 후보 개수(기본 10)
