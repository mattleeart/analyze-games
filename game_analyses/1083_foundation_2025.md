# 《Foundation》 (2025) 심층 분석

> 그리드 없는(gridless) 유기적 중세 도시 건설 시뮬레이션. 6년의 얼리 액세스를 거쳐 2025년 1월 31일 정식 출시. 캐나다 퀘벡시티의 소규모 독립 스튜디오 Polymorph Games가 자체 엔진 Hurricane 위에서 만들어 낸, "타일에 갇히지 않는 도시"라는 한 가지 아이디어를 끝까지 밀어붙인 결과물.

---

## 1. 게임 개요

### 개발사·퍼블리셔·출시 정보

《Foundation》은 캐나다 퀘벡시티(Quebec City)에 본사를 둔 독립 스튜디오 **Polymorph Games**가 개발하고 자체 퍼블리싱한 중세 도시 건설 시뮬레이션이다. Polymorph Games는 2016년 2월, 두 명의 베테랑 게임 개발자가 설립한 회사로, 처음부터 《Foundation》이라는 단 하나의 프로젝트에 회사의 명운을 걸어 온 사실상의 "단일 타이틀 스튜디오"다.

출시 일정은 다음과 같이 길고 굴곡진 여정을 거쳤다.

- **2018년**: Kickstarter 크라우드펀딩 캠페인 진행 및 오픈 알파(open alpha) 공개
- **2019년 2월 1일**: Steam 얼리 액세스(Early Access) 출시
- **2025년 1월 31일**: 정식 1.0 출시 (Windows 단독)

당초 Polymorph Games는 약 1년 정도의 얼리 액세스를 계획했으나, 실제로는 **6년**에 가까운 기간을 거쳐 정식 출시에 도달했다. 이 "6년의 얼리 액세스"라는 사실 자체가 이 게임을 이해하는 핵심 열쇠이며, 본 분석서 곳곳에서 반복적으로 등장하는 주제다. 정식 출시 발표문에서 개발팀은 다음과 같이 회고했다.

> "After 6 years of new features, bug fixes and improving the game, with the help of your feedback, we are proud to finally wrap up Foundation's incredible journey in Early Access!" (6년에 걸친 신규 기능, 버그 수정, 그리고 여러분의 피드백에 힘입은 개선 끝에, 마침내 《Foundation》의 놀라운 얼리 액세스 여정을 마무리하게 되어 자랑스럽습니다.)

장르는 **중세 도시 건설 시뮬레이션(medieval city builder)**이며, 흔히 같은 계보로 묶이는 《Banished》, 《Manor Lords》, 《Anno》 시리즈와 같은 진열대에 놓인다. 다만 후술하듯 생존(survival) 압박이나 전투 중심 설계와는 거리를 두고, "여유롭고(laidback) 표현력 있는(expressive) 도시 짓기"를 전면에 내세운다는 점에서 차별화된다.

### 엔진·기술 스택

《Foundation》의 가장 큰 기술적 자부심은 **자체 개발 엔진 Hurricane**이다. 상용 엔진(Unity, Unreal 등)을 쓰지 않고 인하우스 엔진을 구축한 결정은 소규모 스튜디오로서는 대담한 선택이었으나, 이 게임의 정체성과 직결되는 두 가지 요구사항 때문에 불가피했다.

1. **그리드 없는(gridless) 건설**: 건물을 고정된 타일에 스냅(snap)시키지 않고, 자유 회전·자유 배치하며 주민들이 알아서 최적 경로를 찾아 다니게 하려면, 일반적인 타일 기반 시뮬레이션과는 근본적으로 다른 공간·경로(pathfinding) 처리 구조가 필요했다.
2. **수천 명 단위 주민 시뮬레이션**: Hurricane 엔진은 "수천 명의 움직이는 주민과 복잡한 도시 레이아웃"을 부드럽게 처리하도록 설계됐다. 대도시로 커져도 각 주민이 독립적으로 환경과 상호작용하며 움직이는 것이 핵심 목표였다.

또한 Hurricane 엔진은 **풀 모드 지원(full mod support)**을 염두에 두고 설계됐다. 도시 건설 장르에서 모드 커뮤니티가 게임 수명에 결정적이라는 점을 고려한 선택이다.

### 개발 규모·크레딧

Polymorph Games는 끝까지 수십 명 규모를 넘지 않는 소규모 스튜디오였다. 핵심 크레딧 중 특기할 만한 것은 **사운드트랙**으로, 100분이 넘는 오리지널 음악을 **Audinity**가 작곡했다. Audinity 팀은 《Crusader Kings II》, 《Europa Universalis IV》 등 Paradox의 역사 전략 타이틀 사운드 작업 경험을 보유한 팀으로, 중세 도시 빌더라는 장르의 무드에 잘 맞는 선택이었다.

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 한 문장의 컨셉

