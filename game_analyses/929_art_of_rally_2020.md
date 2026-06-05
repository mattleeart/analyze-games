# 《Art of Rally》 (2020) 심층 분석

> "랠리의 황금기를, 화방에서 막 꺼낸 듯한 그림으로." — 한 사람이 캠핑밴을 몰며 만든 톱다운 랠리 게임이 어떻게 평단과 25만 명의 플레이어를 사로잡았는가.

---

## 1. 게임 개요

### 기본 정보

《Art of Rally》(공식 표기는 소문자 *art of rally*)는 캐나다 인디 스튜디오 **Funselektor Labs Inc.**가 개발·자체 퍼블리싱한 톱다운 시점의 랠리 레이싱 게임이다. 2020년 9월 23일 Windows, macOS, Linux로 먼저 출시되었고, 이후 멀티플랫폼으로 확장되었다.

- **개발/퍼블리셔**: Funselektor Labs Inc. (캐나다)
- **장르**: 톱다운(top-down) 아케이드 랠리 레이싱 / 드라이빙
- **출시일(플랫폼별)**:
  - PC(Windows/macOS/Linux): 2020년 9월 23일 (Steam, GOG, Epic Games Store)
  - Xbox One / Xbox Series X|S / Nintendo Switch: 2021년 8월 12일 (출시일 Xbox Game Pass 동시 입점)
  - PlayStation 4 / PlayStation 5: 2021년 10월 6일
  - iOS / Android: 2024년 1월 18일 (퍼블리싱: Noodlecake Studios)
- **엔진**: Unity (자사 자체 아키텍처 **FunCore** 기반으로 발전)
- **가격대**: 출시가 약 24.99 USD (한국 약 2만 5천 원 내외)

### 디렉터·주요 크레딧 — '거의 1인 개발'이라는 사실

이 게임을 이해하는 출발점은 **사실상 한 사람의 작품**이라는 점이다. Funselektor Labs는 2014년 설립된 스튜디오이지만, 그 정체성은 창립자이자 디렉터인 **Dune Casu(둔 카수, SNS 핸들 @funselektor)** 한 사람에게 거의 전적으로 수렴한다. 그는 디자인, 프로그래밍, 핸들링 물리, 아트 디렉션, 차량 모델링, 레벨 디자인의 전반을 직접 책임졌다.

핵심 협력자는 사운드트랙을 단독 작곡·프로듀싱한 우크라이나 출신 뮤지션 **Tatreal(본명 Slava Korystov / Vyacheslav Anatolevich Korystov)**이다. 즉 본질적으로 "디자이너 1명 + 작곡가 1명"의 협업 구조에 가까웠으며, 후반·콘솔 포팅 단계에서 일부 인력이 합류했지만 이 게임은 인디 '오테르(auteur, 작가주의)' 프로젝트의 전형으로 분류된다.

### 개발 기간·규모·예산

Funselektor의 데뷔작은 2015년에 나온 톱다운 드리프트 게임 《Absolute Drift》였다. Dune Casu는 게임 잼에서 만든 프로토타입을 다듬어 이 데뷔작을 냈고, 콘솔 포팅을 지원하던 중에 이미 《Art of Rally》의 프로토타입을 만지작거리고 있었다. **본격적인 풀 개발은 2017년 시작**되어 2020년 9월 출시까지 약 3년이 걸렸다.

개발 환경 자체가 이 게임의 전설을 이룬다. Dune Casu는 화물용 밴을 캠핑카로 개조해, 미국·캐나다·멕시코를 떠돌며 게임 대부분을 만들었다. 그 여정의 풍경·빛·고독이 게임의 미니멀한 자연 묘사와 명상적 톤으로 그대로 녹아들었다. 또한 그는 뉴질랜드의 랠리 스쿨과 미국의 **DirtFish 랠리 스쿨**에서 실제로 1990년대 WRC 머신을 몰아보며 랠리 주행의 감각을 직접 체득했다. 정확한 예산은 공개되지 않았으나, 1인 인디 규모임을 고려하면 매우 적은 비용으로 만들어졌고 후술하듯 수백만 달러의 매출로 회수했다.

