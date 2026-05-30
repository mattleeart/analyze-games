# CLAUDE.md

이 파일은 Claude Code가 본 저장소에서 작업할 때 따라야 할 프로젝트별 지침을 담고 있습니다.

## 프로젝트 개요

본 저장소는 **성공한 게임의 심층 분석서를 대량 생성하는 프로젝트**다. 2016년 이후 PC/콘솔 성공작을 게임 1개당 .md 1개로, 영어권 자료 기반 한국어 장문(기자 리뷰 수준, 8000자 이상) 분석한다. **단건 작성**과, **클라우드 routine이 큐를 소비하며 무한 자동 생성하는 대량 모드**를 모두 운영한다.

- 빌드·테스트·린트 도구가 없는 **콘텐츠(마크다운) 저장소**다. "완성" 판정은 빌드 통과가 아니라 **결과물 .md 파일의 크기**(`settings.min_size_bytes`, 기본 16000바이트 이상)로 한다.
- 분석 방법론·품질 기준의 단일 출처: 스킬 **`game-analysis-writer`**(`.claude/skills/`). 게임 분석 요청 시 자동 트리거된다.
- 대량 자동화: **`queue-worker`**(큐 소비·분석·갱신)와 **`queue-collector`**(큐 보충·발굴) 두 스킬이 담당한다.
- 현재 규모: `game_analyses/`에 분석서 약 335편 완성, 큐(`_progress.json`)는 총 345개 등록(iteration 7 기준). 수치는 회차마다 증가하므로 정확한 현황은 항상 실제 파일·큐를 스캔해 확인한다.

## 언어 규칙 (필수)

**모든 대화 세션에서 항상 한국어로 응답할 것.**

- 사용자에게 보내는 모든 설명·진행 보고·질문·요약은 한국어로 작성한다.
- 코드·식별자·명령어·파일 경로·라이브러리/프레임워크 이름 등 기술 용어는 원문(영문) 그대로 유지한다.
- 한국어 맞춤법과 띄어쓰기를 정확히 지킨다.
- 시스템 메시지나 도구 결과가 영어로 와도 사용자 응답은 한국어로 한다(영어 요청이 명시되지 않는 한).

## 마크다운 작성 규칙 (필수)

마크다운 렌더러는 `<단어>`를 HTML 태그로 해석해 렌더링 시 사라지거나 깨뜨린다(과거 분석서가 대량으로 망가진 적이 있다).

- **작품명·게임명·매체명은 꺾쇠 `<>`가 아니라 겹화살괄호 《 》로 표기**한다. 예: `《Elden Ring》`
- 부등호(`18kg 미만`)는 자연어로 쓰거나 `&lt;`로 이스케이프한다.
- 표·강조·링크는 표준 마크다운 문법을 쓰고, 백틱은 코드/명령어에만 쓴다.

## 디렉토리 구조

- **`game_analyses/`** — 분석 산출물과 큐
  - `NN_슬러그_연도.md` — 게임별 분석서 (예: `38_hades_2020.md`). 파일명의 `NN`은 큐의 `id`, `슬러그`는 `slug`, `연도`는 출시 `year`와 일치한다.
  - `_progress.json` — **마스터 큐**(UTF-8 BOM). `{schema_version, settings{batch_size, min_size_bytes, augment_count}, total_games, games[{id, title, year, slug, filename, status, completed_at?}], iteration, notes}`. status는 실제 .md 파일 기준으로 재생성되므로 신뢰 가능.
  - `_instructions.md` — subagent가 읽는 분석 지침(8개 섹션, 단일 출처).
    ⚠️ 이 파일 안의 저장 경로는 구 로컬 절대경로(`E:/...`)로 남아 있으나 **무시**한다. 클라우드/현행 규칙은 repo 루트 기준 상대경로(`game_analyses/`)다.
- **`.claude/skills/`** — 프로젝트 스킬
  - `game-analysis-writer/` — 분석 방법론·품질 기준(단건 작성의 단일 출처). `SKILL.md`, `references/analysis-template.md`(8개 섹션 목차), `references/automation-setup.md`(대량 모드), `assets/progress_template.json`(큐 초기 템플릿), `evals/`(품질 평가 기준).
  - `queue-worker/SKILL.md` — 큐 소비: pending을 subagent로 병렬 분석 → 검증 → 큐 갱신 → main push
  - `queue-collector/SKILL.md` — 큐 보충: 신규 후보 발굴 → 큐 등록