《Foundation》은 **"그리드가 없는, 유기적으로 뻗어 나가는 중세 도시 건설 시뮬레이션으로, 유기적 발전·모뉴먼트(monument) 건설·자원 관리에 무게를 둔다"**라고 요약할 수 있다. 다른 도시 빌더가 "타일 위에 효율적인 격자 도시를 짜 맞추는" 퍼즐에 가깝다면, 《Foundation》은 "땅의 생김새를 따라 자연스럽게 자라나는 마을을 빚어내는" 조형(造形)에 가깝다.

### 세계관·시대 배경

배경은 중세 유럽, 더 구체적으로는 **프랑스의 앙시앵 레짐(Ancien Régime, 구체제)에서 영감을 받은 신분제 사회**다. 게임 속 사회는 세 개의 신분(estate)으로 나뉜다.

- **노동(Labour)**: 평민·생산자 계층. 승급(promotion)과 과세(taxation)를 중시한다.
- **성직(Clergy)**: 교회·수도원으로 대표되는 종교 계층. 와인·약초 같은 사치 자원의 교역에 능하다.
- **왕국(Kingdom)**: 영주·군대로 대표되는 봉건 권력 계층. 왕을 위해 병력을 보내 왕국을 돕는다.

플레이어는 한 영주(lord)의 입장에서 황무지에 마을을 세우고, 주민을 끌어들이고, 생산 사슬을 구축하며, 이 세 신분의 비위를 맞추고 그들의 "광휘(Splendour)"를 높여 마을을 영지(estate)로 성장시킨다. 흥미롭게도 이 신분제 설계는 단순한 플레이버가 아니라 게임의 진행(progression) 구조 그 자체를 이룬다(3장 참조). 학술 영역에서도 주목받아, 윈체스터 대학(University of Winchester)의 중세 미디어 학술 행사 발표 자료("A Question of Class? The Three Estates as mechanic in Foundation")에서 《Foundation》의 삼부회(three estates) 메커니즘이 다뤄지기도 했다.

### 줄거리와 톤

《Foundation》에는 전통적인 의미의 서사(스토리 캠페인)는 없다. 대신 플레이어가 백지에서 마을을 키워 가는 **샌드박스형 경험**이 줄거리를 대신한다. 톤은 한마디로 **여유롭고 아늑한(cozy/laidback)** 쪽이다. 같은 계보의 《Banished》가 혹독한 겨울·기근·인구 붕괴로 플레이어를 압박하고, 《Manor Lords》가 사실적 전투와 영토 분쟁을 끌어들이는 것과 달리, 《Foundation》은 다음과 같은 위협 요소를 의도적으로 배제한다.

- 가혹한 겨울 없음
- 가뭄·홍수 없음
- 도적(bandit)·습격 없음

즉, 실패와 생존의 긴장보다 **창조와 표현의 즐거움**에 무게를 둔다. 리뷰어들이 입을 모아 "Bellwright나 (먼 조상 격인) Banished보다 훨씬 느긋하다(far more chill)"고 평한 이유다.

### 아트 디렉션·무드

비주얼은 사실주의를 끝까지 밀어붙인 《Manor Lords》와 달리 **약간 만화적이고(comics feel) 따뜻한** 결을 갖는다. 중세 건축과 도시계획(urbanism)을 충실히 반영하되, 플레이어가 "그 시대의 도시를 자신이 상상한 대로, 혹은 실제 존재했던 모습대로" 재현할 수 있게 하는 것이 비전이었다. 그리드가 없는 덕분에 완성된 도시는 스프레드시트로 설계한 듯한 격자가 아니라 **손으로 빚은 듯한(handmade) 유기적 실루엣**을 띤다. 굽이치는 길, 자연스러운 주거 군집, 지형을 따라 흐르는 레이아웃이 이 게임 스크린샷 특유의 미감을 만든다.

### 사운드·음악

앞서 언급했듯 사운드트랙은 **Audinity**가 작곡한 100분 이상의 오리지널 음악으로 구성된다. 류트와 현악, 합창 등을 활용한 중세풍 분위기의 음악은 게임의 아늑한 톤을 강화하는 핵심 요소다. 마을이 작은 정착지에서 번화한 도시로 성장하는 과정을 정서적으로 뒷받침하며, 《Crusader Kings II》·《Europa Universalis IV》 계열의 역사 전략 사운드 문법을 도시 빌더에 이식했다는 점에서 장르 팬에게 친숙하게 다가간다.

---

## 3. 핵심 시스템 / 메카닉

이 장이 《Foundation》을 다른 도시 빌더와 구별 짓는 본질이다. 가장 자세하게 다룬다.

### 3.1 코어 게임플레이 루프 — 그리드 없는 건설

《Foundation》의 모먼트-투-모먼트 경험은 **"구역을 칠하고(paint), 건물을 자유롭게 놓고, 주민이 알아서 길을 낸다"**는 한 문장으로 압축된다.

