# Cursed to Golf (2022) 심층 분석

> "골프의 다크 소울(the Dark Souls of golf)." — 여러 매체가 《Cursed to Golf》를 묘사할 때 즐겨 쓴 표현. 이 한 줄에 게임의 정체성이 응축돼 있다. 골프라는 가장 정적이고 점잖은 스포츠를, 죽음과 부활을 건 가혹한 로그라이크로 비틀어 놓은 작품.

---

## 1. 게임 개요

《Cursed to Golf》는 2022년 8월 18일 출시된 2D 로그라이크 골프 게임이다. 교토(Kyoto)에 거점을 둔 인디 스튜디오 **Chuhai Labs**가 개발했고, 스웨덴계 인디 퍼블리셔 **Thunderful Publishing**이 배급했다. 장르를 한마디로 규정하기 어려운데, 개발진 스스로는 "골프 게임이 아니라 **골프라이크(Golf-Like)**"라고 부른다. 표면은 스포츠지만 실제 구조는 로그라이크 던전 크롤러에 가깝고, 거기에 퍼즐 플랫포머와 라이트 덱빌딩(deckbuilding)이 얹혀 있다.

- **개발사**: Chuhai Labs (교토 소재 소규모 인디 스튜디오)
- **퍼블리셔**: Thunderful Publishing
- **출시일**: 2022년 8월 18일 (전 플랫폼 동시 출시)
- **플랫폼**: PC(Windows / Steam·GOG·Epic Games Store), PlayStation 4, PlayStation 5, Xbox One, Xbox Series X|S, Nintendo Switch
- **장르**: 로그라이크 / 스포츠 / 퍼즐 플랫포머
- **플레이 모드**: 싱글플레이 전용

### 주요 크레딧

- **디렉터·디자이너**: Liam Edwards — 원작 프로토타입 제작자이자 게임 디렉터. Rockstar Games 출신으로 《Grand Theft Auto V》, 《Red Dead Redemption II》 개발에 참여한 이력이 있다. Rockstar를 떠나 일본으로 이주, 영어 교사를 하며 게임 팟캐스트(Final Games)를 운영하던 중 본작의 씨앗을 틔웠다.
- **리드 프로그래머**: Sean Fisher
- **아트 디렉터**: Jon Davies
- **아티스트**: Nathan Scott, **Shiino Hiroco(시노 히로코)** — 《Yo-kai Watch(요괴워치)》 시리즈 작업으로 알려진 베테랑 픽셀 아티스트
- **작곡**: **Mark Sparling** — 인디 명작 《A Short Hike》의 음악으로 유명한 작곡가

### 개발 규모·엔진

본작의 핵심은 **극단적으로 작은 팀**이라는 점이다. 디렉터 1인이 시작한 프로젝트가 퍼블리싱 계약 후 소수의 산업 베테랑이 합류하며 완성됐다. Liam Edwards는 최초 프로토타입을 **GameMaker**로 itch.io에 올렸고(2020년), 정식판은 이를 확장·재제작한 것이다. (정식판 엔진에 대해서는 일부 자료가 Unity를, 일부가 GameMaker 계열을 언급해 표기가 엇갈린다 — 프로토타입이 GameMaker로 만들어졌다는 사실은 디렉터 본인이 여러 인터뷰에서 확인했다.)

개발 타임라인은 다음과 같다.

- **2020년**: Liam Edwards가 GameMaker로 1차 프로토타입 제작, itch.io에 무료 공개. "던전 안에서 공을 튕긴다"는 물리 실험에서 출발했다.
- 트위터·디스코드를 통해 프로토타입이 입소문을 타며 플레이어가 늘고, 퍼블리셔의 관심을 끌었다.
- **2021년 8월 30일**: 정식 발표. Thunderful Publishing 배급 확정.
- **2022년 3월**: Steam 한정 기간 데모 공개(PAX East 2022 등 행사 출품).
- **2022년 7월 7일**: 최종 출시일 확정 발표.
- **2022년 8월 18일**: 전 플랫폼 정식 출시.

---

## 2. 게임 설명 — 이 게임이 대체 무엇인가

### 컨셉과 세계관