### 기술 스택

게임 엔진은 **Unity**이며, 핸들링 물리는 전작 《Absolute Drift》의 물리 엔진을 토대로 대폭 개선한 것이다. 이후 Funselektor는 향후 Unity 프로젝트를 더 효율적으로, 버그 적고 성능 좋게 빌드하기 위한 자체 게임 비종속 아키텍처 **FunCore**를 다듬었다고 밝혔다. 비주얼은 로우폴리(low-poly) 모델 위에 고품질 라이팅과 포스트프로세싱을 얹는 방식으로, 사양 부담을 낮추면서도 미적 완성도를 끌어올린 전형적 인디 기술 전략을 취한다.

---

## 2. 게임 설명 — 이 게임이 정확히 무엇인가

### 한 줄 컨셉

《Art of Rally》는 **랠리의 황금기(golden era of rally)에 대한 미니멀리즘 헌사**다. 사실적 시뮬레이션이 아니라, 1960~80년대 랠리 머신과 전설적 스테이지를 톱다운(위에서 살짝 비스듬히 내려다보는) 시점의 양식화된 그림으로 재해석한 '아케이드 시뮬'이다. 흔히 "가장 사실적인 마이크로 머신즈(Micro Machines) 시뮬레이터"라는 농담 섞인 비유가 따라붙는다 — 장난감처럼 보이지만, 속내는 의외로 진지하다.

### 세계관·줄거리

내러티브 게임이 아니므로 전통적 줄거리는 없다. 그러나 이 게임에는 분명한 **정서적 세계관**이 있다. 그것은 "랠리라는 스포츠의 가장 위험하고 낭만적이던 시절에 대한 향수"다. 특히 1980년대 초중반의 **그룹 B(Group B)** 시대 — 무게 제한이 풀리고 출력이 폭발적으로 치솟아, 너무 빨라서 결국 사망 사고로 폐지된 그 광기 어린 황금기 — 가 정서의 중심에 있다. 차량은 라이선스 실명이 아니라 실제 명차를 연상시키는 가명("The King of Africa", "Das 559", "The Gazelle" 등)으로 등장하는데, 이는 라이선스 비용을 피하면서도 마니아가 "아, 저건 그 차"라고 알아보게 하는 영리한 장치다.

### 무드·톤·아트 디렉션

이 게임의 정수는 **아트 디렉션**이다. 핀란드의 자작나무 숲, 노르웨이의 눈 덮인 절벽, 사르데냐의 마른 흙길, 일본의 단풍과 도리이, 독일의 콘크리트 트랙, 그리고 후일 추가된 케냐의 사바나와 얼룩말까지 — 각 로케이션은 "마치 미술관에서 막 꺼내, 한 획 한 획 정성껏 칠한 그림" 같다는 평을 들었다. 로우폴리 지오메트리에 부드러운 그림자, 따뜻한 색온도, 안개와 시간대 표현이 더해져 명상적이고 평온한(zen) 분위기를 만든다. 카메라는 차량 뒤 높은 곳에 고정되어, 다가오는 코너를 미리 읽으면서도 풍경 전체를 한 폭의 그림처럼 감상하게 한다.

### 사운드·음악 — 신스웨이브의 결정체

음악은 이 게임을 단순한 레이서 이상으로 끌어올린 결정적 요소다. **Tatreal(Slava Korystov)**이 우크라이나 중부 크리비리흐(Kryvyi Rih)의 스튜디오에서 단독 작곡·프로듀싱했다. OST는 **57곡, 총 4시간 이상** 분량으로, 1970~90년대를 가로지르는 **신스웨이브(synthwave)** 헌정이다. Kraftwerk, Daft Punk, ELO, Cerrone 같은 아티스트의 향취가 깔려 있고, 사운드 제작에는 Roland TR-707, Yamaha RY30 같은 클래식 드럼머신과 Jupiter-8, Moog Modular 같은 가상 악기가 동원되었다.

