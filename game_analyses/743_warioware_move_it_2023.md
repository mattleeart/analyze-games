# 《WarioWare: Move It!》 (2023) 심층 분석

> 닌텐도의 가장 무정부주의적인 IP가 17년 만에 모션 컨트롤의 본가로 귀환했다. 《WarioWare: Move It!》은 2006년 Wii 시절의 명작 《WarioWare: Smooth Moves》를 직계 계승한 시리즈 첫 "정통 속편"이며, Joy-Con의 자이로·적외선 카메라를 통째로 신체 동작 인터페이스로 끌어올린 파티 게임이다. 5초짜리 미니게임(마이크로게임) 200여 개가 신체를 비틀고 흔들게 만드는 이 작품은, 평론과 상업 양면에서 명백한 한계를 안고도 "왜 모션 게임이 여전히 재미있을 수 있는가"를 가장 순수한 형태로 증명한다.

---

## 1. 게임 개요

### 기본 정보

| 항목 | 내용 |
|------|------|
| 정식 명칭 | 《WarioWare: Move It!》 (일본 원제: 『おすそわける メイド イン ワリオ』, 북미 출시명 WarioWare: Move It!) |
| 개발사 | Intelligent Systems (개발 보조: Tose) |
| 퍼블리셔 | Nintendo |
| 플랫폼 | Nintendo Switch (단독) |
| 출시일 | 2023년 11월 3일 (전 지역 동시) |
| 공개일 | 2023년 6월 21일 Nintendo Direct |
| 장르 | 파티 / 미니게임 모음 (마이크로게임) |
| 시리즈 위치 | 《WarioWare》 정규 시리즈 12번째 작품, 시리즈 사상 첫 직계 속편 |

### 핵심 크레딧

- **치프 디렉터(Chief Director):** Goro Abe — 《WarioWare》 시리즈의 사실상 산파이자 오랜 리드 개발자. 초대작부터 시리즈를 지켜온 인물로, 《Smooth Moves》(2006)의 디렉터이기도 하다. 본작이 "Smooth Moves의 정통 후속"으로 설계된 것은 그의 존재와 직결된다.
- **디렉터:** Goro Abe, Waki Shigeta
- **프로듀서:** Kensuke Tanabe(닌텐도 측 베테랑 프로듀서), Shinya Saito, Atsushi Ikuno
- **디자이너:** Nami Komuro
- **프로그래머:** Yusuke Kitayama
- **아트:** Ko Takeuchi(시리즈 간판 아티스트, 워리오 패거리의 시그니처 캐릭터 디자인 담당), Hiroki Kawamae
- **음악:** Jo Kondo, Haruno Ito, Shomo Murata

### 개발 배경 및 규모

본작의 출발점은 Switch 하드웨어 위에서 모션 컨트롤이 다시 "팔릴 수 있는" 환경이 형성되었다는 판단이었다. Goro Abe는 Nintendo Life와의 인터뷰에서 《Ring Fit Adventure》(2019)처럼 신체를 움직이는 Switch 타이틀이 호응을 얻는 흐름을 언급하며 *"플레이어가 Joy-Con을 들고 몸을 움직이는 《WarioWare》를 만들면 재미있겠다"*고 발상했다고 밝혔다. 직전작인 《WarioWare: Get It Together!》(2021)이 캐릭터 조작 기반의 전혀 다른 메카닉이었기에, 같은 플랫폼에서 두 게임이 서로 다른 정체성으로 공존할 명분이 있었다는 것이다.

개발 스케일은 《WarioWare》 특유의 "다품종 소량생산" 구조를 잘 보여준다. 마이크로게임 제작에는 약 80명이 투입되었고, 서로 다른 아티스트–프로그래머 페어가 각자 개별 게임을 만들어내는 방식이었다. 이것이 작품의 압도적인 다양성과 톤의 들쭉날쭉함을 동시에 낳은 원인이다. 가장 인상적인 수치는 아이디어 단계의 규모다. Abe에 따르면 초기 발상 단계에서 사내 전 부서로부터 **1,000개 이상의 마이크로게임 아이디어**를 수집했고, 그중 보스 게임을 포함해 최종 **223종**을 선별·완성했다. 즉, 다섯 중 하나꼴로 살아남은 셈이다. 유일한 사전 제약은 "Form(자세) 종류를 먼저 정해 둔 것"뿐이었고, 그 외에는 직원들의 상상력을 최대한 풀어놨다고 한다.

