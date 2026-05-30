---
name: queue-collector
description: >-
  게임 분석 큐(game_analyses/_progress.json)에 분석할 신규 후보 게임을 발굴해 추가한다.
  queue-worker가 큐를 모두 비웠을 때 자동 호출하거나, 사용자가 "후보 게임 발굴", "큐 채워줘",
  "분석 목록에 게임 추가", "queue-collector 실행"이라고 요청할 때 사용한다. WebSearch로 2016년
  이후 성공한 PC/콘솔 게임을 기존 목록과 중복 없이 찾아 pending으로 등록하고 main에 push한다.
  분석서(.md)는 만들지 않는다 — 분석은 다음 queue-worker 회차가 담당한다.
---

# queue-collector — 게임 분석 큐 보충기

큐가 비었거나 사용자가 후보를 더 원할 때, 분석 대상 게임을 발굴해 큐에 추가하는 스킬이다. **발굴과 큐 등록만** 하고 분석서는 만들지 않는다.

## 실행 환경 전제

- 작업 디렉토리는 **git repo 루트**다. 경로는 repo 상대경로(`game_analyses/_progress.json`)로 쓴다(절대경로 금지).
- 이 스킬도 큐를 **단독으로** 수정한다(동시에 다른 주체가 큐를 건드리지 않는 전제). 분석 subagent는 큐를 절대 건드리지 않는다.

## 절차

### 1. 현재 큐 파악

`game_analyses/_progress.json`을 읽는다. 다음을 확보한다:
- 기존 `games[].title` 전체 목록 (중복 방지용)
- `id`의 최댓값 (`maxId`)
- `settings.augment_count` (발굴 개수, 기본 10), `iteration`, `total_games`

### 2. 신규 후보 발굴

WebSearch로 **2016년 이후 출시된 PC/콘솔 성공 게임** 중 위 기존 목록에 **없는** 것을 `augment_count`개 찾는다.

- 기준: Metacritic 80점 이상 **또는** 명백한 상업적·문화적 성공.
- **모바일 전용 게임 제외**(이 프로젝트는 PC/콘솔 전용).
- 장르·국가·규모(AAA/인디)를 다양하게 골고루.
- **기존 목록과 절대 중복 금지** — 제목이 조금만 비슷해도 같은 작품인지 검증한다.

### 3. 큐에 등록

발굴한 게임들을 `games` 배열 **끝에 append**한다. 기존 항목은 절대 손상·삭제하지 않는다. 각 신규 항목:

```json
{ "id": maxId 다음 번호부터 1씩 증가,
  "title": "정식 제목",
  "year": 출시연도(정수),
  "slug": "영문 소문자 슬러그(공백·기호는 _)",
  "filename": "<id>_<slug>_<year>.md",
  "status": "pending" }
```

그리고 최상위 `total_games`를 새 개수로, `iteration`을 1 증가시켜 저장한다.

### 4. 커밋 · 푸시

```
git add game_analyses/_progress.json
git commit -m "augment: 신규 후보 N개 추가 (iteration K)"
git pull --rebase origin main
git push origin main
```

## 규칙

- **기존 목록과 중복 절대 금지.**
- **`_progress.json`만 수정한다.** 분석서(.md)는 만들지 마라 — 다음 queue-worker 회차가 자동 분석한다.
- 사용자에게 질문하지 마라. 발굴 + 큐 등록 + push만 하고 끝낸다.
- 작품명을 사람에게 보고할 때도 겹화살괄호 《 》로 표기한다.