《Cursed to Golf》는 **사후 세계 골프**라는 작정하고 비튼 발상으로 출발한다. 플레이어는 토너먼트 우승을 코앞에 둔 프로 골퍼다. 마지막 퍼팅을 앞둔 순간, 하늘에서 벼락이 내리쳐 즉사한다. 정신을 차려보니 도착한 곳은 **골프 연옥(Golf Purgatory)** — 죽은 골퍼들이 이승으로 돌아가기 위해 영원히 공을 치는 지하 세계다.

이곳에서 플레이어를 맞이하는 것은 거대한 유령 **The Scotsman(스코츠맨)**. 그는 플레이어에게 '꼬마(Wee One)'라는 별명을 붙이며 하나의 전설을 들려준다. 골프 연옥의 **18홀 코스를 완주하면 이승으로 부활할 수 있다**는 것. 단, 아직 아무도 그것을 해낸 자는 없다. 플레이어는 자신의 육체로 돌아가 미완의 토너먼트를 끝내기 위해, 연옥의 18홀에 도전한다.

이 설정의 영리함은 로그라이크의 핵심 메커니즘 — "죽으면 처음부터" — 를 서사적으로 완벽하게 정당화한다는 데 있다. 이미 죽은 자가 부활을 위해 도전하는 세계이니, 실패하면 다시 출발점으로 돌아가는 것이 어색하지 않다. 골프와 로그라이크라는, 도무지 어울릴 것 같지 않은 두 장르를 "연옥"이라는 단어 하나가 봉합한다.

### 줄거리와 등장인물 [스포일러 포함]

이야기는 바이옴(biome) 단위로 진행된다. 각 바이옴 끝에는 그곳을 지배하는 **전설의 캐디(Legendary Caddie)**가 보스로 기다린다.

- **연옥(Purgatory)** — The Scotsman: 플레이어의 안내자이자 첫 관문. 거대한 유령 골퍼.
- **사막(Desert)** — **The Explorer(탐험가)**
- **동굴(Caves)** — **The Forgotten(잊혀진 자)**

코스를 거듭 오를수록 환경이 험해지고, 종반에 이르면 말 그대로 **지옥(HELL)**에 도달한다. 자료에 따르면 16번째 홀 이후의 구간이 지옥에 해당하며, 그 이름값을 하듯 플레이어가 가진 모든 골프 실력과 Ace Card 능력, 그동안 축적한 보너스를 총동원해야 통과할 수 있는 마지막 시련으로 구성된다. 이 최후의 보루를 넘어서야 비로소 '승천(ascension)' — 즉 이승으로의 부활이 가능하다.

[스포일러] 본작의 서사는 깊은 분기형 스토리텔링보다는 캐릭터 보이스와 분위기로 승부한다. 평론가들은 "자칫 음울하기만 할 수 있었던 설정을, 매력적이고 위트 있는 글쓰기가 살려냈다"고 입을 모았다. The Scotsman의 능청스러운 입담을 비롯한 NPC들의 대사가 죽음과 연옥이라는 무거운 소재를 경쾌하게 풀어낸다.

### 무드·톤·아트 디렉션

비주얼은 **레트로 픽셀 아트**다. 그러나 단순한 향수 자극을 넘어선다. 사막·동굴·지옥으로 이어지는 바이옴 각각이 뚜렷한 색채와 위험 요소를 지니고, 16비트 시대의 골프 게임(특히 《Mario Golf》)을 향한 헌사가 화면 곳곳에 배어 있다. 요괴워치 출신 아티스트 Shiino Hiroco가 참여한 만큼, 캐릭터와 유령들의 표정·실루엣 처리가 인상적이라는 평이 많았다.

### 사운드와 음악

음악은 본작이 가장 큰 찬사를 받은 영역 중 하나다. 《A Short Hike》로 이름을 알린 **Mark Sparling**이 39개 트랙에 달하는 사운드트랙을 작곡했다. 그가 밝힌 최초 음악 컨셉은 **"Castlevania와 Mario Golf의 만남(Castlevania meets Mario Golf)"**. 실제 앨범은 《Mario Golf》, 한국 골프 온라인 게임 《PangYa(팡야)》, 《Castlevania》, 그리고 수많은 레트로 게임 사운드트랙을 향한 러브레터로 묘사된다.