> 로컬 전용 자산(`_worker.ps1`, `monitor/`, `_logs/`, `_wip/`, `_STATUS.md`, 스킬의 `scripts/`, `.obsidian/`)은 `.gitignore`로 제외된다 — 구 로컬 Task Scheduler 방식의 잔재이며 클라우드 운영에는 쓰지 않는다(로컬 복구용으로만 디스크에 보관).

## 대량 자동화 운영 (클라우드 routine)

대량 모드는 **Claude Code 클라우드 routine**(claude.ai/code, `/schedule` cron)이 이 repo를 받아 게임 분석을 무한 생성하는 구조다. **로컬 PC 전원·세션과 무관하게** 클라우드에서 돈다.

**한 회차(routine cron 1회) 흐름**:
1. routine이 main을 fresh clone → `queue-worker` 스킬 실행
2. `_progress.json` + 실제 `.md` 스캔으로 status 재생성(`settings.min_size_bytes` 이상 = completed)
3. `settings.batch_size`개 pending을 `id` 오름차순으로 골라 general-purpose subagent로 **병렬 분석**(각자 .md만 저장)
4. 완성 검증(실제 파일 크기) → 큐 갱신 → `git add game_analyses/ && git commit && git push origin main`
5. pending이 0이면 `queue-collector`로 신규 후보 발굴(`augment_count`개)

**제어**: routine 관리는 `/schedule list`·`/schedule update` 또는 claude.ai/code 웹 UI. 회차당 처리량·완성 임계·발굴 개수는 `_progress.json`의 `settings`에서 조절한다(cron 프롬프트 수정 불필요).

**반드시 지킬 운영 규칙** (실전에서 두 번 크게 망가졌다 고친 것):
1. **subagent는 `_progress.json`을 절대 읽거나 쓰지 않는다.** 분석서 .md만 저장한다. 동시 수정은 race condition으로 큐를 "전부 완료"로 오염시켜 멈추게 한다. 상태 관리는 queue-worker(메인 에이전트)가 실제 파일 존재·크기로만 단독 판정한다. queue-collector도 큐를 단독으로만 수정한다.
2. **동시 실행은 `batch_size`(기본 4)로 제한하고 WebFetch를 절제한다.** 한 번에 너무 많이 띄우거나 WebFetch를 남발하면 사용량 한도를 순식간에 태워 대부분 미완성으로 중단된다. WebSearch를 주력(8~12회)으로, WebFetch는 핵심 출처만(3~5회) 쓴다.
3. **완성 판정은 결과물(.md 크기 ≥ `min_size_bytes`, 기본 16KB)로 한다.** 큐의 기존 status는 신뢰하지 않는다 — subagent 보고 텍스트가 아니라 실제 파일 크기로 재판정하므로 어떤 오염도 다음 회차에 자가 교정된다.

**경로 규칙**: 클라우드 작업 디렉토리는 repo 루트이므로 모든 경로는 **repo 루트 기준 상대경로**(`game_analyses/...`)를 쓴다. 절대경로(`E:\...`)는 클라우드에서 깨지므로 금지.

## 자주 쓰는 명령

빌드/테스트 시스템은 없다. 운영에 실제로 쓰는 명령은 다음과 같다.

```bash
# 완성본 개수 확인 (16KB 이상 = completed 판정 기준)
find game_analyses -maxdepth 1 -name '*.md' -size +16k | wc -l

# 큐 현황(완성/대기) 집계 — BOM 때문에 utf-8-sig로 읽는다
python3 -c "import json;d=json.load(open('game_analyses/_progress.json',encoding='utf-8-sig'));from collections import Counter;print(Counter(g['status'] for g in d['games']))"

# 분석서 미달(부분 완성/깨짐) 후보 찾기
find game_analyses -maxdepth 1 -name '*.md' -size -16k

# 결과 커밋·푸시 (대량 모드는 main, 그 외 작업은 지정 브랜치로)
git add game_analyses/ && git commit -m "analyze: <완성한 게임들>" && git push origin <branch>
```