대부분의 도시 빌더가 고정된 타일 격자 위에 건물을 스냅시키는 것과 달리, 《Foundation》은 건물을 **자유롭게 회전·배치(rotate and place wherever you want)**할 수 있게 한다. 주거·농업·산업 등 용도별로 **랜드스케이프 페인팅(landscape painting)**으로 구역을 지정하면, 주민들이 그 안에서 집과 작업장과 농지를 스스로 적절히 배치한다. 그 결과 플레이어가 "어디에 무엇을 둘지"를 미시적으로 통제하지 않아도, 마을은 마치 실제 중세 정착지처럼 굽이치는 길과 자연스러운 군집을 형성하며 자라난다.

이 시스템의 기술적 심장은 Hurricane 엔진의 **경로 탐색(pathfinding)**이다. 타일이 없으므로 주민들은 매 순간 목적지까지의 최적 경로를 동적으로 계산하고, 그 결과로 길이 닳아 생겨난다(자연 발생적 path 생성). "건물을 어디든 놓으면 주민이 알아서 가는 방법을 찾아낸다(your villagers just figure out the best way to get there)"는 것이 핵심 판매 포인트다.

### 3.2 자원 사슬과 생산 경제

경제의 토대는 **자원 사슬(production chain)**이다.

- **채집(Gatherer) 건물**: 농장을 포함한 기초 자원 추출 시설. 1차 원료(밀, 목재, 석재 등)를 확보한다.
- **정제·가공**: 그 외 거의 모든 재화는 기초 자원을 정제하거나 가공해 만든다. 예컨대 《Manor Lords》와 유사하게 "밀 수확 → 제분(밀가루) → 제빵(빵)" 같은 다단계 사슬, 목재·석재 보급선 관리 등이 핵심이다.
- 게임이 진행될수록 더 고급 건물을 짓고 주민의 욕구를 충족하려면 점점 더 긴 생산 사슬을 구성해야 한다.

자원의 분배(distribution)는 크게 **시장(market)**과 **창고(warehouse)** 두 축으로 이루어진다. 주민은 시장에서 식량과 재화를 "구매"하므로, 시장 접근성이 마을 건강의 핵심 변수다.

### 3.3 경제·세금·교역

수입원은 세 갈래다.

1. **과세(taxation)**: 1.0 정식 출시에서 세금 징수가 **주요 수입원**으로 재설계됐다. "누가 먼저 올바른 건물을 지어 올바른 자원을 생산하고, 가장 먼저 세무소(Tax Office)를 세우느냐"의 경쟁이 초반 게임의 핵심 동선이 됐다.
2. **교역(trade)**: 이웃 도시(neighboring cities)와 교역로(trade route)를 열어, 아직 자체 생산하지 못하는 품목(예: 도구)을 사 오고, 자체 생산한 품목을 팔아 금화 수입을 얻는다.
3. **군사 원정(military)**: 1.0의 새 군사 시스템에서 **부대(Company)**를 편성해 해외로 파견하면, 귀중한 자원을 가지고 돌아온다. 즉 전투를 직접 묘사하지 않으면서도 군사 요소를 "자원 획득 루프"로 추상화했다.

### 3.4 진행 구조 — 세 신분(Estate)과 진행 트리

《Foundation》의 진행(progression)은 장르 내에서 가장 독창적인 부분이다. **진행 트리(Progression Tree)**는 네 갈래의 경로로 구성된다.

- **공통 경로(Common Path)**
- **노동(Labour)**
- **왕국(Kingdom)**
- **성직(Clergy)**

각 경로는 다섯 단계(tier)로 나뉘고, 각 단계 안에 해금 가능한 기술·능력이 들어 있다. 작동 원리는 다음과 같다.

- **단계 해금 조건**: 공통 경로는 **번영도(Prosperity)**가, 나머지 세 경로는 **광휘(Splendour)**가 일정 수준에 도달해야 다음 단계가 열린다.
- **기술 구매 비용**: 공통 경로는 **금화(Gold Coins)**로, 나머지 경로는 **영향력(Influence)**으로 기술을 해금한다.
- **광휘 획득**: 광휘는 신분 유형에 맞는 모뉴먼트를 짓고 장식해 얻는다. 마노어 하우스(Manor House)·선술집(Tavern)·시장(Market) 같은 시민 건물은 **노동 광휘**, 교회·수도원 같은 종교 건물은 **성직 광휘**, 성채(Keep) 같은 군사 건물은 **왕국 광휘**에 기여한다.

각 신분 경로는 뚜렷한 성격을 갖는다. **노동**은 주민 승급과 과세, **왕국**은 병사로 왕국을 돕는 것, **성직**은 와인·약초 같은 사치 자원 교역에 강점을 둔다. 플레이어는 한 신분에 특화할 수도, 셋을 모두 균형 있게 키울 수도 있다. 1.0에서는 진행 시스템이 개편되어 **영지 간 트레이드오프(estate tradeoff)가 제거**되어, 한 영지에 집중하든 모두를 만족시키든 자신이 택한 포부(aspiration)에 따라 플레이할 수 있게 됐다.