에너지 넘치는 칩튠(chiptune)이 연옥에서 골프 레전드로 승천하는 여정 내내 플레이어를 몰아붙인다. 평단은 이 사운드트랙을 거의 만장일치로 호평했으나, 일부는 같은 코스를 반복하다 보면 음악이 다소 반복적으로 느껴질 수 있다는 점을 지적했다. 사운드트랙은 디지털·스트리밍은 물론, Black Screen Records 등을 통해 **2xLP 바이닐(vinyl)**로도 발매돼 인디 게임 음악 컬렉터들의 수집 대상이 됐다.

---

## 3. 핵심 시스템 / 메카닉 — 가장 자세하게

본작의 진짜 매력은 표면의 골프 룩 아래 숨은 정교한 시스템 설계에 있다. 하나씩 분해해 본다.

### 코어 루프: 5타 안의 생존

가장 근본적인 규칙은 **"매 홀을 5타(PAR Count) 안에 끝내라"**다. 5타 안에 공을 컵에 넣지 못하면 — **죽는다.** 단순히 그 홀에서 페널티를 받는 게 아니라, 18홀 도전 전체가 끝나고 맨 처음으로 돌아간다. 전통 골프의 '파(par)'를 생존 자원으로 재해석한 발상이다. 매 스트로크가 곧 생명이며, 플레이어는 항상 "이 한 타를 어디에 쓸 것인가"를 계산하게 된다.

### 사이드뷰 골프 + 플랫포머

본작은 위에서 내려다보는 탑다운 골프가 아니라 **2D 횡스크롤(side-scrolling)** 시점이다. 즉 골프장이 곧 플랫포머 스테이지처럼 펼쳐진다. 평지 위에서 공을 굴리는 게 아니라, 절벽·물웅덩이·TNT·이동 발판·바람 같은 메트로배니아풍 위험 요소들이 빼곡한 복잡한 입체 지형을 통과해 공을 컵까지 보내야 한다. 평론가들은 이 코스들을 "전통 골프장 레이아웃이 아니라 메트로배니아 같은 던전"이라고 묘사했다.

### 클럽과 조준 — 타이밍 게이지

클럽은 **드라이버(driver), 아이언(iron), 웨지(wedge)** 세 종류다. 샷은 타이밍 기반이다. 각도를 정한 뒤 파워 게이지를 멈추고, 다시 정확도(스위트 스팟) 타이밍을 맞춰 친다. 즉 골프 시뮬레이션의 클래식한 3-클릭/타이밍 샷 문법을 그대로 가져왔다. GameSpot의 Steven Petite는 "컨트롤의 단순함(simplicity of the game's controls)"을 호평 포인트로 짚었다.

### 공 스핀 / 공중 제어

본작의 시그니처 메커닉 중 하나는 **공이 날아가는 도중·착지 직후에 스핀을 줘 미세하게 궤도를 조정**할 수 있다는 점이다. 정밀한 백스핀·탑스핀 컨트롤이 가능해, 같은 샷이라도 착지 후 어떻게 굴릴지를 플레이어가 능동적으로 설계한다. 이 공중 제어 시스템은 단순 타이밍 게임을 전술적 퍼즐로 끌어올리는 핵심 장치로 자주 거론됐다.

### Ace Card — 라이트 덱빌딩

본작을 평범한 골프 게임과 가르는 결정적 요소가 **Ace Card(에이스 카드)**다. 일종의 1회용 마법 카드로, 한 라운드 동안 손에 들고 다니다 결정적 순간에 사용한다. 카드는 두 경로로 얻는다 — (1) The Scotsman이 직접 주거나, (2) 코스 곳곳의 **상자(chest)**에 공을 명중시켜 획득. 대표적인 효과들:

- **추가 타수**를 받는 카드(멀리건/Mulligan 계열)
- 공이 공중에 떠 있을 때 **정지**시키는 카드
- 타수를 쓰지 않고 **TNT 장애물을 폭파**시키는 별도의 공을 소환
- 공을 **얼음(ice)**으로 바꿔 물 위를 튕겨 건너기
- 공을 **조종 가능한 로켓(controllable rocket)**으로 변신
- **다수의 무료 샷**을 얻기
- 공을 **드릴(drill)**로 바꿔 발판을 뚫고 내려가기
- 궤도를 꺾는 **U턴(U-turn)** 계열

이 카드들은 5타 제한이라는 가혹한 룰에 숨통을 틔워주는 동시에, "언제 어떤 카드를 아껴 쓸 것인가"라는 자원 관리 레이어를 더한다. 라이트 덱빌딩이라 불리는 이유다.