### 기술 스택

본작은 Switch의 Joy-Con에 내장된 **자이로스코프(gyroscope)**와 **적외선(IR) 모션 카메라**를 핵심 입력으로 삼는다. Abe는 Wii 리모컨이 가속도계(accelerometer) 중심이었던 데 비해, Joy-Con의 자이로는 *"더 미세한 움직임"*을 잡아낼 수 있어 "Squat Form"에서 다리·엉덩이 움직임까지 감지할 수 있었다고 설명한다. 오른쪽 Joy-Con 하단의 IR 카메라는 일부 마이크로게임에서 손 모양·거리 인식에 쓰여, 단순 흔들기를 넘어선 입력 다양성을 만들었다. 엔진은 닌텐도 1st/2nd party 사내 프레임워크 기반(공식 미공개)으로 추정되며, 시각적으로는 시리즈 전통의 저해상도 픽셀·러프한 손그림·3D가 뒤섞인 "의도적 잡탕" 스타일을 유지한다.

---

## 2. 게임 설명

### 컨셉

《WarioWare》는 닌텐도 IP 가운데 가장 반(反)정형적인 시리즈다. 일반적인 "게임 한 판"을 5초 단위로 분쇄해, 각각이 단 하나의 동사(피하라, 잡아라, 눌러라, 흔들어라)로 환원된 초소형 게임 = **마이크로게임**을 쉴 틈 없이 연속으로 던진다. 플레이어는 화면에 1~2단어로 뜨는 지시("DODGE!", "GRAB!")만 보고 직관적으로 정답 동작을 수행해야 하며, 실패하면 목숨이 깎이고 일정 게임을 넘기면 스테이지 보스가 등장한다. 본작의 차별점은 이 모든 입력을 손가락 버튼이 아니라 **온몸의 자세(Form)와 동작**으로 처리한다는 점이다.

### 세계관과 줄거리 [스포일러 포함]

이야기는 전형적인 《WarioWare》식 난센스다. 햄버거 노점이 트로피컬 휴양지 **Caresaway Island(케어서웨이 섬)**의 광고를 띄우자, 워리오는 마늘버거 50개를 한 번에 주문해 — 그 대가로 친구 스무 명과 함께 떠나는 무료 휴가권을 당첨시킨다. 정작 본인은 친구들을 데려가기 싫어하지만, 워리오의 패거리(시리즈 단골 캐릭터 19인)는 그의 환호를 엿듣고는 다 함께 요트를 타고 섬으로 향한다.

섬에 도착한 일행은 각자 한 쌍씩 **Form Stones(폼 스톤)**를 받는다. 폼 스톤은 오래전 강력한 신이 섬에 내린 전설의 유물로, "함께 춤추는 자에게 행운을 가져다준다"고 전해진다. 이 폼 스톤이 본작의 18종 Form(자세) 시스템을 서사적으로 정당화하는 장치다. 이후 각 캐릭터별 챕터가 펼쳐진다 — Dr. Crygor·Penny·Mike는 석기시대로 시간여행해 동굴벽화의 모델이 되고, Ashley는 블루베리를 먹고 작아진 Red를 원래 크기로 되돌리려 하며, Orbulon은 기억상실로 신전 주민들에게 신으로 오해받고, Kat과 Ana는 선인장 괴물 무리(Cractus)에게서 섬 지도를 되찾으려 하며, Young Cricket은 펭귄 군단과 싸우고, Jimmy T.는 상어 위에서 서핑을 하며, Dribble과 Spitz는 수상 레이스에 참가하고, 9-Volt는 으스스한 가게에서 5-Volt·18-Volt·13-Amp를 구해내려 한다.

**[스포일러]** 최종 스테이지에서 워리오는 신전으로 돌아와 황금 보물을 훔치려다 용암에 삼켜져 **부패·변이하며 섬의 거대 화산과 융합**한다. 거대한 화산 워리오가 되어 섬에 재앙을 일으키자, 친구들이 폼 스톤의 힘으로 그를 쓰러뜨려 사태를 수습한다. 전형적인 "탐욕이 부른 자업자득" 구조이되, 서사는 어디까지나 마이크로게임을 꿰는 얇은 실에 불과하다.

