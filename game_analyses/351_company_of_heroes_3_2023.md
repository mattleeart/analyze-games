# Company of Heroes 3 (2023) 심층 분석

> 《Company of Heroes 3》는 2023년 2월 23일 출시된 Relic Entertainment의 제2차 세계대전 실시간 전술(RTS) 게임으로, 7년의 공백을 깨고 돌아온 시리즈 정통 후속작이다. "엄폐(cover)와 파괴(destruction)"라는 시리즈의 DNA를 정점까지 다듬은 한편, 지중해 전역을 무대로 한 야심찬 'Dynamic Campaign Map'을 들고 나왔다. 실시간 전투의 완성도에서는 "지난 10년 RTS 중 최고"라는 찬사를, 캠페인 실험에서는 "비극적 실패"라는 혹평을 동시에 받은, 평가가 극명하게 갈린 작품이다. 본 분석서는 이 게임이 무엇을 시도했고, 어디서 성공하고 어디서 좌초했는지를 영어권 자료를 바탕으로 심층적으로 다룬다.

---

## 1. 게임 개요

### 기본 정보

| 항목 | 내용 |
|------|------|
| 정식 명칭 | 《Company of Heroes 3》 (약칭 CoH3) |
| 개발사 | Relic Entertainment (캐나다 밴쿠버) |
| 퍼블리셔 | SEGA |
| 장르 | 실시간 전술(Real-Time Tactics)/실시간 전략(RTS) |
| 플랫폼 | PC(Windows) → 이후 PS5, Xbox Series X|S |
| PC 출시일 | 2023년 2월 23일 |
| 콘솔 출시일 | 2023년 5월 30일 (Console Edition) |
| 엔진 | Essence Engine 5 (Relic 자체 엔진) |
| 가격 | 59.99달러 (스탠다드) |
| 배경 | 제2차 세계대전 지중해 전역 (이탈리아·북아프리카) |

### 개발사와 시리즈 계보

Relic Entertainment은 1997년 설립된 캐나다 밴쿠버 소재 스튜디오로, 《Homeworld》(1999), 《Warhammer 40,000: Dawn of War》 시리즈, 그리고 본 시리즈를 통해 "스타크래프트식 자원 폭증·물량전 RTS"와 구별되는 **전술 중심 RTS**의 대표 주자로 자리매김했다. 2013년 THQ 파산 후 SEGA에 인수되어 SEGA 산하 스튜디오가 되었다.

시리즈의 출발점인 《Company of Heroes》(2006)는 출시 당시 메타크리틱 93점을 받으며 "RTS의 패러다임을 바꿨다"는 평가를 받은 명작이다. 분대(squad) 단위 전투, 엄폐 시스템, 파괴 가능한 환경, 측면 기동의 전술성을 결합해 '실시간 전술(RTT)'이라는 하위 장르를 사실상 정립했다. 후속작 《Company of Heroes 2》(2013)는 동부전선을 다뤘으나 트루사이트(TrueSight) 시야 시스템, 동상(凍傷) 메카닉 등 호불호가 갈리는 변경과 출시 후 DLC 정책 논란으로 1편만큼의 호평은 받지 못했다.

### 디렉터/주요 크레딧과 개발 규모

게임 디렉션은 **David Littman**을 중심으로 Terri Douglas, Raj Patel 등이 참여했다. David Littman은 업계 20년 이상 경력에 20여 종의 타이틀을 출시한 베테랑 프로듀서/디렉터로, 본 시리즈의 방향타를 잡기 위해 Relic에 합류했다(출처: IMDb, Relic 공식 자료).

음악은 독일 뮌헨의 게임 음악 전문 스튜디오 **Dynamedion**이 담당했으며, Tilman Sillescu가 리드 작곡가로 참여하고 Henning Nugel, Armin Haas, Alex Röder, Jochen Flach, Matthias Wolf 등으로 구성된 팀이 함께 작업했다(출처: Dynamedion 공식 News).