독학 뮤지션인 Tatreal의 사운드트랙은 인디 게임 신스웨이브 음악 중에서도 손꼽히는 수작으로 평가받으며, Steam·Bandcamp·Spotify·Apple Music에 별도 OST로 발매되었다. 평론들이 공통적으로 "사운드트랙이 이 게임 경험의 절반"이라고 말할 만큼, 시각의 평온함과 청각의 향수가 맞물려 '주행 명상(zen driving)'이라 불리는 독특한 체험을 빚어낸다.

---

## 3. 핵심 시스템 / 메카닉 — 가장 자세하게

### 코어 게임플레이 루프

매 순간의 플레이는 단순하다. 위에서 내려다보는 카메라 아래, 흙·눈·자갈 노면 위로 클래식 랠리카를 몰며, 코너 진입 전에 브레이크를 잡고 차체를 미끄러뜨려(드리프트) 곡선을 따라 빠져나가는 것. 직선에서 가속, 코너 전 감속, 적절한 카운터스티어로 슬립을 제어, 출구에서 다시 가속 — 이 리듬이 끝없이 반복되며 '몰입 흐름'을 만든다. 스테이지는 시작점에서 종착점까지 일직선의 포인트-투-포인트 구간이며, 타임 어택이 핵심이다.

### 핸들링 모델 — '아케이드 시뮬'의 미묘한 균형

가장 정교하게 설계된 부분이 **핸들링**이다. 전작 《Absolute Drift》의 물리 엔진을 계승하되, "더 예측 가능하고 더 관대하게" 다듬었다. 즉 노골적 시뮬레이션(《Dirt Rally》류)도, 무중력 아케이드도 아니다. 차는 분명한 관성과 무게감을 갖고, 노면(눈·자갈·아스팔트)에 따라 접지력이 달라지며, 제대로 브레이크를 밟고 드리프트 각을 잡아야 날카로운 코너를 깨끗하게 통과한다. 큰 곡선을 미끄러져 빠져나가는 순간의 손맛이 일품이고, 좌우로 이어지는 연속 드리프트 콤보를 엮어낼 때의 쾌감은 더 크다.

핸들링의 진입 장벽은 양날의 검이다. 다수 평론과 유저가 초반에는 "예측 불가능하고 가파른 학습 곡선" 때문에 답답함을 느꼈다고 했지만, 일단 차의 거동에 익숙해지면 그 깊이와 숙달의 보상이 크다고 입을 모은다. "겉으로는 가볍고 유쾌하지만, 속내는 꽤 진지한 게임"이라는 평가가 여기서 나온다.

### 진행 구조 — 커리어 모드

진행의 중심은 **커리어 모드(Career)**다. 랠리의 황금기를 따라가는 구조로, 핀란드·사르데냐·노르웨이·일본·독일을 무대로 한 **약 60개 스테이지**를 차종 클래스 순서대로 풀어나간다. 시작은 비교적 다루기 쉬운 구형 클래스(흔히 Group 2 / 60년대 차)에서 출발해, 랠리를 완주하며 새 클래스와 차량을 차례로 해금한다. 차량은 **60년대 → 70년대 → 80년대 → Group B → Group S → Group 4 / Group A** 등 시대·규정별로 묶여 있으며, 출력과 다루기 어려움이 점진적으로 올라간다.

### 차량 라인업과 '가명' 디자인

출시 시점에 **50종 이상의 상징적 랠리카**가 수록되었다. 라이선스를 피하기 위해 실명 대신 가명을 쓰되, 실루엣·시대·특성으로 원형을 알아보게 했다. 그룹 B 카테고리에는 란치아 037, 푸조 205, 아우디 S1 콰트로를 연상시키는 머신이 포함되고, 케냐 업데이트로 추가된 "The King of Africa", "Das 559", "The Hyena" 같은 그룹 B 차량, "The Gazelle"(그룹 4) 등도 마니아의 향수를 자극한다. 차량마다 출력·중량·구동 방식(전륜/후륜/4륜)에 따른 거동 차이가 분명해, 같은 코너도 차가 바뀌면 전혀 다르게 공략해야 한다.

### 스테이지 정비·차량 관리