### 캐릭터

본작은 시리즈 역대 캐릭터 대부분을 총출동시킨다 — 워리오를 중심으로 Mona, Jimmy T., Dribble & Spitz, Mona, 9-Volt & 18-Volt, 5-Volt, Kat & Ana, Ashley & Red, Dr. Crygor, Penny, Mike, Young Cricket & Master Mantis, Orbulon, Fronk, Lulu, 13-Amp 등. 각 캐릭터는 스토리 모드에서 자신만의 스테이지를 호스트하며, 파티 모드에서는 플레이어가 고를 수 있는 크루 멤버로 등장한다.

### 무드·톤·아트 디렉션

《WarioWare》의 정체성은 "닌텐도가 허락한 무질서"다. 손그림 픽셀, 클립아트, 저질 3D, B급 광고 패러디가 한 화면에서 충돌하고, 유머는 화장실 개그와 부조리극 사이를 넘나든다. 본작은 여기에 신체성을 더해, 거실에서 친구들이 Joy-Con을 머리 위로 들거나 엉덩이를 흔드는 우스꽝스러운 광경 자체를 콘텐츠로 만든다. NPR이 본작을 *"가족과 친구를 꿈틀대는 카오스 임프(squirming chaos imps)로 변신시킨다"*고 표현한 것이 톤을 정확히 요약한다.

### 사운드·음악

음악은 Jo Kondo, Haruno Ito, Shomo Murata가 맡았다. 시리즈 전통대로 짧고 중독적인 루프, 캐릭터 테마, 효과음 범벅의 보스 BGM이 빠른 템포의 게임플레이를 받친다. 특기할 변화는 **성우 교체**다. 2023년 8월 21일 닌텐도는 오랫동안 워리오를 비롯한 다수 캐릭터를 연기한 **Charles Martinet**의 음성 출연 종료를 발표했고, 본작에서 그의 부재가 확정되었다. 11월 1일에는 《Super Mario Bros. Wonder》에서 마리오·루이지를 맡은 **Kevin Afghani**가 워리오 역을 이어받았음이 확인되었다. 마틴넷 시대 이후의 워리오 보이스가 본격적으로 데뷔한 초기 작품 중 하나라는 점에서 시리즈 사적 의미가 있다.

---

## 3. 핵심 시스템 / 메카닉

### 코어 루프: Form → 지시 → 동작

본작의 모먼트-투-모먼트는 다음과 같이 돌아간다. 한 마이크로게임이 시작되기 직전, 화면은 먼저 **Form(자세)**을 지시한다 — 가령 "Sky Stretch"라면 양손 Joy-Con을 머리 위로 뻗어 들고, "Choo Choo"라면 옆구리에 붙인다. 플레이어가 그 자세를 취하면 곧바로 5초짜리 마이크로게임이 시작되고, 1~2단어 지시("PULL!", "SWAT!")에 맞춰 그 자세를 기준으로 손을 움직여 과제를 푼다. 핵심은 **하나의 Form이 여러 마이크로게임을 묶는 "입력 문법"**으로 작동한다는 것이다. 같은 "At Attention" 자세에서 거수경례를 하기도 하고, 낚싯대를 채기도 한다. 이 추상화가 모션 게임의 고질병인 "무슨 동작을 해야 하는지 모르겠다"를 상당 부분 해소한다.

### Form(자세) 시스템: 18종

본작은 **223종의 마이크로게임을 18종의 Form**으로 조직한다. 확인된 Form 목록에는 Choo-Choo(구 "The Diner"의 개명), Sky Stretch, Knight, Massage, Big Cheese, Tug-of-War, Scales, Lifter, Gift Giver, Ba-KAW, At Attention, Fashionista, Hand Model, Crocodile, Squat, Archer, Lovestruck, Pounce 등이 있다. 이 중 **Big Cheese와 Tug-of-War는 《Smooth Moves》에서 직접 계승**된 자세이며, "The Diner"가 "Choo Choo"로 이름만 바뀌어 돌아왔다 — 정통 속편임을 드러내는 의도적 오마주다.