개발의 가장 큰 특징은 **CoH-Development 커뮤니티 공동개발 프로그램**이다. Relic은 출시보다 1년 이상 앞선 2021년 7월, 게임을 공개하면서 동시에 무료 **Pre-Alpha Preview**를 배포했다. 이는 마케팅용 데모나 베타가 아니라, 개발 초기 단계부터 커뮤니티 피드백을 받아 게임의 형태를 함께 다듬겠다는 의도였다. 이 프로그램은 Amplitude Studios의 **Games2Gether** 플랫폼을 기반으로 운영되었다(출처: Wccftech, NME, History Hit).

### 엔진/기술 스택

CoH3는 Relic의 자체 엔진인 **Essence Engine 5**를 사용한다. 핵심 기술 진보는 "Destruction 2.0"으로 불리는 차세대 3D 파괴 시스템이다. 건물의 개별 타일과 벽돌이 떨어져 나가는 입자 단위 파괴, 지형·차량·구조물까지 모든 요소가 파괴 가능한 환경을 구현했다. 실시간 전투에서 평균 약 150fps를 유지할 만큼 최적화되었다는 보도도 있다(출처: Saving Content 리뷰). 물리 시뮬레이션은 엄폐 시스템과 직결되는데, 폭발로 벽이 무너지면 그 벽이 제공하던 엄폐가 실시간으로 사라지는 식이다.

---

## 2. 게임 설명

### 컨셉과 세계관

《Company of Heroes 3》는 제2차 세계대전의 **지중해 전역(Mediterranean Theatre)**을 무대로 한다. 전작들이 노르망디(서부전선)와 동부전선을 다룬 것과 달리, 본작은 상대적으로 게임에서 덜 다뤄진 **이탈리아 전역과 북아프리카 사막전**을 전면에 내세웠다. Relic은 "지중해는 바람이 휘몰아치는 이탈리아 산악 고개에서 가혹한 북아프리카 사막, 해안 풍경에 이르기까지 막대한 다양성의 공간"이라고 묘사했다.

게임은 크게 **두 개의 캠페인**으로 구성된다.

**1) 이탈리아 캠페인 (Italian Dynamic Campaign)** — 본작의 간판 신기능. 연합군 사령관이 되어 이탈리아 본토를 점령한 추축군을 몰아내는 전역 전체를 지휘한다. 지상·공중·해상 전력을 운용하고 보급선을 건설하며, '샌드박스 스타일'의 전략적 선택을 한다. 나폴리에서 시작해 북상하는 구조다.

**2) 북아프리카 작전 (Operation in North Africa)** — 전통적인 미션 기반 선형 캠페인. **Deutsches Afrikakorps(DAK)**, 즉 에르빈 롬멜 휘하 독일 아프리카 군단을 플레이어가 지휘한다. 토브룩(Tobruk), 엘 알라메인(El Alamein) 등에서 영국군과 격돌하는 역사적 전투를 다룬다.

### 줄거리와 톤 [스포일러 포함]

이탈리아 캠페인은 명확한 단일 서사보다 사령관의 작전적 의사결정에 초점을 맞춘다. 반면 **북아프리카 캠페인의 서사적 선택은 강한 논란을 낳았다**. 이 캠페인은 리비아 벵가지의 유대인 공동체를 비롯한 현지 주민에게 제2차 세계대전이 어떤 영향을 미쳤는지를 리비아 유대인 화자(narrator)의 시점에서 풀어내려 한다. 그런데 플레이어가 조종하는 진영은 **독일군(DAK)**이다.

이 설정은 심각한 **톤의 불일치(whiplash)**를 만들어냈다. 플레이어가 판처(전차)로 영국군 참호를 즐겁게 짓밟는 미션과, 화자의 유대인 이웃들이 SS에 의해 등록되고 색출당하는 이야기가 교차한다. 비평가들은 이를 두고 "롬멜 캠페인은 잊혀질 만큼 평범하고 현실적 근거가 없으며, 북아프리카 전역에 정당한 대우를 하지 못했다"고 지적했다. 화자가 들려주는 유대인 공동체의 비극적 이야기에 "거의 시간과 노력을 들이지 않았다"는 비판도 함께 나왔다(출처: WayTooManyGames, Kotaku).

### 무드/톤/아트 디렉션