랠리 특성을 살려, 스테이지와 스테이지 **사이**에 차량을 정비하는 자원 관리 요소가 있다. 주행 중 충돌·점프 착지 실패 등으로 차가 손상되면 성능이 떨어지므로, 정비 시간을 배분해 다음 스테이지에 대비하는 전략적 판단이 들어간다. 이는 실제 랠리의 서비스 파크 개념을 가볍게 추상화한 장치다.

### 프리 로밍(Free Roam)

커리어 외에 **자유 주행(Free Roam)** 모드가 있다. 각 국가별 오픈 영역(예: 케냐의 Mara Simba)을 시간 제한·경쟁 없이 자유롭게 돌아다니며 풍경과 주행 그 자체를 즐기는 모드로, 게임의 '명상적' 정체성을 가장 잘 보여준다. 숨겨진 요소·뷰포인트를 찾아다니는 탐험적 재미도 있다.

### 온라인 이벤트 — 데일리·위클리 챌린지

라이브 운영은 가볍지만 효과적이다. **일간·주간 챌린지**가 제공되어, 정해진 차량·스테이지·조건으로 전 세계 플레이어와 같은 코스를 달리고 리더보드 순위를 겨룬다. 시즌 패스나 공격적 MTX는 없으며, 이 게임은 풀프라이스 단품 + 무료 대형 업데이트라는 정직한 모델을 택했다(상세는 7장).

### 난이도·접근성

난이도 조절 옵션이 풍부하다. 어시스트(주행 보조), 되감기(rewind, 실수한 구간을 되돌려 재시도) 등으로 캐주얼 플레이어의 진입을 돕고, 보조를 끄고 빡센 타임을 노리는 하드코어 플레이도 허용한다. "플러그 앤드 플레이"식 단순함과, 빠른 차를 해금하고 싶게 만드는 동기 부여가 결합해, 폭넓은 숙련도의 플레이어를 모두 끌어안는다.

### UI/UX 디자인 철학

UI 역시 게임의 미니멀 미학을 따른다. 잡다한 HUD를 절제하고, 화면의 시각적 평온함을 해치지 않는 선에서 필요한 정보(시간·구간·속도)만 담백하게 제시한다. 톱다운 카메라 자체가 "다가올 코너를 미리 읽는다"는 UX 기능을 겸하므로, 시뮬 랠리의 핵심인 페이스노트(co-driver의 코너 콜)에 대한 의존을 시각 정보로 상당 부분 대체한다 — 이는 페이스노트 암기 장벽을 낮추는 접근성 설계이기도 하다.

---

## 4. 평가

### 평론 점수 (Metacritic / OpenCritic)

- **Metacritic (PC)**: "generally favorable"(대체로 호평) 등급, 메타스코어 **약 77점**.
- **Metacritic (Xbox Series X|S)**: 마찬가지로 "generally favorable".
- **Metacritic (Nintendo Switch)**: "mixed or average"(보통/혼재) — Switch 포팅의 시각적 다운그레이드·성능 문제로 PC판보다 평가가 낮았다.
- **OpenCritic**: 평론가 30명 기준 **평균 81점**, **'Strong'** 등급, 추천 비율 **86%**.

### 주요 평론 인용

- **Eurogamer** — Martin Robinson은 게임을 추천하며 "brilliantly playable"(탁월하게 잘 플레이된다), "arrestingly stylish"(시선을 사로잡을 만큼 스타일리시하다)고 평했고, 차량 비주얼과 사운드트랙을 특히 칭찬했다.
- **Nintendo Life** — "Stylish Driving With Plenty Of Substance"(스타일과 알맹이를 겸비한 주행)라는 부제로, 스위치판의 한계에도 게임 자체의 완성도를 높이 샀다.
- **Checkpoint Gaming** — "Style, substance and passion"(스타일·알맹이·열정)이라는 제목으로, 1인 개발의 진심이 게임 전반에 배어 있음을 강조했다.
- **autoevolution** — "Zen Driving on the Winds of Synthwave"(신스웨이브의 바람을 타는 선(禪) 주행)라는 표현으로, 음악과 주행의 명상적 결합을 핵심 매력으로 꼽았다.
- 다수 매체가 《Art of Rally》를 "**2020년 최고의 레이싱 게임 후보**" 중 하나로, "지금껏 나온 가장 독창적인 랠리 게임 중 하나"로 평했다.