### Idol(우상상) — 골드 / 실버

5타라는 자원을 늘릴 두 번째 수단이 코스에 배치된 **Idol(아이돌/우상상)**이다. 부수면 추가 타수를 준다.

- **골드 우상상(Gold Idol)**: 명중 시 **+4타**
- **실버 우상상(Silver Idol)**: 명중 시 **+2타**

문제는 이 우상상들이 종종 위험하거나 까다로운 위치에 배치돼 있다는 점이다. 추가 타수를 얻으러 가는 행위 자체가 타수와 리스크를 소모한다. "지금 우상상을 노릴 것인가, 아니면 안전하게 컵으로 직행할 것인가"라는 끊임없는 손익 계산이 발생한다.

### 진행 구조와 로그라이크 요소

코스는 **약 70개의 사전 제작된 홀(predesigned holes)** 풀에서 무작위로 뽑혀 배치된다. 즉 절차적 생성으로 지형 자체를 만드는 방식이 아니라, **수제 홀을 셔플(shuffle)**하는 구조다. 다만 매번 동일하진 않다 — 장애물과 우상상 위치, 상자 배치 등이 런마다 달라진다. 18홀을 클리어하는 한 번의 런(run)은 보통 두 시간 안팎이 걸린다.

영구 죽음(permadeath)이 핵심이지만, 본작에는 영속성(meta-progression)도 일부 존재한다. 각 바이옴 보스(전설의 캐디)를 격파하면 그 보상이 **이후에도 유지**되어, 반복 도전이 완전히 무의미해지지 않도록 설계됐다.

### Eterni-Tee — 상점

홀을 클리어하면 **코인(coin)**을 얻는다. 이 코인은 The Scotsman이 운영하는 상점 **Eterni-Tee(에터니-티)**에서 새로운 Ace Card를 구매하는 데 쓴다. (이름부터 'Eternity'와 'Tee'의 말장난이다 — 본작 특유의 골프 펀(pun) 작명 센스가 곳곳에 박혀 있다.) 상점에서는 PINS 섹션 등을 통해 카드 풀을 보강할 수 있어, 런이 진행될수록 플레이어의 전술적 선택지가 넓어진다.

### Birdie-Eye 카메라