Relic은 본작에서 '시네마틱 비전'을 강조했다. 흙먼지가 피어오르는 지중해의 햇살, 무너지는 이탈리아 마을, 사막의 모래폭풍 등 전장의 스펙터클을 강조한 연출이 특징이다. 전작들이 회색빛 동부전선의 음울함이나 노르망디의 진창을 담았다면, 본작은 색채가 한층 다채롭고 따뜻한 지중해 팔레트를 사용한다. 다만 이 톤이 전쟁의 참혹함과 충돌한다는 위 서사 논란과도 연결된다.

### 사운드/음악

Dynamedion이 작곡한 사운드트랙은 지중해 전역의 분위기를 살려 오케스트라 기반의 군사 스코어에 지역색을 가미했다. 다만 일부 커뮤니티에서는 **성우 연기와 억양**에 대한 비판이 제기되었는데, 특히 캠페인 대사의 품질이 몰입을 떨어뜨린다는 지적이 있었다(출처: Steam 커뮤니티 토론). 파괴와 폭발의 사운드 디자인, 분대 단위 음성 콜아웃 등 시리즈 전통의 사운드 연출은 호평받았다.

---

## 3. 핵심 시스템 / 메카닉

### 코어 게임플레이 루프

《Company of Heroes》시리즈의 심장은 **"엄폐와 파괴, 측면 기동"**의 삼위일체다. 본작도 이 루프를 계승·정제했다.

플레이어는 소수의 분대를 운용해 맵의 핵심 자원 지점(영토 포인트, 연료 포인트, 군수품 포인트)을 점령하고, 그 자원으로 추가 병력과 차량을 생산하며 전선을 밀어 올린다. 단순 물량전이 아니라, 각 분대의 **위치 선정**이 승패를 좌우한다.

### 엄폐 시스템 (Cover System)

본작 게임플레이의 정수이자 비평가들이 가장 일관되게 극찬한 요소다. 한 리뷰는 "엄폐 시스템이 절대적으로 환상적이며 설명된 그대로 작동한다. 모든 RTS가 가져야 할 수준의 파괴와 환경 상호작용을 갖췄다"고 평했다.

- **모든 오브젝트가 엄폐를 제공**한다. 돌담, 모래주머니, 차량 잔해, 분화구 등.
- 엄폐는 **녹색(중엄폐, heavy cover)**과 **노란색(경엄폐, light cover)**으로 시각화된다. 녹색은 정면 사격을 크게 흡수하고, 노란색은 부분적으로 흡수한다.
- 엄폐는 **동적(dynamic)**이다. 전투 중 생성되고 파괴된다. XCOM의 엄폐와 유사하되 실시간으로 작동하는 점이 핵심 차별점이다. 폭발로 벽이 무너지면 엄폐도 사라지고, 분화구가 생기면 새 엄폐가 만들어진다.

이로 인해 플레이어는 상대 분대의 엄폐 정면을 피해 **측면(flank)**으로 돌아 사격 효율을 극대화하거나, 박격포·수류탄으로 엄폐 자체를 파괴해 적을 노출시키는 전술적 선택을 끊임없이 하게 된다.

### 파괴 시스템 (Destruction 2.0)

Essence Engine 5의 차세대 파괴는 단순 연출이 아니라 게임플레이에 직결된다. 건물 벽이 입자 단위로 무너지고, 무너진 잔해가 새로운 지형·엄폐가 된다. 전차로 담장을 밀고 들어가 적의 엄폐 라인을 붕괴시키는 등, 환경 자체가 전술 변수로 작동한다.

### Battlegroups (배틀그룹)

전작의 'Command Doctrines'(1편)와 'Commanders'(2편)를 계승한 시스템이다. 멀티플레이와 스커미시에서 핵심 진영을 보강하는 고유 유닛·업그레이드·능력의 트리다.

- 플레이어는 매치 시작 시 **세 개의 배틀그룹 중 하나**를 선택한다.
- 전투 중 누적하는 **커맨드 포인트(Command Points)**로 해당 배틀그룹의 테크 트리를 따라 능력을 해금한다.
- 진영의 기본 군대 위에 특화 색깔을 입히는 방식으로, 같은 진영도 배틀그룹에 따라 운용이 달라진다.

### Tactical Pause (전술적 일시정지)

본작이 새로 도입해 강조한 접근성·전술 기능이다.