이 신분제와 맞물리는 것이 **행정관(Administrator)과 만다트(Mandate)** 시스템이다. 신분마다 한 종류의 행정관이 있다 — **베일리프(Bailiff, 노동)**, **수도원 사절(Monastic Emissary, 성직)**, **왕실 정신(Royal Courtier, 왕국)**. 각 유형은 게임당 한 명만 임명할 수 있다. 행정관은 만다트(특수 지령)를 발동하는데, 예컨대 세무소 기능이 노동 경로 전용이 되면서 추가된 **부역 징발(Levy)** 만다트 등이 있다.

### 3.5 모뉴먼트 디자인 — 노드 기반 자유 건축

《Foundation》의 시그니처 시스템은 단연 **모뉴먼트 디자인(Monument Design)**이다. 플레이어는 애비(Abbey, 대수도원)·교회·영주 저택·성채 등 거대 건축물을 **독자적인 노드 기반(node-based) 도구**로 자유롭게(free-form) 설계한다. 정해진 외관을 배치하는 것이 아니라, 벽·탑·아치·지붕 등의 부품(part)을 조합해 자신만의 건축물을 빚어내는 일종의 "중세 건축 미니 게임"이다.

1.0에서 이 경험은 대대적으로 개편됐다.

- **부품 교체(replace parts)** 및 **모뉴먼트 전체 이동(move an entire monument)** 기능 추가
- 전면적인 UI 개편
- 모뉴먼트 하위 건물 메뉴에 **검색창** 추가 — 카테고리·키워드·연관어로 원하는 부품을 빠르게 찾도록

이 시스템은 게임의 "표현력"을 상징한다. 동일한 자원으로 누군가는 소박한 예배당을, 누군가는 압도적인 대성당을 짓는다. 광휘 시스템과 직접 연결되므로 미학적 만족과 기능적 진행이 한 몸으로 묶인다.

### 3.6 주민 시뮬레이션과 비주얼 피드백

주민(villager)은 단순한 일꾼 토큰이 아니라 **생활하는 시민**으로 시뮬레이션된다 — 일하고, 쉬고, 교역하고, 기도하고, 잔치를 벌인다(live, work, relax, trade, pray and party). 1.0에서는 주민 표현이 한층 강화됐다.

- **복장 시스템(outfit system)**: 주민의 모든 의상을 전면 개편해 더 다양하고 풍부한 색감을 입혔다. 모든 직업이 고유하고 알아보기 쉬운 외형을 갖게 되어, 시각만으로 누가 무슨 일을 하는지 파악된다. 수확 축제(Harvest Festival) 같은 특정 행사에는 주민이 옷을 갈아입는 식의 이벤트 반응도 추가됐다.
- **노동 효율 개선**: 주민의 전체 작업 시간에서 **이동 시간(travel time)을 제거**해, 작업 시간을 더 효과적으로 쓰도록 바꿨다.

### 3.7 1.0에서 더해진 주요 시스템·콘텐츠

정식 출시는 단순한 "버그 수정 + 발표"가 아니라, 사실상 대규모 콘텐츠 업데이트였다. 주요 추가·개편 사항은 다음과 같다.

- **문장(Heraldry) 시스템**: 새로운 **문장 편집기(Coat of Arms editor)**로 마을 고유의 문장·깃발을 제작·커스터마이즈.
- **성채(Castle) 모뉴먼트**: 모뉴먼트 디자인 방식으로 짓는 완전히 새로운 성채. 새 군사 시스템과 연동.
- **주거 계층 개편**: 더 높은 밀도·품질의 주거 계층 추가로 도시 커스터마이즈 폭 확대. 중밀도 주거는 순찰(patrol) 커버리지를 요구.
- **인프라 확장**: 포장도로, 건설 가능한 성벽, 망루(watchtower), 경비 배치, 확장 가능한 건물(나무꾼 캠프·창고 등).
- **UI/UX 전면 개편**: 새 메인 메뉴, 진행 트리, 개선된 툴팁, 마을 정보를 담는 책(Book) 강화.
- **룰셋(rulesets)**: 난이도를 조절할 수 있는 커스텀 룰셋.

### 3.8 난이도·접근성

《Foundation》은 생존 압박을 배제한 설계 덕에 **입문자 친화적(beginner-friendly)**이라는 평을 받는다. IGN Deutschland가 "아늑하고 입문자 친화적인 도시 빌더"라 표현했듯, 실패의 공포 없이 천천히 도시를 키우는 경험을 제공한다. 동시에 룰셋으로 난이도를 조절할 수 있어, 더 빡빡한 경제 운영을 원하는 플레이어도 자기 입맛에 맞출 수 있다. 다만 후술하듯 "기본 설정에서의 후반부 도전 부재"는 양날의 검으로 지적된다.