설계상 흥미로운 점은 **좌우 비대칭 처리**다. "Knight", "Tug-Of-War", "Ba-KAW", "Fashionista", "Crocodile", "Archer" 등의 Form은 왼손잡이/오른손잡이에 따라 Joy-Con 잡는 위치가 달라진다. 초반 자세는 머리 위로 들기(Sky Stretch)나 옆구리에 붙이기(Choo Choo)처럼 매우 단순하게 시작해, 후반으로 갈수록 한 손은 입에 새 부리처럼, 다른 한 손은 엉덩이에 대는 식의 우스꽝스럽고 복잡한 동작으로 난도와 황당함이 동시에 올라간다.

### 자이로와 IR 카메라의 정밀 입력

본작의 입력 정밀도는 Wii 시절 대비 진일보했다. Joy-Con 자이로는 미세 회전·기울기를 잡아, 예컨대 Squat Form에서 무릎 굽힘과 엉덩이 흔들기를 구분한다. 한 마이크로게임은 Joy-Con을 등 뒤로 돌려 엉덩이로 우주 공간에 도형을 그리게 하고(Digital Trends가 "마리오 3의 너구리 슈트를 엉덩이로 조종했다"고 표현), 또 다른 게임은 한 손을 입에, 한 손을 엉덩이에 대게 한다. 오른쪽 Joy-Con의 IR 카메라는 손 모양·물체 인식을 더해 단순 모션을 넘어선 변주를 제공한다.

### 진행 구조: 스토리 모드

싱글플레이 메인은 **스토리 모드**로, 캐릭터별 스테이지(섬의 각 구역)를 순회한다. 각 스테이지는 일군의 마이크로게임 + **보스 게임**으로 마무리되며, 새 스테이지마다 새 Form 1~2종이 도입된다(예: "Mermaid Meet and Greet"가 Sky Stretch·Knight를, "A Curious Case of Cave Art"가 Massage·Big Cheese를 처음 소개). 마이크로게임은 진행할수록 속도(템포)와 난도가 올라가, 후반에는 같은 게임도 더 빨리·더 변칙적으로 등장한다. 메인 스토리 자체는 **2시간 안쪽**에 클리어 가능할 만큼 짧고, 이후 콘텐츠는 점수 갱신·미니게임 해금·멀티 모드로 외연을 넓힌다.

### 멀티플레이: 협력과 파티

본작의 무게중심은 명백히 멀티플레이다.

- **로컬 협력(2인):** 두 플레이어가 동기화해 마이크로게임을 함께 푸는 모드. 평론이 가장 호평한 구간으로, "둘이서 하면 게임이 솟아오른다"는 평가가 다수다.
- **파티 모드(최대 4인):** 각 플레이어가 크루 멤버를 골라 즐기는 **다섯 가지 모드**를 담는다. 확인된 모드로는 Galactic Conquest, Listen to the Doctor, Medusa March, Go the Distance, 그리고 4인 전용 The "Who's in Control?" Show가 있다. 다만 보드게임형 모드는 "Mario Party보다 깊이가 얕다"는 지적을, 3~4인 파티 전반은 "실망스럽다"는 평을 받았다.
- **Copycat Mirror:** Ashley와 Red가 호스트하는 부가 모드로, 한 플레이어가 TV를 등지고 서서 다른 플레이어의 동작을 거울처럼 따라 한다. 모션 콘셉트를 사회적 놀이로 확장한 사례다.

### 난이도·접근성

접근성은 본작의 가장 논쟁적인 약점이다. **착석(seated) 대체 동작이 거의 제공되지 않는다.** 일부 동작은 앉아서도 가능하지만, 스쿼트나 점프처럼 본질적으로 서서 해야 하는 게임은 대체 불가다. 즉 본작은 사실상 **기립 + 전신 가동 범위 + 약간의 활동 공간**을 전제한다. TechRadar·Yahoo Tech 등은 이를 "거대한 접근성 누락(accessibility nightmare)"으로 비판했고, 거동·공간에 제약이 있는 플레이어가 배제된다는 점을 정면으로 문제 삼았다.

### UI/UX 디자인 철학