- 캠페인 미션, AI 상대 스커미시에서 **언제든 게임을 멈출 수 있다**.
- 일시정지 상태에서 전장을 재평가하고, 실시간으로 내릴 수 있는 모든 명령(이동·사격·능력 사용 등)을 **미리 큐에 쌓아둘 수 있다**.
- 정밀한 다중 명령을 차분히 계획한 뒤 해제하면 한꺼번에 실행된다.

이는 RTS에 입문하는 플레이어나 손이 느린 플레이어에게 진입 장벽을 크게 낮추는 동시에, 고난도 미션에서 정교한 전술 플레이를 가능하게 한다. 단, **실제 사람 상대 멀티플레이에서는 비활성화**된다. AI 상대 커스텀 매치나 캠페인에서만 쓸 수 있다.

### 진영(Factions)

본작은 **4개 진영**으로 출시되었으며, 각 진영이 친숙하면서도 뚜렷한 강점으로 차별화된다.

| 진영 | 성격 | 특징 |
|------|------|------|
| Deutsches Afrikakorps (DAK) | 기동·공격형 | 기갑과 강력한 유닛으로 돌격·측면 기동에 강함 |
| British Forces (영국군) | 방어형 | 진지 방어 중심, 비교적 초보자 친화적 |
| US Forces (미군) | 유연·다재다능 | 다양한 조합과 균형 잡힌 운용 |
| Wehrmacht (독일 국방군) | 정통 독일군 | 강력한 후반 기갑과 정통 전술 |

### 진행 구조: Dynamic Campaign Map

이탈리아 캠페인의 'Dynamic Campaign Map'은 본작 최대의 야심이다. 《Total War》식 턴제 전략 레이어 위에 CoH의 실시간 전술 전투를 얹은 하이브리드 구조다.

- 이탈리아 본토 전체가 헥스/지점 기반의 전략 맵으로 펼쳐진다.
- 플레이어는 사령관으로서 지상·공중·해상 전력을 배치하고 보급선을 건설하며 전역의 큰 그림을 지휘한다.
- 영토를 두고 충돌이 발생하면 익숙한 CoH 실시간 전술 전투로 전환되거나, 자동 해결(auto-resolve)을 선택할 수 있다.
- 어느 도시를 먼저 칠지, 어디에 자원을 투입할지 등 **'샌드박스식' 전략적 선택**이 핵심이다.

### 멀티플레이/라이브 운영

멀티플레이는 1v1부터 4v4까지의 대전, 협동 vs AI 모드를 지원한다. 배틀그룹 메타와 진영 밸런스가 핵심이다. 다만 **출시 시점에는 관전(spectator)과 리플레이 기능이 없었고**, 이는 경쟁 RTS로서의 잠재력에 심각한 제약으로 지적되었다(출처: Jump Dash Roll, WayTooManyGames). 이후 1.x 패치를 통해 점진적으로 보강되었다.

### 난이도/접근성

Tactical Pause가 접근성의 핵심 축이다. 그 외에 난이도 단계 조절, 'RTS Boot Camp' 튜토리얼 등 입문자 지원이 마련되었다. 그럼에도 본작은 여전히 "심약한 사람이나 즉각적 만족을 원하는 사람을 위한 게임은 아니다"라는 평을 받는, 깊은 학습 곡선의 하드코어 RTS다.

---

## 4. 평가

### 메타크리틱/오픈크리틱 점수

| 플랫폼/집계 | 점수 | 비고 |
|-------------|------|------|
| Metacritic (PC) | "Generally Favorable" (대체로 호평) | |
| Metacritic (Xbox Series X) | "Generally Favorable" | |
| Metacritic (PS5) | "Mixed or Average" (혼재/평균) | 콘솔판 평가 하락 |
| OpenCritic | 78점, 'Strong', 77명 비평가, 추천율 77% | (집계 시점에 따라 변동) |

출시 직후 일부 집계에서는 18개 리뷰 기준 평균 81점·추천율 88%로 더 높게 잡히기도 했다(출처: OpenCritic 초기 집계, Saving Content). 시간이 지나며 더 많은 리뷰가 반영되면서 78점대로 수렴했다.

### 주요 평론 인용