### 수상·후보

- **Global Game Awards 2020** — **Best Racing Game(최고 레이싱 게임) 후보** 지명.
- Xbox판 출시 트레일러가 PC 시절 축적한 다수의 매체 호평(accolades)을 모아 구성될 만큼, 출시 후 평단의 인정을 꾸준히 쌓았다.

### 상업 지표

- **Steam 누적 판매(추정)**: 한 서드파티 판매 추정 서비스(Steam Marketing Tool / games-stats.com)에 따르면 **약 233,365본 판매, 누적 매출 약 371만 5천 달러(약 $3.72M)**. (※ 서드파티 추정치로, 공식 발표가 아님에 유의.)
- **SteamSpy 소유자 추정**: 5만~10만 구간(서드파티 추정).
- **Steam 유저 평가**: 약 3,917개 리뷰 기준 **93% 긍정** — '매우 긍정적(Very Positive)' 수준의 압도적 호평.
- 위 수치는 Steam만 집계한 것으로, GOG·Epic·콘솔(특히 출시일 Xbox Game Pass 입점 효과)·모바일까지 합치면 실제 도달 규모는 더 크다. 1인 인디 프로젝트로서는 명백한 상업적 성공이다.

### 평론-유저 괴리

평론(메타 77 / 오픈크리틱 81)과 유저 평가(Steam 93% 긍정) 사이에 흔치 않은 '유저 우위' 괴리가 있다. 평론은 톱다운 카메라의 한계·물리의 적응 비용·콘텐츠 분량을 지적해 점수를 다소 절제한 반면, 실제로 구매한 플레이어는 미학·음악·주행감·가격 대비 만족도에서 강하게 호응했다. 즉 "리뷰 점수보다 직접 해보면 훨씬 좋다"는 전형적 인디 슬리퍼 히트의 패턴을 보인다.

---

## 5. 성공 요인 분석 — 핵심

### (1) 디자인: '미학을 메카닉으로 만든' 차별화

가장 큰 성공 요인은 **압도적 시청각 정체성**이다. 로우폴리 + 고급 라이팅의 비주얼과 Tatreal의 신스웨이브 사운드트랙이 결합해, 다른 어떤 랠리 게임과도 즉시 구별되는 인장을 만들었다. 중요한 것은 이 미학이 단순 장식이 아니라 **게임플레이 그 자체**라는 점이다. 높은 톱다운 카메라는 풍경을 그림처럼 보여주는 동시에 코너를 미리 읽게 하는 기능을 하고, 음악은 '주행 명상'이라는 핵심 경험을 완성한다. 미학과 메카닉이 한 몸이라는 점에서 이 게임은 '예쁜 인디 레이서'를 넘어선다.

### (2) 틈새 정조준: 시뮬과 아케이드 사이의 빈 자리

2020년 랠리 게임 시장은 양극화되어 있었다. 한쪽엔 하드코어 시뮬(《Dirt Rally 2.0》), 다른 쪽엔 본격 아케이드/오픈월드(《Dirt 5》, 《Forza Horizon》류)가 있었다. 《Art of Rally》는 그 사이의 빈 공간 — "쉽게 시작하지만 깊이 있게 숙달하는, 부담 없이 명상적으로 즐기는 랠리" — 을 정확히 메웠다. 또한 1980년대 그룹 B에 대한 짙은 향수는, 사실적 시뮬에서는 라이선스·물리 부담으로 제대로 살리기 어려웠던 정서적 틈새였다.

### (3) 정직한 비즈니스 모델과 신뢰 구축