Abe가 밝힌 핵심 원칙은 *"마이크로게임의 조작과 규칙은 직관적이어야 하며, 누구나 즉시 작동 방식을 파악할 수 있어야 한다"*는 것이다. 목표 체감은 "두세 번째 시도면 성공"하는 수준이고, 테마는 연령·배경을 가리지 않고 통해야 한다. 플레이테스트에서는 초심자가 헷갈리거나 입력이 안 잡히는 지점을 관찰해 반복 수정했으며, "컨트롤러를 등에 대야 하는" 프로토타입처럼 직관에 어긋나는 발상은 폐기·조정했다고 한다. 즉 본작의 UX는 "가르치지 않고 보여줘서 즉시 이해시키는" 마이크로게임 특유의 설계 철학을 신체 동작 영역으로 확장한 결과물이다.

---

## 4. 평가

### 종합 점수

| 매체/집계 | 점수 |
|-----------|------|
| Metacritic (Switch) | **75 / 100** (약 90개 리뷰) |
| OpenCritic | 추천율 **약 56%** (약 81개 리뷰) |
| Famitsu | **35 / 40** |

### 개별 평론 (확인된 점수)

| 매체 | 점수 |
|------|------|
| Nintendo Life | 8 / 10 |
| Famitsu | 35 / 40 |
| GamesRadar+ | 4 / 5 |
| IGN | 7 / 10 |
| Destructoid | 7 / 10 |
| Shacknews | 7 / 10 |
| GameSpot | 6 / 10 |
| Eurogamer | 3 / 5 |
| PCMag | 3.5 / 5 |
| Hardcore Gamer | 3 / 5 |

### 주요 평론 인용

- **Nintendo Life (8/10):** "Wii 시절 모션 기반 광기로의 멋진 귀환(A Fine Return For Wario's Wii-Era, Motion-Based Mayhem)"이라 평하며 창의성과 멀티플레이를 칭찬하되, 싱글플레이 선택지의 빈약함을 지적했다.
- **GamesRadar+ (4/5):** "Switch가 마땅히 받아야 할 워리오 파티 게임"이라 호평했다.
- **GameSpot (6/10):** 모션의 즐거움은 인정하되, 깊이 부족과 간헐적 컨트롤 인식 문제가 장기적 만족을 가로막는다고 봤다.
- **Eurogamer (3/5):** 콘텐츠의 결핍과 솔로 플레이의 사실상 부재("virtually nonexistent longevity for those who will want to play solo")를 비판했다.
- **NPR:** "두 명이서는 훌륭하지만 그 이상에서는 어중간하다(terrific for two players, middling for more)" — 협력은 솟아오르지만 파티 모드는 그만큼이 아니라는 본작 평가의 전형을 요약.

### 상업 지표

본작은 시리즈 평균에 못 미치는 상업 성적을 냈다. 일본 발매 첫 주 판매량은 **약 29,000장(주간 3위)**으로, Game Data Library 집계 기준 이는 **시리즈 일본 리테일 런칭 사상 두 번째로 낮은 수치**(Wii U작들 다음)였고, 《Get It Together!》나 《Smooth Moves》 런칭의 절반에도 못 미쳤다. 이후 누적은 **2024년 2월 기준 약 167,000장(일본)**, 후속 보고에서는 약 172,000장 수준으로 집계됐다. 글로벌 판매는 닌텐도가 별도 수치를 공개하지 않았으나, 일본 런칭의 약세는 본작이 시리즈 내에서 상업적 화제작이 되지 못했음을 시사한다. (모든 수치는 Famitsu/Gematsu, VGChartz, Game Data Library 등 외부 집계 기준이며 닌텐도 공식 발표가 아닌 점에 유의.)

### 평론-유저 괴리

평단의 "좋지만 얇다"는 합의와 달리, 실제로 거실에서 여럿이 즐긴 플레이어층의 체감 만족은 더 높은 경향이 있다. 본작은 "혼자 콘텐츠를 소비하는 게임"이 아니라 "사람들과 함께하는 자리에서 빛나는 게임"이라, 리뷰 점수(주로 싱글·가성비·롱제비티 축으로 채점)와 실사용 경험 사이에 구조적 간극이 존재한다.

---

## 5. 성공 요인 분석

본작은 흥행 대박은 아니었으나, "왜 이 게임이 평가와 애정을 얻었는가"라는 디자인적 성공 요인은 분명하다.