- **PC Gamer**: "주력 캠페인이 빛나지 못할 때조차 빛나는 장관(spectacular)의 RTS"라고 평하면서도, 이탈리아 캠페인은 "근본적으로 망가졌다(fundamentally broken)"고 직격했다. AI가 공격성을 결여하고 있다는 점이 핵심 문제로 지목되었다.
- **종합 평**: "RTS로서 《Company of Heroes 3》는 최정상급이지만, Relic의 실험적 캠페인은 비극적이게도 다소 실패작(a bit of a dud)이다."
- 한편 "지난 10년 최고의 RTS일 것"이라며 "풍부한 싱글플레이 콘텐츠와 장기 멀티플레이를 위한 견고한 토대"를 갖췄다는 호평도 나왔다.
- **IGN**: 커뮤니티 토론에 따르면 6/10점으로, 상대적으로 박한 평가를 매겼다(출처: Steam 커뮤니티/NeoGAF 리뷰 스레드).
- **Push Square (PS5판)**: "베테랑 RTS 시리즈가 PS5에서 피로스의 승리(Pyrrhic Victory)를 누린다"는 제목으로, 콘솔 이식의 한계를 지적했다.

### 평론의 핵심 패턴

거의 모든 리뷰가 **동일한 양분 구조**를 보였다. 즉, **실시간 전술 전투(엄폐·파괴·측면 기동·멀티플레이 토대)는 시리즈 최고 수준**으로 호평하는 반면, **간판 신기능인 이탈리아 Dynamic Campaign Map은 실망**으로 평가했다. 전략 레이어의 AI가 소극적이고, 전략·전술 두 레이어의 결합이 매끄럽지 않으며, 자동 해결의 균형이 어색하다는 지적이 반복되었다.

### 상업 지표

- **소유자 수**: SteamSpy 추정 100만~200만 명.
- **동시접속 최고치**: Steam 기준 역대 최고 약 **36,629명**(출시 직후 추정). 이후 통상 수천 명대를 유지하며, 2025년 3월에는 12,035명 피크를 기록하기도 했다(출처: SteamDB, Steambase, SteamSpy).
- **가격**: 59.99달러.
- **유저 평점**: Steam 약 38,000여 리뷰 기준 'Mixed(복합적)' — 출시 상태에 대한 불만(특히 이탈리아 캠페인, 멀티 편의기능 부재, 일부 버그·발렌스)이 반영된 결과다. 단, 이후 다수의 패치로 'Mostly Positive' 구간으로 개선되었다는 평가도 나온다.

SEGA의 공식 판매량 수치는 별도로 공개되지 않았으나, SteamSpy 추정치와 동접 데이터로 미루어 100만 본 이상은 판매된 것으로 보인다.

### 수상/노미네이트

본작은 전작 1편 같은 GOTY급 영예를 받지는 못했다. 평가가 양분된 데다 출시 상태의 미완성도가 발목을 잡아, 메이저 시상식에서 두드러진 수상 기록은 남기지 못했다.

---

## 5. 성공 요인 분석

### 디자인 측면: 시리즈 코어의 정점

CoH3가 비평적으로 인정받은 가장 큰 이유는 **"엄폐+파괴" 코어 메카닉을 시리즈 역사상 가장 정교하게 다듬었기 때문**이다. Destruction 2.0의 입자 단위 파괴, 동적 엄폐, 4개 진영의 뚜렷한 정체성, 배틀그룹의 빌드 다양성은 RTS 장르에서 독보적인 전술 깊이를 제공한다. "모든 RTS가 가져야 할 수준의 환경 상호작용"이라는 평가가 이를 압축한다.

### 시장 환경/타이밍

2010년대 후반~2020년대 초반은 전통적 RTS 장르가 침체기를 겪던 시기였다. 《StarCraft II》이후 대형 신작 RTS가 드물었고, 《Age of Empires IV》(2021)가 장르 부활의 신호탄을 쏘아 올린 상황이었다. **RTS 팬덤이 신작에 굶주려 있던 타이밍**에, 검증된 IP의 정통 후속작이 나온 것은 강력한 호재였다. 특히 본작은 멀티플레이 토대가 탄탄해 "지난 10년 최고의 RTS"라는 평가를 끌어낼 만한 빈 자리를 채웠다.