복잡한 입체 코스를 공략하려면 전체 지형을 봐야 한다. 이를 위한 보조 기능이 **Birdie-Eye(버디-아이) 카메라**다. 스테이지 전체를 조망해 장애물 배치와 경로를 미리 계획할 수 있게 해준다. (역시 'Bird's-eye'와 골프의 'Birdie'를 엮은 말장난.)

### 난이도와 접근성

본작은 의도적으로 어렵다. "골프의 다크 소울"이라는 별칭은 농담이 아니라 실제 난이도 곡선에서 나온 것이다. 5타 제한, 영구 죽음, 두 시간짜리 런이 결합돼, 후반 홀에서의 한 번의 실수가 두 시간의 노력을 통째로 날려버릴 수 있다. 이 가혹함이 본작 평가의 가장 큰 분기점을 형성한다(6장 참조).

---

## 4. 평가

### 종합 점수 (Metacritic / OpenCritic)

본작은 플랫폼별로 "대체로 호의적(generally favorable)" 평가를 받았다.

| 플랫폼 | Metacritic |
|---|---|
| PC | 80 / 100 |
| Xbox Series X\|S | 79 / 100 |
| Nintendo Switch | 75 / 100 |
| PlayStation 5 | 74 / 100 |

**OpenCritic**에서는 49명의 평론가 기준 평균 약 78점, 등급 'Strong'으로 집계됐으며 평론가 추천율은 약 67%였다. ResetEra의 리뷰 스레드는 출시 시점 기준 **"83 MC / 78 OpenCritic"**으로 정리하기도 했다(플랫폼·집계 시점에 따라 수치는 다소 변동).

### 주요 평론 인용

- **Video Games Chronicle (VGC) — 5/5 (만점)**: "천재의 한 수(a stroke of genius)"라 평하며, "골프 장르를 향한 빛나는 해석이며, 훌륭하게 설계된 스테이지와 강력한 슈팅 메커닉이 플레이하는 내내 꿈같다"고 극찬.
- **GameSpot — 9/10**: 리뷰어 Steven Petite는 "An Ace In The Hole(에이스 인 더 홀)"이라는 제목으로, 컨트롤의 단순함과 Ace Card·공 스핀 메커닉을 구체적으로 칭찬.
- **Nintendo Life — 8/10**: "파(par) 이상으로 충분한, 으스스한 로그라이크"라 평. 리뷰 라운드업에서 "잠재적 걸작(potential masterpiece)"의 신호로까지 거론.
- **Push Square — 8/10**: 리뷰어 Graham Banas는 난이도를 "만족스럽다(satisfying)"고 평가. 다만 사운드트랙의 반복 가능성을 지적.
- **NME — 4/5**, **Hardcore Gamer — 4/5**, **TouchArcade — 4/5**, **Kotaku**: "GOTY 후보로 거론되는 화제작 — 당신을 박살내고 죽일 골프 게임"이라는 헤드라인으로 소개.
- **God is a Geek — 7.5/10**, **Metro GameCentral — 7/10**: 메커닉과 아트를 호평하되 로그라이크 구조의 빈틈을 지적.

### 상업 지표 및 유저 평가

본작은 소규모 인디 작품인 만큼 대형 흥행작은 아니다. 한 매출 추적 사이트(steam-revenue-calculator)는 Steam 기준 누적 총매출을 매우 보수적으로 추정해 약 $22,805(개발사 추정 순매출 약 $6,727)로 잡기도 했다 — 다만 이는 한 추정치일 뿐 실제 전 플랫폼 합산 성과와는 거리가 있을 수 있다. **Steam 유저 평가**는 679개 리뷰 기준 약 **70% 긍정**으로 집계됐다.

유저 반응의 핵심 분기점은 명확하다. 코어 메커닉·아트·음악·유머에 대해서는 폭넓은 호평이, 가혹한 난이도와 로그라이크 반복성에 대해서는 호불호가 갈렸다.

### 평론–유저 괴리

평론(메타 74~80)과 유저 평가(Steam 70% 긍정) 사이에 극단적 괴리는 없으나, 양쪽 모두 동일한 지점에서 평가가 갈렸다. 즉 "정교한 메커닉을 사랑하느냐 vs. 두 시간 런이 통째로 날아가는 좌절을 견디느냐"가 점수를 가른 단일 변수였다.

---

## 5. 성공 요인 분석

본작은 메가 히트작은 아니지만, **1인이 시작한 itch.io 프로토타입이 멀티플랫폼 정식 출시와 평단의 폭넓은 호평까지 도달한 인디 성공 사례**로서 분석할 가치가 크다.

### (1) 장르 융합이라는 디자인적 한 수

가장 결정적인 성공 요인은 **누구도 시도하지 않은 조합** — 로그라이크 × 골프 × 플랫포머 × 라이트 덱빌딩 — 을 응집력 있게 묶어냈다는 점이다. Liam Edwards는 로그라이크 팟캐스트를 듣다가 "던전 안에서 공을 튕긴다"는 물리 실험을 떠올렸고, 그 튕기는 공의 움직임에서 골프를 연상했다. 그는 "골프에서 공을 치는 행위와 게임 속 전투의 이동(combat movement)이 닮았다"는 통찰에서 출발했다. 이 비전이 단순한 컨셉 놀음에 그치지 않고, 5타 생존 룰·Ace Card·우상상·공 스핀이라는 서로 맞물리는 시스템으로 구체화된 것이 핵심이다.

### (2) 서사와 메커닉의 완벽한 정합

"이미 죽은 골퍼가 부활을 위해 도전한다"는 연옥 설정은 로그라이크의 영구 죽음·반복 도전을 서사적으로 100% 정당화한다. 많은 로그라이크가 "왜 죽으면 처음부터인가"를 억지로 끼워 맞추는 데 비해, 본작은 컨셉 자체가 그 답을 내장하고 있다. 장르 메커니즘과 픽션이 한 몸으로 설계된 보기 드문 사례다.

### (3) 작은 팀, 정상급 협업자

극소 규모 팀이면서도 핵심 협업자가 정상급이었다. 《A Short Hike》의 Mark Sparling이 만든 사운드트랙, 《Yo-kai Watch》 출신 Shiino Hiroco의 픽셀 아트가 인디 예산 대비 압도적인 프로덕션 밸류를 만들어냈다. "Castlevania meets Mario Golf"라는 명확한 음악 디렉션은 게임의 톤 전체를 규정했다.

### (4) 프로토타입 우선 검증 전략

Edwards는 완성된 상품을 먼저 만들지 않았다. 2020년 GameMaker로 만든 거친 프로토타입을 itch.io에 무료 공개하고, **트위터·디스코드로 입소문을 검증**한 뒤 퍼블리셔 계약과 정식 개발에 들어갔다. 시장 리스크를 출시 전에 크게 줄인, 모범적인 인디 검증 루프다. itch.io의 작은 데모가 결국 Switch·PlayStation·Xbox·PC 멀티플랫폼 출시로 이어진 "from itch to Switch" 서사 자체가 마케팅 자산이 됐다.

### (5) 퍼블리셔의 멀티플랫폼 동시 출시

Thunderful Publishing의 배급으로 PC·PS4/5·Xbox 전 세대·Switch에 **동일 날짜 동시 출시**가 가능했다. 소규모 인디가 단독으로 해내기 어려운 6개 플랫폼 동시 런칭은 노출과 리뷰 커버리지를 극대화했다.

### (6) 강력한 후크 — "어렵지만 공정한"

"골프의 다크 소울"이라는 별칭은 그 자체로 강력한 바이럴 후크였다. 점잖은 스포츠라는 통념을 박살내는 가혹한 난이도는, 도전을 즐기는 코어 플레이어층에게 정확히 어필했다. Kotaku가 "당신을 박살내고 죽일 골프 게임"이라 소개한 것처럼, 역설적인 가혹함이 화제성을 낳았다.

### 동시기 작품 대비 차별점

비슷한 시기의 인디 골프 게임으로는 절차적 미니 골프 《Golf With Your Friends》, 캐주얼 명작 《What the Golf?》, 물리 코미디 《Golf Story》 등이 있다. 그러나 이들 중 **로그라이크 영구 죽음과 덱빌딩 자원 관리를 골프에 정면으로 결합한 작품은 본작이 유일**하다. 《What the Golf?》가 골프의 형식을 해체하는 부조리 코미디였다면, 본작은 골프의 룰(파·스트로크)을 진지하게 재해석해 생존 자원으로 바꾼 점에서 결을 달리한다.

---

## 6. 비평적 시각 / 한계 / 논란

호평 일색은 아니었다. 본작의 약점은 명확하고, 평가가 갈리는 지점도 분명하다.

### (1) 로그라이크 구조의 불완전한 통합

가장 자주 지적된 약점이다. **Rock Paper Shotgun의 Rachel Watts**와 스페인 매체 **Vandal의 Juan Rubio**는 본작의 "로그라이크로서의 리플레이성"과 "느린 진행 속도"를 비판했다. 핵심 문제는 이렇다 — 코스가 절차적으로 생성되는 게 아니라 70여 개 수제 홀을 셔플하는 방식이라, 몇 시간만 플레이하면 **같은 홀을 여러 번 보게 된다.** 그 결과 플레이어는 초반 홀을 빨리 넘기고 싶어 서두르다 실수를 하게 되고, 반복 구간을 "건너뛰고 싶다"는 욕구를 느낀다. 진정한 로그라이크의 매번 새로운 변주가 약하다는 것이다.

### (2) 한 번의 실수 = 두 시간의 증발

한 번의 런이 약 두 시간이고, 한 홀이라도 5타를 넘기면 죽어 처음으로 돌아간다. 즉 **후반의 단 한 번 실수가 두 시간의 노력을 통째로 날려버린다.** Kotaku를 비롯한 여러 매체가 이 점을 지적했다 — "공들인 노력이 한순간에 연기처럼 사라진다(go up in smoke)." 이 가혹함은 일부에게 짜릿한 도전이지만, 다른 일부에게는 부당한 시간 낭비다.

### (3) 난이도 — 만족 vs. 불필요한 좌절

난이도 평가는 정확히 둘로 갈렸다. Push Square의 Graham Banas는 "만족스럽다"고 본 반면, **Eurogamer Italy의 Simone Cantini**는 "불필요하게 짜증난다(unnecessarily frustrating)"고 평했다. 동일한 게임을 두고 정반대 결론이 나온 것은, 본작의 난이도가 취향을 강하게 타는 양날의 검임을 보여준다.

### (4) 시야 문제 — 줌아웃의 부재

구체적인 UX 결함도 지적됐다. **Polygon의 Russ Frushtick**은 "제한된 시야와 추측에 의존하게 되는(limited vision and guesswork)" 데서 오는 좌절을 짚었다. 드라이버나 아이언으로 강하게 치면 공이 화면 밖으로 날아가는데, **충분한 줌아웃 뷰가 없어 어디에 착지할지 예측하기 어렵다**는 것이다. Birdie-Eye 카메라가 있긴 하지만, 샷의 실시간 궤도를 추적하는 데는 한계가 있다는 비판이다.

### (5) 사운드트랙의 반복성

Mark Sparling의 음악은 호평받았지만, 같은 코스·바이옴을 반복하다 보면 일부 트랙이 반복적으로 느껴진다는 지적이 따랐다(Push Square 등). 칩튠 특유의 강렬함이 장시간 반복 노출에서 피로감으로 전환될 수 있다는 것.

요약하면, 본작의 한계는 모두 **"가혹함과 반복"이라는 한 뿌리**에서 갈라져 나온다. 이 게임을 사랑하는 이유와 싫어하는 이유가 동일한 설계 결정에서 비롯된다는 점이, 본작 평가의 가장 흥미로운 구조다.

---

## 7. 영향과 유산

### 장르적 의미

《Cursed to Golf》는 상업적 메가 히트는 아니었으나, **"무엇이든 로그라이크가 될 수 있다"**는 2020년대 인디 신의 흐름을 상징하는 작품으로 남았다. 《Slay the Spire》 이후 덱빌딩 로그라이크가 폭발하고, 로그라이크 메커니즘이 모든 장르로 침투하던 시기에, 본작은 "가장 어울릴 것 같지 않은 스포츠(골프)조차 로그라이크가 될 수 있다"는 것을 설득력 있게 증명했다. 장르 융합 실험의 성공 사례로서의 레퍼런스 가치가 크다.

### 인디 개발 모델로서의 유산

본작의 진짜 유산은 **개발 경로 그 자체**일지 모른다. AAA(Rockstar) 출신 개발자가 회사를 떠나 일본으로 건너가, 영어 교사를 하며 1인 프로토타입을 GameMaker로 만들고, itch.io 무료 공개와 SNS 입소문으로 검증한 뒤, 퍼블리셔 계약을 거쳐 멀티플랫폼 정식 출시에 이르렀다. 이 "from itch to Switch" 서사는 소규모 인디 개발자에게 매우 구체적인 로드맵을 제시한다 — 거대한 완성품을 먼저 만들지 말고, 핵심 후크를 담은 프로토타입을 빠르게 공개해 시장으로 검증하라는 것.

### 문화적 의미

골프 게임 계보에서 본작은 《Mario Golf》, 《PangYa》, 《Hot Shots Golf(みんなのGOLF)》로 이어지는 아케이드 골프 전통에 명백한 헌사를 바치면서도, 그것을 진지한 도전형 로그라이크로 비틀어 새로운 하위 장르의 가능성을 열었다. Mark Sparling 사운드트랙이 바이닐 LP로까지 발매되며 인디 게임 음악 컬렉션의 일부가 된 점도 작은 문화적 발자취다.

### 후속·확장

본작은 거대한 프랜차이즈로 확장되지는 않았으나, "골프라이크(Golf-Like)"라는 개발진의 자칭 장르 명칭과 그 디자인 어휘는 이후 장르 융합을 시도하는 인디 개발자들에게 하나의 참조점이 됐다. Thunderful Publishing의 인디 포트폴리오 안에서도 독특한 장르 융합 실험으로 자리매김했다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
|---|---|
| 개발사 | Chuhai Labs (교토) |
| 퍼블리셔 | Thunderful Publishing |
| 디렉터 | Liam Edwards (전 Rockstar Games) |
| 리드 프로그래머 | Sean Fisher |
| 아트 디렉터 | Jon Davies |
| 아티스트 | Nathan Scott, Shiino Hiroco |
| 작곡 | Mark Sparling (《A Short Hike》) |
| 출시일 | 2022년 8월 18일 |
| 플랫폼 | PC, PS4, PS5, Xbox One, Xbox Series X\|S, Switch |
| 장르 | 로그라이크 / 스포츠 / 퍼즐 플랫포머 / 라이트 덱빌딩 |
| 홀 수 | 약 70개 수제 홀 풀에서 셔플 / 1런 = 18홀 |
| 기본 타수 | 매 홀 5타(PAR Count) |
| 우상상 | 골드 +4타 / 실버 +2타 |
| Metacritic | PC 80 · Xbox 79 · Switch 75 · PS5 74 |
| OpenCritic | 평균 약 78 (Strong), 추천율 약 67% |
| Steam 유저 평가 | 약 70% 긍정 (679개 리뷰 기준) |
| 사운드트랙 | 39 트랙 / 디지털·2xLP 바이닐 |

### 주요 평론 점수

| 매체 | 점수 |
|---|---|
| Video Games Chronicle (VGC) | 5/5 (만점) |
| GameSpot | 9/10 |
| Nintendo Life | 8/10 |
| Push Square | 8/10 |
| NME | 4/5 |
| Hardcore Gamer | 4/5 |
| TouchArcade | 4/5 |
| God is a Geek | 7.5/10 |
| Metro GameCentral | 7/10 |

### 주요 인터뷰·자료

- Pocket Tactics — "From itch to Switch - the story of Cursed to Golf's development" (개발 경로 상세 인터뷰): https://www.pockettactics.com/cursed-to-golf/interview
- NME — "'Cursed To Golf''s Liam Edwards tells all on his roguelike golf game": https://www.nme.com/features/gaming-features/cursed-to-golfs-liam-edwards-tells-all-on-his-roguelike-golf-game-3033923
- GamesRadar — Future Games Show 디렉터 인터뷰: https://www.gamesradar.com/cursed-to-golf-interview-future-games-show/
- Tokyo Weekender — "10 Questions With Kyoto-based Video Game Director Liam Edwards": https://www.tokyoweekender.com/tw-community/10-questions-kyoto-based-video-game-designer-liam-edwards/
- PixelSmiths Ep. 10 (팟캐스트) — Chuhai Labs 게임 디렉터 Liam Edwards: https://www.podcampmedia.com/post/pixelsmiths-ep-10-cursed-to-golf-w--chuhai-labs-game-director-liam-edwards

### 참고 자료 (영어권 매체 중심)

- Wikipedia — Cursed to Golf: https://en.wikipedia.org/wiki/Cursed_to_Golf
- GameSpot 리뷰 (9/10) — "An Ace In The Hole": https://www.gamespot.com/reviews/cursed-to-golf-review-an-ace-in-the-hole/1900-6417942/
- Kotaku 리뷰: https://kotaku.com/cursed-to-golf-review-switch-ps4-xbox-pc-1849456188
- Nintendo Life 리뷰 (8/10): https://www.nintendolife.com/reviews/switch-eshop/cursed-to-golf
- Nintendo Life — 리뷰 라운드업("Potential Masterpiece"): https://www.nintendolife.com/news/2022/08/round-up-cursed-to-golf-reviews-signal-a-potential-masterpiece
- NME 리뷰: https://www.nme.com/reviews/game-reviews/cursed-to-golf-review-3293063
- Metacritic: https://www.metacritic.com/game/cursed-to-golf/
- OpenCritic: https://opencritic.com/game/13555/cursed-to-golf
- ResetEra 리뷰 스레드 (83 MC / 78 OpenCritic): https://www.resetera.com/threads/cursed-to-golf-review-thread-83-mc-78-opencritic.621165/
- Mark Sparling — Cursed to Golf Original Soundtrack (Bandcamp): https://marksparling.bandcamp.com/album/cursed-to-golf-original-soundtrack
- Steam 스토어 페이지: https://store.steampowered.com/app/1726120/Cursed_to_Golf/
- itch.io 원작 프로토타입 (LiamBME): https://liamedwards.itch.io/cursed-to-golf

---

*본 분석서는 2022년 출시판을 기준으로 작성되었으며, 모든 평점·판매 추정치는 출처를 명시한 시점의 집계값이다. 매출 추정치(steam-revenue-calculator)는 단일 추적 사이트의 보수적 추정이므로 실제 전 플랫폼 성과와 차이가 있을 수 있다.*