### (1) 17년 만의 "정통 속편"이라는 포지셔닝

《WarioWare》 시리즈는 휴대용·거치형을 오가며 매번 입력 방식을 갈아 끼워 왔지만, "Wii 리모컨으로 온몸을 흔드는" 《Smooth Moves》는 그중에서도 컬트적 사랑을 받은 정점이었다. 본작은 시리즈 첫 직계 속편을 표방하며 Big Cheese·Tug-of-War 같은 Form을 되살려, 17년간 "그 경험의 재림"을 기다린 팬덤의 정확한 욕구를 겨냥했다. 한 평론가가 "Nintendo에게서 17년간 원했던 바로 그것"이라 쓴 것이 이 포지셔닝의 위력을 보여준다.

### (2) Joy-Con 자이로·IR의 적시 활용

Wii 리모컨 가속도계의 거친 입력은 《Smooth Moves》의 한계이기도 했다. 본작은 그 사이 성숙한 Joy-Con 자이로·IR 카메라로 더 미세한 동작을 잡아내, "동작은 황당하되 인식은 정확한" 균형을 상당 부분 달성했다. 즉 단순 리메이크가 아니라 하드웨어 세대교체가 만든 신작이었다.

### (3) "동작 자체가 콘텐츠"인 사회적 설계

본작의 진짜 게임은 화면 안이 아니라 거실 안에서 벌어진다. 친구들이 폼 스톤 지시에 따라 머리 위로 손을 뻗고 엉덩이를 흔드는 광경 자체가 웃음과 유대를 만든다. 이는 《Jackbox》류 파티 게임, 《Just Dance》, 《Mario Party》가 공유하는 "관전이 곧 콘텐츠"인 성공 공식을, 5초 마이크로게임의 속도감으로 압축한 것이다.

### (4) 압도적 다양성의 생산 방식

1,000개 이상 아이디어에서 223개를 추린 선별 과정, 80여 명이 페어를 이뤄 개별 게임을 만든 분산 제작은 "두 게임도 똑같지 않은" 변주를 보장했다. 이 비효율적으로 보이는 다품종 생산이 역설적으로 시리즈의 핵심 매력(예측 불가)을 떠받친다.

### (5) 낮은 진입장벽과 즉시성

"두세 번째 시도면 성공"하는 직관성, 1~2단어 지시, 연령 불문 테마라는 설계 철학은 비게이머·가족·파티 손님을 즉시 끌어들인다. 학습 곡선이 사실상 없다는 점이 거실 게임으로서의 범용성을 만든다.

### (6) 동시기 경쟁작 대비 차별점

같은 파티/모션 영역의 《Just Dance》는 춤(리듬)에, 《Mario Party》는 보드게임 메타에, 《Jackbox》는 스마트폰·텍스트 위주에 특화돼 있다. 본작은 "초고속 신체 반응"이라는 틈새를 점유해, 이들과 직접 경쟁하기보다 보완재로 자리한다.

---

## 6. 비평적 시각 / 한계 / 논란

### (1) 빈약한 싱글플레이와 롱제비티

가장 일관된 비판은 콘텐츠 부피다. 메인 스토리는 2시간 안쪽에 끝나고, 솔로 플레이어를 위한 장기 동기가 부족하다. Eurogamer가 "거리(시간) 대비 콘텐츠가 원시적이고, 솔로용 수명은 사실상 전무하다"고 못 박은 것이 대표적이다.

### (2) 멀티의 무게중심 편향

협력(2인)은 호평이지만, 그 대가로 싱글이 희생되었다는 인상이 강하다. 또한 3~4인 파티 모드는 보드형 모드가 "Mario Party보다 얕다"는 평가처럼, 협력 모드만큼의 완성도를 보여주지 못했다. "둘이면 최고, 그 이상이면 어중간"이라는 NPR의 요약은 본작 평가의 구조적 균열을 정확히 짚는다.

### (3) 접근성 문제 (가장 심각한 논란)