### 차별화된 무대 선택

서부전선과 동부전선을 이미 다룬 시리즈가 **상대적으로 덜 탐구된 지중해 전역**을 택한 것은 신선함을 더했다. 사막전과 이탈리아 산악·해안전은 노르망디의 진창이나 동부전선의 설원과는 다른 시각적·전술적 변주를 제공했다.

### 개발 방법론: 커뮤니티 공동개발

**CoH-Development 프로그램**은 마케팅과 품질 양면에서 의미 있는 시도였다. 출시 1년 이상 전부터 Pre-Alpha Preview를 풀고 Games2Gether 플랫폼으로 피드백을 수렴함으로써, 핵심 팬층의 충성도를 출시 전에 확보하고 코어 게임플레이를 검증할 수 있었다. 이는 RTS처럼 밸런스가 생명인 장르에서 특히 유효한 전략이었으며, 출시된 전투 메카닉의 높은 완성도는 이 과정의 산물로 볼 수 있다.

### IP/커뮤니티 효과

《Company of Heroes》라는 이름값 자체가 거대한 자산이다. 1편이 RTT 장르를 정립한 명작이라는 역사적 평판, 그리고 7년의 공백이 만들어낸 기대감이 출시 동접 3.6만 명이라는 강력한 초기 화력으로 이어졌다.

---

## 6. 비평적 시각 / 한계 / 논란

### 이탈리아 캠페인의 구조적 실패

본작의 가장 큰 약점은 역설적으로 가장 야심찬 기능이었다. **Dynamic Campaign Map은 비전은 매력적이었으나 실행이 따라가지 못했다.** PC Gamer는 이를 "근본적으로 망가졌다"고까지 표현했다. 핵심 문제들은 다음과 같다.

- **AI의 소극성**: 전략 레이어의 적 AI가 공격성을 결여해, 플레이어가 압박을 거의 느끼지 못한 채 진행하게 된다. 긴장감이 사라진다.
- **두 레이어의 봉합 부실**: 《Total War》식 전략 맵과 CoH식 전술 전투의 결합이 매끄럽지 않다. 자동 해결의 균형, 보급·이동의 직관성, 전략적 의사결정의 무게감이 기대에 미치지 못했다.
- **반복성**: 샌드박스를 표방했으나 실제로는 전투가 반복적으로 느껴지고, 전략적 선택의 결과가 충분히 의미 있게 다가오지 않는다는 지적이 많았다.

### 북아프리카 캠페인의 톤 논란

위에서 다룬 대로, **독일 DAK를 조종하면서 유대인 화자의 비극을 듣는 서사 구조**는 톤의 충돌을 일으켰다. 비평가들은 롬멜 캠페인을 "잊혀질 만큼 평범하고 현실적 근거가 없다"고 평했고, 현지 유대인 공동체의 이야기를 다루겠다는 선의가 피상적 처리에 그쳤다고 비판했다. 미션들도 이탈리아 캠페인의 명장면급 전투에 비해 인색하고 기억에 남지 않는다는 평가를 받았다.

### 멀티플레이 편의 기능 부재

출시 시점에 **관전·리플레이 기능이 없었다.** 경쟁 RTS의 생명선인 이 기능들의 부재는 e스포츠/경쟁 씬 형성에 치명적 제약으로 작용했다. 또한 일부 리뷰는 진영별 유닛 다양성 부족과 밸런스 문제로 각 진영이 특정 플레이스타일에 갇히는 "egregious(심각한)" 밸런스 이슈를 지적하며, "멀티플레이 씬이 이미 생명 유지 장치에 의존하는 듯 보인다"고까지 평했다(출처: Sportskeeda, WayTooManyGames).

### 콘솔판의 한계

2023년 5월 콘솔 출시는 시리즈 최초의 가정용 게임기 진출이라는 의미가 있었으나, PS5판은 메타크리틱 "Mixed" 평가를 받았다. 정밀한 분대 마이크로 컨트롤을 패드로 구현하는 것의 본질적 어려움, 그리고 콘솔판이 인게임 스토어·챌린지·모딩 지원을 결여한 채 출시된 점이 한계로 작용했다.