이 게임은 **공정한 풀프라이스(약 25달러) + 대형 무료 업데이트**라는 모델을 택했다. 출시 후 케냐(2021)·인도네시아(2022) 같은 대규모 로케이션을 **무료**로 추가했고, 이는 기존 구매자에게 강한 신뢰와 만족을 줘 입소문(word of mouth)을 증폭시켰다. 시즌 패스·공격적 MTX가 없다는 점이 인디 게이머 커뮤니티에서 호감을 샀다.

### (4) 마케팅·출시 전략

마케팅은 게임의 비주얼 그 자체가 했다. 2019년 5월 공개 트레일러부터 정지 화면만으로도 강렬한 인상을 남겼고, 2020년 3월 **무료 공개 데모(PC)**를 배포해 핸들링이 낯선 잠재 구매자가 직접 손맛을 확인하게 했다 — 이는 진입 장벽이 있는 게임에 특히 효과적인 전략이었다. 결정적으로 2021년 콘솔 확장 시 **출시일 Xbox Game Pass 동시 입점**을 성사시켜, 수백만 구독자에게 무료로 노출되며 인지도·플레이어 기반을 폭발적으로 넓혔다.

### (5) 개발 방법론: 1인 오테르의 진정성

전작 《Absolute Drift》의 물리·미학 자산을 재활용하면서도, 실제 랠리 스쿨에서 차를 몰아본 경험과 캠핑밴 여행에서 흡수한 자연의 감각을 그대로 작품에 이식했다. 이 진정성(authenticity)은 평론·유저 모두가 반복적으로 언급한 매력으로, "한 사람의 명확한 비전"이 만들어내는 응집력이 이 게임의 일관된 톤을 가능케 했다.

### (6) 동시기 작품 대비 차별점

- 《Dirt Rally 2.0》(2019, Codemasters): 본격 시뮬. 깊지만 진입 장벽 높고 분위기가 진지. → 《Art of Rally》는 접근성·미학·평온함으로 대비.
- 《Absolute Drift》(2015, 동일 개발자): 같은 톱다운 드리프트 계보지만, 랠리·향수·자연 풍경·시대 차량이라는 새 옷을 입어 정서적 폭이 훨씬 넓다.
- 《Micro Machines》식 위트와 《Dirt》식 진지함 사이를 절묘하게 오가는 톤이 고유 포지션을 만들었다.

---

## 6. 비평적 시각 / 한계 / 논란

### 디자인적 약점

1. **카메라의 양날성**: 높고 고정된 톱다운 카메라는 미학적으로는 성공했지만, 일부 평론은 "정밀한 코너링을 방해한다"고 지적했다. 노면 굴곡·드리프트 각의 미세한 피드백을 시각으로 충분히 전달받기 어려운 순간이 있고, 빠른 그룹 B 차량에서 이 한계가 두드러진다.
2. **물리의 적응 비용**: 초반 핸들링이 "예측 불가능하다"는 평이 많다. 학습 곡선이 가팔라, 일부 플레이어는 차의 거동에 익숙해지기 전까지 좌절감을 느낀다. 시뮬도 순수 아케이드도 아닌 중간 지점이라, 두 진영 모두에서 "내가 기대한 것과 다르다"는 반응이 나올 수 있다.
3. **콘텐츠 분량과 반복성**: 스테이지가 일정 부분 반복적으로 느껴질 수 있고, 출시 시점 콘텐츠 분량이 풀프라이스 시뮬 대비 가볍다는 인상도 일부 있었다(이후 무료 업데이트로 상당히 보완).

### 기술적 이슈

- **팝인(pop-in)**: 원경 오브젝트가 늦게 그려지는 팝인이 눈에 띈다는 지적이 여러 리뷰에 등장한다.
- **플랫폼별 편차**: 특히 **Nintendo Switch판의 시각적 다운그레이드·성능 문제**가 두드러져, 같은 게임임에도 메타크리틱 등급이 PC/Xbox의 "favorable"에서 Switch의 "mixed"로 떨어졌다. 미학이 핵심인 게임에서 비주얼 손실은 체감 타격이 컸다.

### 평가가 갈리는 지점