착석 대체 동작의 부재는 단순 불편을 넘어 배제의 문제로 비판받았다. 거동·공간 제약이 있는 플레이어, 좁은 거실, 야간·소음 민감 환경에서는 상당수 마이크로게임을 정상적으로 플레이할 수 없다. TechRadar는 이를 "플레이어가 대가를 치르는 거대한 접근성 이슈"로 규정했다. 닌텐도가 《Smooth Moves》 시절보다 접근성 감수성이 높아진 시대에 내놓은 작품임을 고려하면, 명백한 설계 누락으로 지적된다.

### (4) 모션 인식의 간헐적 불안정

자이로·IR이 개선됐다고는 하나, 일부 마이크로게임에서 의도한 동작이 인식되지 않거나 환경(조명·공간)에 따라 입력이 흔들리는 사례가 보고됐다. "작동할 때는 훌륭하지만(when it works)"이라는 단서가 여러 리뷰 제목에 붙은 이유다.

### (5) 시리즈 정체성의 양날

"매번 다른 입력 방식"은 시리즈의 매력이자 위험이다. 본작의 전신 모션은 휴대 모드·취침 전·대중교통 등 Switch의 핵심 사용 맥락과 충돌하며, "언제 어디서나"라는 Switch의 강점을 스스로 반납한다. 이것이 상업적 약세(특히 일본 런칭 부진)의 한 요인으로 추정된다. [추정]

---

## 7. 영향과 유산

### 장르·시리즈 내적 의미

본작은 《WarioWare》가 "정통 속편을 만들 수 있는 시리즈"임을 처음 입증했다. 그간 시리즈는 매 작품 콘셉트를 갈아 끼우는 것을 자기 정체성으로 삼았기에, 특정 과거작(Smooth Moves)을 직접 계승한다는 선택 자체가 이례적이었다. 이는 닌텐도가 자사의 컬트 명작에 대한 팬덤 자산을 회수·재투자하는 방식의 한 사례다.

### 모션 컨트롤 부흥의 맥락

본작은 《Ring Fit Adventure》, 《Nintendo Switch Sports》 등 Switch 후기 라이프사이클의 "신체 활동형 캐주얼 라인업" 흐름 위에 놓인다. Joy-Con 모션이 Wii 시절의 향수를 넘어 여전히 거실 파티의 유효한 인터페이스임을 재확인했고, 동시에 그 한계(접근성·휴대성과의 충돌)도 함께 드러냈다.

### 성우 세대교체의 분기점

Charles Martinet의 음성 출연 종료 직후 Kevin Afghani 체제의 워리오가 본격 등장한 초기 작품이라는 점에서, 본작은 마리오 패밀리 보이스의 세대교체라는 닌텐도 IP 사적 변곡점의 한 자락을 차지한다.

### 문화적 의미

전신을 비틀게 만드는 본작의 마이크로게임들은 스트리밍·SNS에서 "남이 하는 모습이 더 웃긴" 콘텐츠로 소비됐다. "엉덩이로 우주에 그림 그리기" 같은 동작은 클립화하기 좋은 밈성 소재로, 게임이 관전·공유 문화 속에서 작동하는 방식을 보여줬다. 비록 대형 흥행작은 아니지만, "닌텐도가 여전히 가장 기이하고 순수한 놀이를 만들 수 있다"는 브랜드 자산을 강화한 작품으로 남는다.

### 후속·계승

본작 자체가 모방작을 양산하지는 않았으나(마이크로게임 포맷은 본래 모방이 어려운 닌텐도 고유 영역), 시리즈가 "각 하드웨어의 신규 입력 기능을 가장 먼저·가장 과감히 실험하는 테스트베드"라는 전통을 이어갔다는 점에서 의미가 있다. 차세대 하드웨어가 새 입력 방식을 도입할 때 《WarioWare》가 다시 그 쇼케이스가 될 가능성을 본작이 재확인했다.

---

## 8. 부록

### 핵심 통계 표

| 지표 | 값 |
|------|-----|
| 마이크로게임 수 | 223종 (보스 게임 포함) |
| Form(자세) 종류 | 18종 |
| 초기 수집 아이디어 | 1,000개 이상 |
| 마이크로게임 제작 인력 | 약 80명 |
| 메인 스토리 클리어 시간 | 약 2시간 이내 |
| 최대 동시 인원 | 4인 (파티 모드) |
| 파티 모드 수 | 5종 |
| Metacritic | 75/100 |
| OpenCritic 추천율 | 약 56% |
| Famitsu | 35/40 |
| 일본 첫 주 판매 | 약 29,000장 (주간 3위) |
| 일본 누적(2024.2) | 약 167,000장 |