### 출시 상태(Day-1) 미완성도

전반적으로 본작은 "장기적으로 훌륭해질 견고한 토대를 갖췄으나, 출시 당시에는 미완성"이라는 인상을 남겼다. 양분된 평론, Steam의 'Mixed' 유저 평가, 캠페인의 미흡함, 멀티 편의기능 부재가 합쳐져 "1편의 영광을 재현하지 못했다"는 아쉬움이 따라붙었다.

---

## 7. 영향과 유산

### 장르적 의미

《Company of Heroes 3》는 침체된 RTS 장르에서 **"전술 깊이의 정점"을 다시 한번 입증한 작품**으로 남는다. 엄폐와 파괴를 결합한 RTT 디자인은 후속 RTS·전술 게임에 계속 영향을 미치는 레퍼런스다. 동시에, **간판 신기능(Dynamic Campaign Map)의 실패**는 "전략 레이어와 전술 레이어를 결합하는 하이브리드 캠페인은 비전만으로 부족하며, AI와 봉합의 완성도가 결정적"이라는 교훈을 장르에 남겼다.

### 라이브 운영과 장기 개선

Relic은 출시 후 적극적인 업데이트 로드맵을 가동했다. 2023년 하반기 'Brass Leopard' 등 콘텐츠 업데이트로 신규 맵, 오디오 개선, 게임플레이 튜닝을 더했고, PC와 콘솔을 별도 트랙으로 관리하며 멀티 편의기능과 밸런스를 점진적으로 보강했다. 이 덕분에 출시 후 수년에 걸쳐 평가가 개선되었고, 2025년 시점에는 "2년이 지난 지금은 살 만한 가치가 있는가"를 긍정적으로 재평가하는 리뷰들이 등장했다(출처: Strategy and Wargaming, 2025).

### Relic의 독립과 IP의 미래

본작의 유산은 개발사 자체의 격변과도 얽혀 있다. **2024년 3월, SEGA는 Relic Entertainment를 매각**했다. SEGA는 유럽·영국 팀(Creative Assembly, Sega Hardlight 포함)에서 총 **240명을 감원**하는 구조조정의 일환으로 Relic을 분리했고, Relic은 투자사 **Emona Capital**의 지원을 받아 비공개 금액에 자사를 되사들여 **독립 스튜디오**가 되었다. 그러나 독립 직후 다시 41명을 추가 감원하는 등 진통을 겪었다(출처: Variety, GameSpot, GamesBeat, Game Developer).

독립 후에도 Relic은 《Company of Heroes 3》를 계속 지원하겠다고 약속했고, 2024년 4월 1.6 업데이트를 예고했다. 즉 CoH3는 대형 퍼블리셔의 우산 아래에서 출시되었으나, 그 IP를 가진 스튜디오가 독립 후에도 살아남아 운영을 이어가는, 변동성 큰 게임 산업의 단면을 보여주는 사례가 되었다.

### 문화적·산업적 의미

CoH3는 **"평가가 양분된 야심작"의 전형적 표본**으로 종종 인용된다. 코어 시스템의 완성도와 출시 시점의 미완성, 비전과 실행의 간극을 동시에 보여준 작품이기 때문이다. 또한 **커뮤니티 공동개발(CoH-Development)** 모델은 RTS처럼 밸런스 민감도가 높은 장르에서 출시 전 핵심 메카닉을 검증하는 방법론으로서 의미 있는 선례를 남겼다 — 비록 그 방법론이 싱글플레이 캠페인의 구조적 결함까지 막아주지는 못했지만.

---

## 8. 부록

### 핵심 통계 표

| 지표 | 값 | 출처 |
|------|-----|------|
| PC 출시일 | 2023-02-23 | Wikipedia, Steam |
| 콘솔(PS5/Xbox) 출시일 | 2023-05-30 | companyofheroes.com FAQ |
| 메타크리틱 (PC) | Generally Favorable | Metacritic |
| 메타크리틱 (PS5) | Mixed or Average | Metacritic |
| OpenCritic | 78 (Strong), 추천율 77% | OpenCritic |
| Steam 역대 최고 동접 | 약 36,629명 | SteamDB/Steambase |
| Steam 추정 소유자 | 100만~200만 | SteamSpy |
| Steam 유저 평가 | Mixed (약 38,000 리뷰) | SteamSpy/Steam |
| 가격 | 59.99달러 | Steam |
| 진영 수 | 4개 (DAK, 영국, 미군, Wehrmacht) | 공식 |
| 엔진 | Essence Engine 5 / Destruction 2.0 | Saving Content |