### 3.9 라이브 운영·사후 지원

정식 출시 후에도 Polymorph Games는 지원을 이어 갔다. 2025년 11월 26일 **Update 1 (Quality of Life Update)**가 예고되어, 개선 사항·새 도구·새 건물 부품·비주얼 업그레이드를 더했다. 2026년에도 데브로그(Devlog #21 등)가 이어지며 "경험 다듬기(Refining the Experience)"를 표방했다. 풀 모드 지원 엔진과 결합해 장기 수명을 도모하는 운영 기조다.

---

## 4. 평가

### 4.1 평론 점수 (정식 출시 1.0 기준)

《Foundation》 정식판은 평단에서 **대체로 호의적(generally favorable)** 평가를 받았다.

- **Metacritic**: 84/100 (generally favorable). OpenCritic 집계에서도 출시 직후 "찬사받는 리뷰(glowing reviews)"로 보도됐다.
- **SpazioGames**: 85/100 (8.5/10, 2025년 3월 15~16일)
- **NoobFeed**: 83/100 (2025년 2월 24일)
- **IGN Deutschland**: 80/100 — "아늑하고 입문자 친화적인 도시 빌더(a cozy and beginner-friendly city builder)"
- **GameStar**: 78/100 (2025년 3월 7일)

평론가들이 공통적으로 꼽은 강점은 다음과 같다.

> "one of those city builders you never want to put down" (한번 잡으면 손에서 놓고 싶지 않은 도시 빌더 중 하나)

> "everything you'd expect from a city management sim, skillfully blending creative freedom with careful planning" (도시 경영 시뮬레이션에서 기대할 만한 모든 것을 갖추었으며, 창조적 자유와 세심한 계획을 능숙하게 결합한다)

여러 매체가 "시각적으로 빼어나고(visually stunning) 플레이가 즐겁다"고 평했으며, GINX TV는 "풍부하고 보람 있는 중세 도시 빌더(A Rich, Rewarding Medieval City Builder)"라는 헤드라인을 달았다. 한 평가는 "완성된 패키지로서 매우 참신한 게임이며, 시장에서 최고의 중세 도시 빌더라 주장할 자격이 있다(a legitimate claim to be the best medieval city builder on the market)"고까지 평했다.

반대로 거의 모든 호평이 단 하나의 단서를 달았다 — "긴 개발 기간에도 불구하고 여전히 남아 있는 간헐적 버그와 몇 차례의 크래시(occasional bug and a few crashes that persist despite the long development time)."

### 4.2 유저 평가 (Steam)

상업적·커뮤니티적 성과는 평론 못지않게 견고하다.

- **Steam 전체 평가**: "매우 긍정적(Very Positive)" — 전체 리뷰 약 10,986건 중 **86%가 긍정적**.
- **출시 직후 동향**: 정식 출시 이틀 만에 긍정 338 vs 부정 141 수준으로 출발, 이후 안정적으로 "매우 긍정적"에 안착.
- 최근 30일 기준으로도 긍정 비율 83%대를 유지(시점에 따라 변동).

### 4.3 상업 지표

- **Steam 최고 동시 접속자**: **18,448명** (2025년 2월 2일, 정식 출시 직후). 도시 건설 장르의 싱글플레이 빌더로서는 매우 강력한 수치다.
- **누적 판매**: 얼리 액세스 기간이던 2019년 시점에 이미 **20만 장(200,000 copies)**을 돌파했다(Wikipedia 기준). 6년에 걸친 얼리 액세스와 정식 출시까지의 누적은 이를 크게 상회할 것으로 [추정]되나, Polymorph Games는 정식 출시 시점의 구체적 총판매량을 공개하지 않았다.

### 4.4 평론-유저 괴리

평론(84점대)과 유저(86% 긍정)의 방향이 일치한다는 점이 특징이다. 큰 괴리는 없으나, 미묘한 결의 차이는 존재한다. 평론은 "참신함·표현력·완성도"를 높이 사면서도 "버그·후반부 도전 부재"를 일관되게 감점 요인으로 든 반면, 일부 코어 유저 사이에서는 패치로 인한 변경(특히 1.0에서의 시스템 개편, 얼리 액세스 세이브 비호환)에 대한 불만이 표출되기도 했다("Congrats on ruining a good game" 같은 토론 스레드 존재). 즉, 신규·라이트 유저에게는 호평이지만, 오래된 코어 유저에게는 변화에 대한 호불호가 갈리는 양상이다.

---

## 5. 성공 요인 분석

### 5.1 단일 핵심 차별점에 집중 — "그리드가 없다"

《Foundation》의 성공은 "그리드 없는 유기적 건설"이라는 **단 하나의 강렬한 차별점**을 끝까지 밀어붙인 데서 나온다. 도시 빌더 장르는 포화 상태이지만, 대부분의 게임이 타일 격자 위 효율 퍼즐에 머물러 있었다. 《Foundation》은 "마을이 스프레드시트가 아니라 손으로 빚은 듯 자라난다"는, 한 줄로 설명 가능하면서도 스크린샷만으로 확연히 구별되는 차별점을 제시했다. 이 명료한 정체성은 마케팅·입소문·장르 내 포지셔닝 모두에서 강력한 무기였다.

### 5.2 표현력 중심 설계 — 창의력 발산의 장

생존 위협을 배제하고 모뉴먼트 디자인·문장 편집기·자유 배치를 전면에 둔 결정은, 도시 빌더를 "실패하지 않는 창작 도구"에 가깝게 만들었다. 《Cities: Skylines》가 현대 도시에서 그러했듯, 《Foundation》은 중세 도시에서 "내 마을을 자랑하고 싶게 만드는" 표현 욕구를 자극했다. 이는 스크린샷 공유·커뮤니티 자랑 문화로 이어지며 자연스러운 바이럴을 만든다.

### 5.3 비어 있던 틈새 — "전투 없는 Manor Lords"

타이밍과 시장 환경도 결정적이었다. 2024년 《Manor Lords》가 폭발적 화제를 모으며 중세 도시 빌더에 대한 수요를 환기했지만, 《Manor Lords》는 여전히 얼리 액세스였고 전투·전쟁 요소를 품고 있었다. 많은 플레이어가 원한 것은 "Manor Lords의 평화로운 마을 짓기 절반"이었다. 《Foundation》은 바로 그 수요를 정조준했다.

- "Manor Lords에 가장 가까운 단일 경험(the single closest experience to Manor Lords)"
- 단, **전투가 없고**, 평화로운 빌딩에 집중하며, **이미 정식 출시된 완성 패키지(more polished, fully released package)**

즉 화제작이 비워 둔 "전투 없는, 완성된 평화 빌더"라는 자리를 정확히 차지했다. 경제 루프(밀→밀가루→빵, 목재·석재 보급선)는 《Manor Lords》와 닮아 친숙하되, 그리드 없는 표현력과 완결성으로 차별화한 것이다.

### 5.4 6년의 얼리 액세스 — 커뮤니티 공동 개발

역설적으로 "1년 계획이 6년이 된" 긴 얼리 액세스는 약점인 동시에 성공 요인이었다. 그 기간 동안 게임은 커뮤니티 피드백을 받아 수없이 다듬어졌고, 정식 출시 시점에는 이미 1만 건 가까운 리뷰와 충성 팬층, 검증된 핵심 루프를 확보한 상태였다. 정식 출시는 "신작 발표"가 아니라 "오래 다듬어 온 게임의 완성 선언"이었고, 이는 출시 직후 1.8만 동접이라는 폭발적 복귀를 가능케 했다.

### 5.5 기술적 자부심 — 자체 엔진의 보상

자체 엔진 Hurricane은 막대한 개발 비용을 요구했지만, 그리드 없는 건설과 수천 명 주민 시뮬레이션이라는 핵심 차별점을 기술적으로 보장했다. 풀 모드 지원까지 염두에 둔 설계는 장기 수명의 토대가 된다. 소규모 스튜디오가 상용 엔진의 제약을 우회해 "자기만의 게임"을 만들 수 있음을 보여 준 사례다.

### 5.6 입문 장벽 완화 + 아늑한 톤

생존 압박 부재와 입문자 친화적 난이도, 따뜻한 아트 톤은 하드코어 전략 게이머를 넘어 **코지(cozy) 게임 수요층**까지 시장을 넓혔다. "느긋하게 예쁜 중세 마을을 키우는" 경험은 번아웃 없는 힐링 콘텐츠로 소비되며, 장르 외 유저까지 끌어들였다.

---

## 6. 비평적 시각 / 한계 / 논란

### 6.1 후반부 콘텐츠 고갈

가장 일관되게 지적된 약점은 **후반부 빈곤**이다. 여러 리뷰가 "첫 15~20시간은 탐험과 건설로 매력적이지만, 이후 콘텐츠가 예상보다 빨리 마르면서 정체된다(things plateau)"고 평했다. 새 건물 해금이 드물어지고 동일한 루프가 반복되며, 기본 난이도에서는 후반에 새로운 도전이 생기지 않는다는 것이다. 생존 압박을 배제한 설계의 필연적 대가로, "아늑함"이 "할 일 없음"으로 전이되는 지점이다.

### 6.2 UI/UX의 정보 부족

UI는 칭찬과 비판이 갈린다. 1.0에서 대대적으로 개편됐음에도, 일부 리뷰는 여전히 다음을 문제로 든다.

- 물류(logistics) 측면에서 정보가 부족해 "추측 게임(guesswork)"이 된다.
- 유용한 정보를 찾기 어렵고, 기록의 책(book of records)이 다루기 번거롭다.
- 건물 UI의 작은 패널이 탐색 시 답답하다.
- Polygon은 "성가신 UI 특이점(annoying user interface quirks)"을 지적했다.

즉 "정보를 충분히 공유하지 않아 무언가 빠진 느낌"이라는 평이 반복된다.

### 6.3 일부 시스템의 비효율·반직관성

코어 유저 사이에서는 설계의 깊이에 대한 불만도 있다. "상당수 생산 건물·사슬이 인력 낭비에 가깝고(complete waste of manpower)", 선술집 서비스와 사치품 노점이 서로 잠식하는(cannibalize) 등 일부 메커니즘이 반직관적으로 작동한다는 지적이다. 표현력은 풍부하나, 최적화 깊이를 추구하는 전략 게이머에게는 시스템적 정합성이 아쉬울 수 있다.

### 6.4 기술적 안정성 — 버그·크래시·세이브 손상

6년의 개발에도 불구하고 **안정성 이슈**가 끈질기게 남았다는 점은 거의 모든 호평이 단 단서다. 보고된 문제로는 빌더가 작업을 멈추거나 NPC가 끼이는 AI 버그, UI 프리징, 그리고 일부 플레이어가 세이브 손상(save corruption)으로 도시 전체를 잃는 사례까지 있다. "패치가 자주 새로운 문제를 만든다"는 불만도 있었다. 긴 개발 기간에 비추어 이 안정성 문제는 가장 뼈아픈 비판이다.

### 6.5 1.0 개편과 세이브 비호환 논란

정식 출시는 대규모 개편을 동반했고, 그 과정에서 **얼리 액세스 세이브가 1.0과 비호환**이 됐다(레거시 1.9 버전은 Steam 베타로 접근 가능). 진행 시스템·세무소·만다트 등의 재설계는 신규 유저에게는 개선이었지만, 수백 시간을 투자한 일부 베테랑에게는 "익숙한 게임이 바뀌어 버렸다"는 상실감으로 다가왔다. 토론 게시판의 "Congrats on ruining a good game" 류 스레드가 이 정서를 보여 준다. 라이브 게임의 메이저 개편이 으레 겪는 코어-라이트 유저 간 긴장의 전형적 사례다.

---

## 7. 영향과 유산

### 7.1 장르에 던진 화두 — 그리드의 종언?

《Foundation》은 "도시 빌더는 반드시 그리드여야 하는가"라는 질문을 대중적으로 검증했다. 유기적·그리드 없는 건설이 단순한 기믹이 아니라 상업적으로 성립하는 핵심 셀링 포인트가 될 수 있음을 입증했고, 이후 《Manor Lords》를 비롯한 "유기적 중세 빌더" 흐름과 함께 장르의 미학적 기대치를 끌어올렸다. 마을이 격자가 아니라 지형을 따라 자라야 한다는 감각은 이 게임이 장기간 전파해 온 가치다.

### 7.2 소규모 스튜디오의 장수 모델

Polymorph Games는 단일 타이틀에 6년을 투자해 정식 출시에 도달하고, 그 과정에서 20만 장 이상을 팔며 회사를 지탱한 **얼리 액세스 장수 모델**의 사례다. 1년 계획이 6년이 된 것은 분명 리스크 관리의 실패담이기도 하지만, 동시에 커뮤니티와 함께 게임을 완성해 정식 출시 순간 1.8만 동접으로 보상받은 인디 성공담이기도 하다. 자체 엔진 구축이라는 무모해 보이는 선택이 핵심 차별점으로 보답받은 사례이기도 하다.

### 7.3 "코지 빌더"의 확장

생존·전투를 배제하고 표현·아늑함에 집중한 설계는, 하드코어 전략 장르였던 도시 빌더를 코지 게임 영역으로 확장하는 흐름에 일조했다. "실패하지 않고 예쁜 마을을 키우는" 경험에 대한 시장 수요가 분명히 존재함을 보여 주었고, 이는 장르의 외연을 넓혔다.

### 7.4 문화적 의미 — 디지털 중세 도시계획

윈체스터 대학 중세 미디어 학술 발표에서 다뤄질 만큼, 《Foundation》은 단순 오락을 넘어 **중세 사회 구조(삼부회/신분제)와 도시계획을 게임 메커니즘으로 번역**한 사례로도 주목받았다. 앙시앵 레짐의 노동·성직·왕국 신분을 진행 시스템으로 직조한 설계는, 역사적 사회 구조를 플레이어가 손으로 체험하게 만든 흥미로운 시도였다.

---

## 8. 부록

### 8.1 핵심 통계 표

| 항목 | 내용 |
| --- | --- |
| 개발사 | Polymorph Games (캐나다 퀘벡시티, 2016년 2월 설립) |
| 퍼블리셔 | Polymorph Games (자체 퍼블리싱) |
| 엔진 | 자체 엔진 Hurricane (풀 모드 지원) |
| 플랫폼 | Windows (PC) |
| 장르 | 중세 도시 건설 시뮬레이션 (gridless) |
| 크라우드펀딩 | Kickstarter (2018) |
| 오픈 알파 | 2018 |
| 얼리 액세스 출시 | 2019년 2월 1일 |
| 정식 1.0 출시 | 2025년 1월 31일 |
| 사운드트랙 | Audinity 작곡, 100분+ (CK2·EU4 작업 경력) |
| Metacritic | 84/100 (generally favorable) |
| Steam 유저 평가 | "매우 긍정적" (약 10,986건 중 86% 긍정) |
| 최고 동시 접속 | 18,448명 (2025년 2월 2일) |
| 누적 판매(2019 시점) | 20만 장 이상 |
| 주요 사후 업데이트 | Update 1 QoL (2025년 11월 26일 예고) |

### 8.2 진행 시스템 요약 표

| 경로 | 해금 조건 | 기술 비용 | 성격 | 행정관 |
| --- | --- | --- | --- | --- |
| 공통(Common) | 번영도(Prosperity) | 금화(Gold Coins) | 기초 진행 | — |
| 노동(Labour) | 광휘(Splendour) | 영향력(Influence) | 승급·과세 | 베일리프(Bailiff) |
| 성직(Clergy) | 광휘(Splendour) | 영향력(Influence) | 사치 자원 교역 | 수도원 사절(Monastic Emissary) |
| 왕국(Kingdom) | 광휘(Splendour) | 영향력(Influence) | 병력·왕국 봉사 | 왕실 정신(Royal Courtier) |

### 8.3 주요 평론 인용 모음

- **SpazioGames**: 85/100 (8.5/10) — 창작 자유와 계획의 능숙한 결합
- **NoobFeed**: 83/100 — "한번 잡으면 놓고 싶지 않은 도시 빌더"
- **IGN Deutschland**: 80/100 — "아늑하고 입문자 친화적인 도시 빌더"
- **GameStar**: 78/100
- **GINX TV**: "A Rich, Rewarding Medieval City Builder"
- **Polygon**: 느긋한 플레이를 칭찬하되 "성가신 UI 특이점" 지적
- **Rock Paper Shotgun**: "a comfortable experience(편안한 경험)"

### 8.4 참고 자료 목록 (영어권 매체 중심)

- Wikipedia — *Foundation (video game)*: https://en.wikipedia.org/wiki/Foundation_(video_game)
- Polymorph Games 공식 — *Foundation 1.0 Is Now Available!* (2025.01.31): https://www.polymorph.games/foundation/news/2025/01/31/foundation-full-release/
- Polymorph Games 공식 뉴스 허브: https://www.polymorph.games/foundation/news/
- Official Foundation Wiki — *Progression*: https://wiki.polymorph.games/foundation/Progression
- Official Foundation Wiki — *1.0 Release*: https://wiki.polymorph.games/foundation/1.0_Release
- Official Foundation Wiki — *Mandates*: https://wiki.polymorph.games/foundation/Mandates
- Steam 상점 페이지 (app 690830): https://store.steampowered.com/app/690830/Foundation/
- SteamDB — 동접·차트: https://steamdb.info/app/690830/charts/
- Metacritic — *Foundation*: https://www.metacritic.com/game/foundation/
- OpenCritic — *Foundation*: https://opencritic.com/game/18070/foundation/reviews
- OpenCritic 뉴스 — *Popular Medieval City Builder Leaves Early Access to Glowing Reviews*: https://opencritic.com/news/11408/
- Game Rant — *Popular Medieval City Builder Leaves Early Access to Glowing Reviews*: https://gamerant.com/foundation-medieval-city-builder-pc-reviews/
- GINX TV — *Foundation Review: A Rich, Rewarding Medieval City Builder*: https://www.ginx.tv/en/video-games/foundation-review-polymorph-games
- BitsNPixels — *Foundation City-Builder Review 2025*: https://bitsnpixels.org/p/foundation-medieval-city-builder-review
- LadiesGamers — *Foundation Review*: https://ladiesgamers.com/foundation-review/
- Mega Bears Fan — *Foundation: a cozier, more expressive medieval city-builder*: http://www.megabearsfan.net/post/2025/10/01/Foundation-game-review.aspx
- Switchblade Gaming — *Best Games Like Manor Lords* (비교 분석): https://www.switchbladegaming.com/strategy-games/like-manor-lords/
- University of Winchester — *A Question of Class? The Three Estates as mechanic in Foundation* (학술 발표): https://issuu.com/theuniversityofwinchester/docs/mamg22_proceedings/s/17585391

---

*본 분석서는 2026년 6월 기준, 영어권 매체·공식 자료·커뮤니티 자료를 종합해 작성되었다. 판매·동접 등 수치는 출처 시점 기준이며, 라이브 운영 중인 게임 특성상 일부 수치는 시점에 따라 변동될 수 있다.*