### 주요 Form 목록 (18종)

Choo-Choo(구 The Diner), Sky Stretch, Knight, Massage, Big Cheese(Smooth Moves 계승), Tug-of-War(Smooth Moves 계승), Scales, Lifter, Gift Giver, Ba-KAW, At Attention, Fashionista, Hand Model, Crocodile, Squat, Archer, Lovestruck, Pounce.

### 파티/멀티 모드

- 로컬 협력(2인 동기 플레이)
- Galactic Conquest
- Listen to the Doctor
- Medusa March
- Go the Distance
- The "Who's in Control?" Show (4인 전용)
- Copycat Mirror (Ashley & Red 호스트, 동작 따라하기)

### 주요 인터뷰

- Nintendo Life, "Butt Movements, Pitches, And 9-Volt's Retro Microgames — We Speak With WarioWare's Chief Director" (Goro Abe 인터뷰): 1,000개 아이디어→223개 선별, Joy-Con 자이로의 미세 동작 감지, 9-Volt 레트로 게임 제작 시 원작 데이터 수배 일화, 80인 분산 제작, 직관성 설계 철학 등.
- Goro Abe, 《Smooth Moves》 시절 E3 Q&A(Game Developer / Gamasutra 아카이브): 본작의 직계 전작 설계 사상 참고.

### 참고 자료 목록 (영어권 중심)

- [WarioWare: Move It! — Wikipedia](https://en.wikipedia.org/wiki/WarioWare:_Move_It!)
- [WarioWare: Move It! — Super Mario Wiki](https://www.mariowiki.com/WarioWare:_Move_It!)
- [List of WarioWare: Move It! microgames — Super Mario Wiki](https://www.mariowiki.com/List_of_WarioWare:_Move_It!_microgames)
- [Form Stones — Super Mario Wiki](https://www.mariowiki.com/Form_Stones)
- [WarioWare: Move It! Reviews — Metacritic](https://www.metacritic.com/game/warioware-move-it/)
- [WarioWare: Move It! Reviews — OpenCritic](https://opencritic.com/game/15395/warioware-move-it-)
- [Review: WarioWare: Move It! (Switch) — Nintendo Life](https://www.nintendolife.com/reviews/nintendo-switch/warioware-move-it)
- [Butt Movements, Pitches, And 9-Volt's Retro Microgames — Goro Abe Interview, Nintendo Life](https://www.nintendolife.com/features/butt-movements-pitches-and-9-volts-retro-microgames-we-speak-with-wariowares-chief-director)
- ['WarioWare: Move It!' Review — NPR](https://www.npr.org/2023/11/01/1209770371/warioware-move-it)
- [WarioWare: Move It review — GamesRadar+](https://www.gamesradar.com/warioware-move-it-review/)
- [WarioWare: Move It! has a huge accessibility issue — TechRadar](https://www.techradar.com/gaming/nintendo-switch/warioware-move-it-has-a-huge-accessibility-issue-and-players-are-paying-the-price)
- [WarioWare: Move It! let me control Mario 3's Tanooki suit with my butt — Digital Trends](https://www.digitaltrends.com/gaming/warioware-move-it-hands-on-impressions/)
- [Famitsu Sales: 2/12/24 – 2/18/24 — Gematsu](https://www.gematsu.com/2024/02/famitsu-sales-2-12-24-2-18-24)
- [Sales — WarioWare: Move It! — VGChartz](https://www.vgchartz.com/game/231910/warioware-move-it/sales)

---

*본 분석은 2026년 6월 기준 영어권 공개 자료(닌텐도 공식 인터뷰, Metacritic/OpenCritic 집계, IGN·Nintendo Life·GameSpot·Eurogamer·NPR 등 평론, Wikipedia·Super Mario Wiki, VGChartz·Gematsu·Game Data Library 판매 집계)를 종합·재구성한 것이다. 판매 수치는 외부 집계 기반이며 닌텐도 공식 발표가 아닌 점, 일부 모드·Form 명칭은 지역판에 따라 다를 수 있는 점을 밝힌다.*