### 주요 진영 요약

| 진영 | 핵심 플레이스타일 |
|------|------------------|
| Deutsches Afrikakorps (DAK) | 고기동·공격형 기갑 |
| British Forces | 방어 지향, 입문자 친화 |
| US Forces | 다재다능·균형형 |
| Wehrmacht | 정통 독일군, 후반 기갑 강세 |

### 핵심 인터뷰/자료

- Relic 공식 — CoH-Development / Pre-Alpha Preview 프로그램 안내
- History Hit — "How a Cinematic Vision Inspires the Spectacle of Company of Heroes 3" (아트 디렉션·시네마틱 비전 인터뷰)
- Dynamedion 공식 News — "Composing Company of Heroes 3" (음악 제작)
- companyofheroes.com — Console Edition FAQ / Launch Content & Beyond 로드맵

### 참고 자료 목록 (영어권 매체 중심)

- [Metacritic — Company of Heroes 3](https://www.metacritic.com/game/company-of-heroes-3/)
- [OpenCritic — Company of Heroes 3](https://opencritic.com/game/14319/company-of-heroes-3)
- [PC Gamer — Company of Heroes 3 review](https://www.pcgamer.com/company-of-heroes-3-review/)
- [Saving Content — Company of Heroes 3 Review](https://www.savingcontent.com/2023/02/20/company-of-heroes-3-review/)
- [WayTooManyGames — Review: Company of Heroes 3](https://waytoomany.games/2023/03/06/review-company-of-heroes-3/)
- [Kotaku — Company of Heroes 3: The Kotaku Review](https://kotaku.com/company-of-heroes-3-the-kotaku-review-1850110787)
- [Push Square — Company of Heroes 3 (PS5) Review](https://www.pushsquare.com/reviews/ps5/company-of-heroes-3)
- [Jump Dash Roll — Console Edition Review](https://www.jumpdashroll.com/article/company-of-heroes-3-console-edition-review)
- [Strategy and Wargaming — Is It Worth It Two Years Later? (2025)](https://strategyandwargaming.com/2025/05/17/company-of-heroes-3-review-is-it-worth-two-years-later/)
- [MMORPG.com — Strategy Session: Dynamic Map Preview](https://www.mmorpg.com/previews/strategy-session-company-of-heroes-3s-dynamic-map-is-going-to-keep-me-coming-back-for-more-2000126768)
- [Wccftech — Company of Heroes 3 Announced, Pre-Alpha Preview](https://wccftech.com/company-of-heroes-3-announced-preview-playable-now/)
- [Dynamedion — Composing Company of Heroes 3](https://dynamedion.com/news/company-of-heroes-3/)
- [companyofheroes.com — Console Edition FAQ](https://www.companyofheroes.com/en/post/company-of-heroes-3-console-edition-faq)
- [Variety — Sega to Sell Relic Entertainment; Layoffs](https://variety.com/2024/gaming/news/sega-relic-entertainment-sale-layoffs-240-employees-1235954787/)
- [GameSpot — Relic Suffers Layoffs After Going Independent](https://www.gamespot.com/articles/company-of-heroes-dev-relic-suffers-layoffs-after-going-independent-from-sega/1100-6522436/)
- [SteamDB — Company of Heroes 3 Charts](https://steamdb.info/app/1677280/charts/)
- [SteamSpy — Company of Heroes 3](https://steamspy.com/app/1677280)
- [Wikipedia — Company of Heroes 3](https://en.wikipedia.org/wiki/Company_of_Heroes_3)

---

*본 분석서는 영어권 매체 리뷰·집계 사이트·개발사 공식 자료·산업 보도를 종합해 작성되었다. 모든 판매·동접 수치는 출처를 명시했으며, 추정치는 본문에 추정임을 밝혔다.*