이 게임의 호불호는 결국 **기대치 정렬** 문제다. "스타일리시한 평온한 아케이드 랠리"를 기대하면 만족도가 매우 높지만, "톱다운으로 본 《Dirt Rally》"를 기대하면 물리의 깊이·정밀함에서 아쉬움을 느낀다. 논란이라 할 만한 운영·윤리적 스캔들(MTX 남용, 거짓 마케팅 등)은 사실상 없었다는 점은, 이 게임의 평판 관리가 깨끗했음을 보여준다.

---

## 7. 영향과 유산

### 장르·인디 신에 미친 영향

《Art of Rally》는 "톱다운/양식화 시점으로도 사실적 모터스포츠의 정서를 진지하게 다룰 수 있다"는 것을 증명한 사례다. 미학·음악을 게임플레이의 핵심으로 끌어올린 설계는, 이후 분위기 중심 인디 레이서·드라이빙 게임들에 하나의 레퍼런스가 되었다. 전작 《Absolute Drift》에서 시작된 Funselektor 특유의 "미니멀 톱다운 드라이빙 + 무드 음악" 공식을 한층 성숙시켜, 일종의 작은 하위 장르로 자리매김시켰다.

### 무료 대형 업데이트라는 운영 유산

출시 후 운영은 인디 모범 사례로 꼽힌다.

- **Kenya 업데이트(2021)**: 콘솔 출시(2021년 8월)와 함께 **무료** 제공. 신규 차량 4종(그룹 B의 "The King of Africa"·"Das 559"·"The Hyena", 그룹 4의 "The Gazelle")과 6개 스테이지(Mount Kenya, Karura, Homa Bay, Ndere Island, Lake Baringo, Lake Nakuru), 그리고 새 프리로밍 지역(Mara Simba)을 추가. 사바나와 얼룩말이 등장하는 풍경은 PC Gamer 등에서 "그저 황홀하다"는 평을 받았다.
- **Indonesia 업데이트(2022년 9월 22일)**: 인도네시아 배경 6개 스테이지 추가, 역시 무료.

이러한 "콘텐츠를 팔지 않고 신뢰를 쌓는" 운영은 장기 입소문과 세일 시 재구매를 유도해 라이브 매출 곡선을 길게 유지하는 효과를 냈다.

### 플랫폼 확장과 도달 범위

PC 출시 약 1년 만에 Xbox(+Game Pass 동시), Switch, PlayStation으로, 다시 2024년 Noodlecake 퍼블리싱의 iOS/Android로 확장하며, 1인 인디 프로젝트로는 이례적으로 폭넓은 플랫폼 도달을 달성했다. 모바일 진출은 톱다운·가벼운 사양이라는 설계가 멀티플랫폼 확장에 유리하게 작용했음을 보여준다.

### 문화적 의미

《Art of Rally》는 "1인 개발자가 캠핑밴에서 만든 게임이 평단과 시장에서 통했다"는 인디 신의 낭만적 성공 서사 그 자체로 회자된다. 또한 랠리의 황금기, 특히 그룹 B에 대한 대중적 향수를 게임이라는 매체로 멋지게 보존·재현했다는 점에서 모터스포츠 팬덤 내에서도 의미 있는 작품으로 남았다. Tatreal의 사운드트랙은 게임 밖에서도 독립적으로 사랑받는 신스웨이브 앨범이 되었다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
| --- | --- |
| 개발/퍼블리셔 | Funselektor Labs Inc. (캐나다) |
| 디렉터 | Dune Casu (사실상 1인 개발) |
| 작곡 | Tatreal (Slava Korystov), 우크라이나 — OST 57곡, 4시간+ |
| 엔진 | Unity (자체 FunCore 아키텍처로 발전) |
| 풀 개발 기간 | 2017년 ~ 2020년 (약 3년) |
| PC 출시 | 2020년 9월 23일 (Win/macOS/Linux) |
| 콘솔 출시 | Xbox·Switch 2021년 8월 12일(Game Pass 동시) / PS4·PS5 2021년 10월 6일 |
| 모바일 출시 | 2024년 1월 18일 (iOS/Android, Noodlecake 퍼블리싱) |
| 출시가 | 약 24.99 USD |
| 출시 콘텐츠 | 50종 이상 차량, 약 60개 커리어 스테이지(핀란드·사르데냐·노르웨이·일본·독일) |
| 무료 대형 업데이트 | Kenya(2021, 차량 4·스테이지 6) / Indonesia(2022, 스테이지 6) |
| Metacritic | PC·Xbox "generally favorable"(약 77), Switch "mixed or average" |
| OpenCritic | 평균 81, 'Strong', 추천 86% (평론가 30명) |
| Steam 판매(서드파티 추정) | 약 233,365본 / 누적 매출 약 $3.72M |
| Steam 유저 평가 | 약 3,917개 리뷰 중 93% 긍정 |
| 수상 | Global Game Awards 2020 Best Racing Game 후보 |

### 주요 인터뷰·자료

- GamingBolt, "art of rally Interview – Art Style, Development, and More" — 아트 스타일·개발 전반에 대한 Dune Casu 인터뷰.
- Team VVV, "Art of Rally gameplay and developer interview" — 게임플레이 시연 + 개발자 인터뷰.
- Traxion.GG Podcast S4 E3, "art of rally's Dune Casu on the game's inspiration and future" — 영감과 미래 계획.
- Overcrest: A Pretty Good Podcast — "Dune Casu / Creator: Art of Rally" 에피소드.
- Funselektor 공식 About/Team 페이지 — 스튜디오·개발 배경.

### 참고 자료 목록 (영어권 매체 중심)

- [Art of Rally — Wikipedia](https://en.wikipedia.org/wiki/Art_of_Rally)
- [Funselektor 공식 About](https://www.funselektor.com/about) / [Team](https://www.funselektor.com/team)
- [art of rally 공식 사이트](https://www.artofrally.com/)
- [art of rally on Steam](https://store.steampowered.com/app/550320/art_of_rally/)
- [art of rally Reviews — Metacritic](https://www.metacritic.com/game/art-of-rally/)
- [art of rally Reviews — OpenCritic](https://opencritic.com/game/10188/art-of-rally)
- [GTPlanet — Art of Rally Takes a Top-Down Look at Rallying's Golden Age](https://www.gtplanet.net/art-of-rally-takes-a-top-down-look-at-rallyings-golden-age/)
- [GamingBolt — art of rally Interview](https://gamingbolt.com/art-of-rally-interview-art-style-development-and-more)
- [Team VVV — gameplay and developer interview](https://www.teamvvv.com/interviews/art-of-rally-gameplay-and-developer-interview/)
- [Traxion.GG — Dune Casu on inspiration and future](https://traxion.gg/art-of-rallys-dune-casu-on-the-games-inspiration-and-future-traxion-gg-podcast-s4-e3/)
- [PC Gamer — Art of Rally's big free Kenya update is out today](https://www.pcgamer.com/art-of-rallys-big-free-kenya-update-is-out-today/)
- [Nintendo Life — Art Of Rally Arrives Today With New Kenya DLC](https://www.nintendolife.com/news/2021/08/art_of_rally_arrives_today_with_new_kenya_dlc_included)
- [autoevolution — Zen Driving on the Winds of Synthwave](https://www.autoevolution.com/news/art-of-rally-review-zen-driving-the-winds-of-synthwave-164711.html)
- [Checkpoint Gaming — Style, substance and passion](https://checkpointgaming.net/reviews/2020/10/art-of-rally-review-style-substance-and-passion/)
- [The Gamer — Top-Down Rally Cry](https://www.thegamer.com/art-of-rally-review/)
- [Tatreal — Art of Rally Original Soundtrack (Bandcamp)](https://tatreal.bandcamp.com/album/art-of-rally-original-soundtrack)
- [games-stats.com — art of rally revenue and stats](https://games-stats.com/steam/game/art-of-rally/)
- [SteamSpy — art of rally](https://steamspy.com/app/550320)

---

*본 분석서는 영어권 매체·공식 자료·서드파티 통계를 종합해 작성되었다. 판매·소유자 수치는 명시한 대로 서드파티 추정치이며, 공식 발표가 아님을 밝혀 둔다.*
