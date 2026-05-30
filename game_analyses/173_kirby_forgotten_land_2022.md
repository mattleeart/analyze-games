# Kirby and the Forgotten Land (2022) 심층 분석

> 30년 동안 옆으로만 걷던 분홍 공이 마침내 정면을 바라보고 입체 공간에 첫발을 디뎠다. 그리고 그 첫발은 시리즈 역사상 가장 많이 팔린 작품이 되었다. 《Kirby and the Forgotten Land》는 닌텐도가 "쉬운 게임"이라는 안전지대 안에서도 어떻게 디자인의 야망을 펼칠 수 있는지를 보여 준, 조용하지만 결정적인 전환점이다.

---

## 1. 게임 개요

《Kirby and the Forgotten Land》(이하 《Forgotten Land》)는 HAL Laboratory가 개발하고 Nintendo가 퍼블리싱한 3D 플랫포머다. 2022년 3월 25일 Nintendo Switch 전용으로 전 세계에 동시 출시되었으며, 이후 2025년 8월 28일에는 추가 캠페인 《Star-Crossed World》를 포함한 Nintendo Switch 2 Edition이 발매되었다.

이 작품의 가장 큰 역사적 의미는 단순하다. **커비 시리즈 30년 역사상 처음으로, 메인 넘버링 작품이 완전한 3D 공간을 무대로 삼았다는 것이다.** 1992년 게임보이판 《Kirby's Dream Land》 이래 커비는 거의 언제나 2D 횡스크롤(혹은 의사 3D)의 분홍 영웅이었다. 《Forgotten Land》는 그 30년의 관성을 깨고, 마리오가 《Super Mario 64》에서 했던 도약을 커비식으로 재해석했다.

### 개발사와 크레딧

- **개발사**: HAL Laboratory (보조 개발 Vanpool)
- **퍼블리셔**: Nintendo
- **디렉터**: Tatsuya Kamiyama(카미야마 타츠야) — 메인 시리즈 커비 작품의 디렉터를 맡은 것은 이번이 처음이었다.
- **제너럴 디렉터(종합 감독)**: Shinya Kumazaki(쿠마자키 신야) — 약 20년간 커비 시리즈에 관여해 온 베테랑으로, 본작에서는 캐릭터 디자인, 인게임 오디오, 서사 방향, 게임 텍스트 등 프로젝트 전반을 총괄했다. 사실상 작가(writer) 역할도 겸했다.
- **레벨 디자인 디렉터**: Yuki Endo(엔도 유키)
- **어소시에이트 프로듀서**: Kei Ninomiya(니노미야 케이, Nintendo)
- **프로듀서진**: Tadashi Kamitake, Toyokazu Nonaka, Akira Kinashi 등

### 개발 규모와 위상

HAL Laboratory는 《Forgotten Land》를 자사 역대 **최대 규모의 커비 프로젝트**로 규정했다. 닌텐도의 공식 개발자 인터뷰 시리즈 "Ask the Developer Vol. 4"(2022년 3월)와 GDC 2023 강연에 따르면, HAL은 3D 메인 커비를 오랫동안 준비해 왔으며, 직전작 《Kirby Star Allies》(2018)를 완성한 뒤 비로소 이 숙원 프로젝트에 본격 착수할 준비가 되었다고 밝혔다. 실제로 HAL은 《Star Allies》와 《Forgotten Land》를 하나의 "연결된 프로젝트(connected project)"로 인식했으며, 《Star Allies》가 부분적으로 차세대 커비의 기술적·디자인적 기반을 닦기 위한 작품이었다고 회고했다.

엔진/기술 스택에 대해서는 공식적으로 특정 상용 엔진(예: Unreal Engine)을 명시한 신뢰 가능한 1차 자료를 확인하기 어렵다. 따라서 본 분석서에서는 사용 엔진을 단정하지 않는다. 다만 개발진이 3D 전환 과정에서 마주한 기술적 난제(후술)는 자체적인 카메라·판정 보정 시스템을 구축했음을 시사한다. [추정]

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 컨셉과 세계관

《Forgotten Land》의 무대는 시리즈 팬에게도 낯선 곳이다. 평소 커비의 고향인 행성 Popstar의 Dream Land 위로 어느 날 거대하고 어두운 소용돌이(vortex)가 나타나 모든 것을 빨아들인다. 커비는 그 소용돌이에 휩쓸려, 고대 문명의 폐허가 흩어진 **신세계(the new world, 이른바 Forgotten Land)** 에 떨어진다.

이 세계의 미감은 커비 시리즈의 전통과 정면으로 충돌하면서도 묘하게 어우러진다. 파스텔톤의 동화적 캐릭터들이, 인류 문명이 사라진 듯한 **포스트-아포칼립스**의 무대 위를 뛰어다닌다. 녹슨 쇼핑몰, 물에 잠긴 놀이공원, 모래에 파묻힌 도시, 자연이 되삼킨 콘크리트 구조물. 이 "자연이 인공물을 되삼킨" 풍경은 《The Last of Us》나 《Horizon Zero Dawn》 같은 진지한 작품에서 익숙한 것이지만, 거기에 분홍 공 한 마리가 자판기를 통째로 삼키며 굴러다니는 순간 모든 무게가 유쾌하게 전복된다. 이 의외성 자체가 본작 아트 디렉션의 핵심 무기다.

### 줄거리 (스포일러 포함 — [스포일러])

[스포일러] 신세계에서 커비는 토착 야생 무리인 **Beast Pack**이 Dream Land에서 함께 빨려 온 Waddle Dee들을 납치하고 있음을 발견한다. 그 와중에 친칠라를 닮은 작은 생물 **Elfilin**을 만난다. Elfilin은 Waddle Dee들이 이 세계에 정착하도록 도운 선한 존재다. 커비와 Elfilin은 납치된 Waddle Dee들을 구출하며 모험을 시작한다.

[스포일러] Beast Pack의 수장은 사자 형태의 **Leongar**다. 그는 고대 주민들이 "ID-F86"이라 불리는 존재의 힘으로 "꿈의 땅"으로 떠났다는 전설을 설명하며, Fecto Forgo와 Elfilin을 재결합시켜 자신도 같은 길을 가려 한다.

[스포일러] 진실은 이렇다. **Fecto Forgo**는 수세기 전, 아직 번성하던 Forgotten Land 문명을 침공하려던 외계 생명체였다. 그 외계체는 포획되었고, 주민들은 그것의 차원 균열 능력을 연구해 결국 그 힘으로 이 세계를 떠났다. 그 과정에서 외계체는 둘로 분리되었으니, 선한 반쪽이 **Elfilin**, 위험한 반쪽이 **Fecto Forgo**다.

[스포일러] Leongar를 쓰러뜨린 직후 Fecto Forgo가 각성한다. 그는 사실 Leongar에게 빙의해 Beast Pack을 조직했고, Dream Land로 향하는 소용돌이를 열었으며, King Dedede를 최면으로 조종하고 Waddle Dee들을 노동력으로 납치한 흑막이었다. 모든 것은 중단되었던 침공을 재개하기 위한 포석이었다.

[스포일러] **일반 엔딩**: Fecto Forgo가 Elfilin을 흡수하면 둘은 본래의 완전한 형태 **Fecto Elfilis**로 결합한다. 커비는 Fecto Elfilis를 약화시켜 Elfilin을 떼어내지만, Fecto Elfilis는 Popstar로 향하는 거대한 소용돌이를 만들어 신세계와 충돌 코스에 올린다. 커비는 마지막 순간 **세미 트레일러 트럭을 입에 머금어 그대로 들이받아** Fecto Elfilis를 격파한다(본작 명물 Mouthful Mode의 서사적 클라이맥스). Elfilin은 자신의 모든 힘을 쏟아 두 세계 사이의 소용돌이를 봉인하고, 커비는 신세계에 남겨진다.

[스포일러] **트루 엔딩**: 커비와 Elfilin은 또 다른 차원 **Isolated Isles: Forgo Dreams**로 향해 Leongar의 영혼을 수거하고 그를 구하려 한다. Soul Forgo에게 빙의된 Leongar를 쓰러뜨리면 Soul Forgo가 모습을 드러내고, 진홍빛 나비가 날아들어 그것을 흡수하며 영혼을 포식하는 발키리형 전사 **Morpho Knight**로 변신한다. 커비가 Morpho Knight를 격파하면서 Leongar는 완전히 해방된다.

[스포일러] **시크릿/궁극 엔딩**: 선택적 최종 도전에서 커비는 Forgo Dreams의 환영들과 보스 러시를 치른 뒤 새로 형성된 **Chaos Elfilis**와 맞붙는다. 이를 격파하면 남은 영혼의 잔재가 Elfilin에게 다가오고, Elfilin은 이를 받아들여 마침내 자신의 두 반쪽을 온전한 하나로 만든다.

이처럼 본작은 표면적으로는 밝고 귀여운 어린이용 어드벤처지만, 그 이면에는 멸망한 문명, 분리된 자아, 영혼을 둘러싼 비극이라는 커비 특유의 "표면은 동화, 심층은 코스믹 호러"의 이중 구조를 깔아 두었다. 시리즈 팬들이 오랫동안 사랑해 온 이 톤의 격차가 《Forgotten Land》에서도 충실히 살아 있다.

### 캐릭터와 무드

주역은 언제나처럼 말 없는 커비, 그리고 본작의 새로운 파트너 Elfilin이다. 2인 협력 시 등장하는 **Bandana Waddle Dee**는 창을 든 든든한 조력자이며, 시리즈 단골인 King Dedede와 Meta Knight도 (대개 적/장애물로) 등장한다. 무드는 앞서 말한 대로 "동화적 캐릭터 × 폐허가 된 현실 세계"의 대비가 지배한다.

### 사운드와 음악

음악은 **Yuuta Ogasawara**(Lead Sound), **Hirokazu Ando**(Lead Music), **Jun Ishikawa**, **Yuki Shimooka**가 작곡했고, 상징적인 테마곡 "Welcome to the New World"는 **Tadashi Ikegami**가 작곡했다. 특히 Hirokazu Ando는 HAL Laboratory의 시니어 사운드 작곡가로 커비 시리즈를 대표하는 작곡가 중 한 명이며, 2016년부터 리드 사운드 직을 맡아 왔다. 본작의 사운드트랙은 보스전의 격렬한 록/오케스트라 편곡부터 Waddle Dee Town의 따스한 멜로디까지 폭넓은 스펙트럼을 보여 주며, 다수 평론에서 게임의 강점으로 직접 언급되었다.

---

## 3. 핵심 시스템 / 메카닉

### 코어 게임플레이 루프

본작의 모먼트-투-모먼트는 전통적인 커비 문법을 3D로 옮긴 것이다. 적을 **흡입(inhale)** 하고, 뱉어서 발사하거나 삼켜서 그 적의 능력을 복사(**Copy Ability**)하고, 그 능력으로 전투와 플랫포밍, 그리고 곳곳에 숨겨진 수집 요소를 해결한다. 여기에 본작만의 두 가지 혁신 — Mouthful Mode와 Evolved Copy Abilities — 이 더해진다.

### 진행 구조

게임은 **6개의 메인 월드**로 구성되며, 각 월드에는 여러 스테이지, 클리어 후 공개되는 미션 목록, 그리고 숨겨진 Waddle Dee들이 배치되어 있다. 각 스테이지를 클리어할 때마다 사전에 비공개였던 미션이 드러나는데(예: "특정 장소의 Waddle Dee 구출", "숨은 보물 발견", "특정 조건 달성"), 이는 한 스테이지를 여러 번 반복 플레이하게 만드는 동시에 첫 플레이의 발견 쾌감을 해치지 않는 영리한 설계다. 진행은 선형적인 스테이지 기반으로, 오픈월드가 아니다. 다수 매체가 이를 두고 **"《Super Mario Odyssey》보다 《Super Mario 3D World》에 가깝다"** 고 평했다.

### 허브 — Waddle Dee Town

구출한 Waddle Dee들은 중앙 허브 **Waddle Dee Town**으로 모인다. 구출 인원이 늘어날수록 마을이 재건·확장되어 무기상, 미니게임, 카페, 낚시터, 영화관 등 다양한 시설이 차례로 열린다. 일부 시설은 일정 인원 또는 스토리 진행을 요구한다. 즉 "Waddle Dee 구출"이라는 수집 행위가 곧바로 허브의 성장과 보상으로 환원되는, 명확하고 만족스러운 진척 루프가 게임 전체를 떠받친다.

### Mouthful Mode — 본작의 간판 메카닉

**Mouthful Mode**는 본작이 시리즈에 가져온 가장 상징적인 신규 시스템이다. 커비가 자동차, 교통 콘, 자판기, 전구, 코일, 계단, 물풍선, 심지어 세미 트레일러 트럭 같은 **현실의 거대한 사물을 통째로 입에 머금어** 그 사물 자체로 변형하는 것이다. 자동차 커비는 빠르게 질주하고, 자판기 커비는 캔을 발사하며, 코일 커비는 높이 튀어 오르고, 계단 커비는 굴러서 경사를 내려간다.

설계상 중요한 디테일이 둘 있다.

1. **Copy Ability와 동시 보유가 가능하다.** 커비는 Copy Ability 하나와 Mouthful Mode 하나를 동시에 가질 수 있다. Mouthful Mode를 쓰기 위해 Copy Ability를 버릴 필요가 없고, Mouthful Mode 중에는 Copy 능력을 사용할 수 없지만 그렇다고 잃지도 않는다.
2. **Mouthful Mode는 무기보다 진행·퍼즐 수단에 가깝다.** 적을 공격하는 데 쓸 수도 있지만, 본질적으로는 레벨을 통과하고 퍼즐을 풀기 위한 도구다. 덕분에 전투용 Copy Ability와 역할이 깔끔하게 분리되어, 두 시스템이 서로의 영역을 침범하지 않는다.

Mouthful Mode는 본작의 비주얼 아이덴티티이자 마케팅의 핵심이기도 했다. 트레일러에서 자동차를 삼킨 커비의 모습은 즉각적인 화제를 모았고, 앞서 보았듯 최종 보스를 트럭으로 들이받는 클라이맥스로 서사적 정점까지 책임진다.

### Copy Ability와 Evolved Copy Abilities

전통의 Copy Ability는 본작에서 한층 정련되었다. Sword, Fire, Ice, Ranger(신규, 원거리 사격), Drill(신규, 지중 이동/공격), Cutter, Bomb 등 다양한 능력이 있으며, 각 능력은 **하나 이상의 진화형(Evolved Copy Ability)** 으로 강화할 수 있다.

진화 절차는 본작 경제 시스템의 중심이다.
- 스테이지에서 **설계도(blueprint)** 를 수집한다.
- 이를 Waddle Dee Town의 **무기상 Waddle Dee**에게 전달한다.
- **Star Coins**(화폐)와 **Rare Stones**(희귀 재료)를 지불해 진화형을 구매·해금한다.

예컨대 기본 Sword가 강력한 광역기를 가진 상위 검으로, Ranger가 더 강력한 사격 능력으로 진화하는 식이다. 이 시스템은 "수집(설계도) → 자원 축적(Star Coin/Rare Stone) → 강화(진화) → 더 어려운 콘텐츠 도전"이라는 선순환을 만들어, 단순한 클리어 너머의 장기 동기를 부여한다.

### Treasure Road — 집중형 챌린지

각 월드 곳곳에는 **Treasure Road**라는 사이드 스테이지가 숨어 있다. 이들은 특정 Copy Ability 또는 Mouthful Mode를 지정해 주는 짧고 집중적인 **타임 트라이얼**로, 목표 완주 시간을 달성하면 추가 보상(주로 Rare Stone)을 준다. 목표 시간은 종종 거의 완벽한 실행을 요구할 만큼 빡빡해, 본작에서 보기 드물게 진지한 손맛의 도전을 원하는 플레이어를 위한 콘텐츠 역할을 한다. 즉 메인 스테이지는 누구나 즐길 수 있게 너그럽게 두되, 도전 욕구는 Treasure Road와 후술할 콜로세움으로 분리해 흡수하는 영리한 난이도 분배다.

### 난이도와 접근성

**《Forgotten Land》는 시리즈 최초로 명시적인 난이도 선택지를 도입했다.**

- **Spring-Breeze Mode**(봄바람 모드): 이지 난이도. 커비와 Bandana Waddle Dee의 체력이 **400 HP**로 크게 높아지고, 일부 스테이지에서는 적 수가 줄어든다. 어린이·초심자·여유로운 플레이를 원하는 사람을 위한 모드.
- **Wild Mode**(와일드 모드): 표준/도전 난이도. 체력이 **250 HP**로 낮고 적이 더 많으며 더 까다롭지만, 그 대가로 Star Coin 보상이 늘어난다.

핵심은 **게임 도중 언제든 두 모드를 자유롭게 전환할 수 있다**는 점이다. 까다로운 보스 앞에서 잠시 Spring-Breeze로 낮췄다가, 자신이 붙으면 다시 Wild로 올리는 식의 유연한 운용이 가능하다. 이는 "쉬운 게임 vs 어려운 게임"이라는 이분법 대신, 플레이어가 매 순간 자신에게 맞는 경험을 직접 조립하게 하는 현대적 접근성 설계다.

### 협력 플레이

본작은 **로컬 2인 협력**을 지원한다. 두 번째 플레이어는 창을 휘두르는 **Bandana Waddle Dee**를 조작한다. 커비가 Copy Ability와 Mouthful Mode로 다채로운 액션을 펼치는 동안, Waddle Dee는 단순하지만 든든한 근접 딜러로 가족·친구 동반 플레이의 진입 장벽을 낮춘다.

### 기타 콘텐츠

게임 본편 클리어 후에는 **콜로세움**(보스 러시형 챌린지)이 열려, 강화된 보스들을 연속으로 상대하는 진지한 전투 콘텐츠를 제공한다. 가장 강력한 진화 능력을 해금하고도 고전할 수 있을 만큼의 난도를 갖춰, 본편의 너그러움과 균형을 이룬다. 또한 amiibo를 지원해 추가 보너스를 제공한다.

### UI/UX 디자인 철학

본작의 UI/UX는 일관되게 "쉽지만 깊게"라는 철학을 따른다. 진척 미션을 클리어 후에 공개해 첫 플레이의 발견을 보호하고, 수집과 강화의 인과를 허브에서 가시적으로 보여 주며, 난이도를 실시간으로 조절할 수 있게 한다. 이 모든 장치가 "누구도 막히지 않게 하되, 원하는 사람은 깊이 파고들 수 있게" 한다는 닌텐도식 접근성 철학의 모범 사례다.

---

## 4. 평가

### 평론 점수

《Forgotten Land》는 출시와 함께 폭넓은 호평을 받았다.

| 매체 | 점수 |
| --- | --- |
| Metacritic (Switch) | 85 / 100 |
| OpenCritic | 85 (Mighty/Top Critic 평균) |
| GameSpot | 9 / 10 |
| IGN | 8 / 10 |
| Edge | 8 / 10 |
| Eurogamer | Recommended |
| Nintendo Life | 매우 높은 호평 (Switch 최고 3D 플랫포머 중 하나) |

(참고: 2025년 Nintendo Switch 2 Edition + Star-Crossed World의 Metacritic은 83.)

### 주요 평론 인용

- **GameSpot (9/10)**: "Kirby and the Forgotten Land는 훌륭하게 설계된 스테이지와 역동적인 능력 무기고 덕분에 Nintendo Switch 최고의 플랫포머 중 하나다." (one of the best platformers on Nintendo Switch thanks to its brilliantly designed stages and a dynamic arsenal of abilities)
- **IGN (8/10)**: "Kirby and the Forgotten Land는 시리즈가 이미 보유한 즐거운 능력 기반 전투·플랫포밍·비밀 찾기의 조합을 3차원으로 성공적으로 비틀어 옮겨 놓았다." (successfully warps the series' already fun mix of ability-based combat, platforming, and secret hunting into the third dimension)
- **Edge (8/10)**: "콤팩트하고 상상력 넘치는 모험"이자 "조용한 승리, 대단한 솜씨와 재치의 작품"이라고 평하면서도, "지금껏 커비의 매력을 이해하지 못했던 이들이 그의 3D 진출로 설득될 가능성은 낮다"고 단서를 달았다. (a compact, imaginative adventure / a low-key triumph, a work of great craft and wit)
- **Nintendo Life**: 전체 캠페인을 통틀어 거슬리는 레벨이 단 하나도 없었다며, Switch에서 가장 정제된 3D 플랫포머 중 하나로 꼽았다.

### 수상 이력

- **The Game Awards 2022 — Best Family Game 수상.** 《LEGO Star Wars: The Skywalker Saga》, 《Splatoon 3》 등 쟁쟁한 경쟁작을 제치고 수상했다.
- **Japan Game Awards 2022 — Award for Excellence(우수상).**
- **BAFTA Games Awards 2023 — Family 부문 수상.**
- **New York Game Awards 2023 — Best Kids Game.**

### 상업적 지표

상업적으로 《Forgotten Land》는 커비 역사를 새로 썼다.

- **출시 2주 만에 전 세계 210만 장 이상** 판매(Shacknews 보도).
- **일본 발매 첫 이틀 물리판 380,060장** — 시리즈 역대 최고의 물리판 런칭.
- **출시 첫 15주 누적 455만 장** — 당시 기준 시리즈 역대 최고 sell-through(Game Developer 보도).
- **2024년 3월 31일 기준 누적 752만 장**(닌텐도 결산 기준) — **커비 프랜차이즈 역사상 최다 판매작.**
- 2022년 미국 시장 연간 판매 14위.

후속 보도들에 따르면 누적 판매는 이후로도 계속 늘어 2025년 시점에는 약 800만 장 안팎으로 추산된다. [추정]

### 유저 평가와 평론-유저 괴리

유저 평가 또한 대체로 매우 우호적이었다. ResetEra와 Famiboards의 리뷰 스레드, Metacritic 유저 스코어 모두 "커비의 3D 데뷔가 기대 이상으로 매끄러웠다"는 반응이 주를 이뤘다. 평론-유저 간 큰 괴리는 거의 없었으며, 갈리는 지점은 오직 하나 — **난이도** 였다. 일부 코어 플레이어는 본편이 지나치게 쉽다고 느꼈고, 반대로 가족 단위·라이트 유저층에게는 그 너그러움이 정확히 본작을 사랑하게 만든 이유였다.

---

## 5. 성공 요인 분석

### (1) "쉬운 전환"이라는 디자인적 정답

3D 전환은 모든 2D 프랜차이즈의 무덤이 될 수 있는 도박이다. 《Sonic》, 《Castlevania》, 《Mega Man》 등 수많은 시리즈가 3D 전환에서 정체성을 잃거나 조작감을 망쳤다. HAL이 택한 길은 영리하게도 **욕심을 부리지 않는 것**이었다. 오픈월드(《Mario Odyssey》)가 아니라 잘 짜인 선형 스테이지(《Super Mario 3D World》)를, 자유로운 카메라가 아니라 의도된 시점을 택했다. 그 결과 "3D가 처음인 커비"가 길을 잃지 않고 자신의 강점 — 흡입·복사·발견의 즐거움 — 을 고스란히 새 차원으로 옮겨 올 수 있었다. 적게 시도해서 확실히 성공한, 신중한 디자인의 승리다.

### (2) Mouthful Mode라는 단 하나의 강력한 후크

신규 IP나 신규 시도에는 한눈에 각인되는 "후크"가 필요하다. 《Forgotten Land》에게 그것은 명백히 Mouthful Mode였다. 자동차를, 자판기를, 트럭을 통째로 삼키는 분홍 공의 이미지는 트레일러 한 컷만으로 강렬한 인상을 남겼고, 실제 플레이에서도 "다음엔 뭘 삼킬 수 있을까"라는 호기심으로 진행 동기를 끊임없이 자극했다. 하나의 메카닉이 마케팅 후크와 게임플레이 동기와 서사 클라이맥스를 동시에 책임진, 보기 드물게 효율적인 설계다.

### (3) 접근성과 깊이의 양립

본작은 "쉬운 게임은 얕고, 깊은 게임은 어렵다"는 흔한 이분법을 거부한다. 메인 스테이지는 누구나 즐기게 너그럽게 두되, Treasure Road의 빡빡한 타임 트라이얼과 콜로세움, 진화 능력 컬렉션, 트루/시크릿 엔딩에 이르는 다층 콘텐츠로 코어 플레이어의 깊이 욕구를 별도 트랙으로 흡수했다. 거기에 실시간 난이도 전환까지 더해, 가족과 코어 게이머가 같은 게임을 각자의 방식으로 즐길 수 있게 했다. 이 폭넓은 수용성이 시리즈 최다 판매라는 결과의 직접적 동력이었다.

### (4) 타이밍과 시장 환경

2022년 3월은 《Elden Ring》(2월 말)이 게임계를 집어삼킨 직후였다. 광활하고 가혹한 소울라이크 대작에 지친 플레이어들에게, 정확히 그 반대편의 따뜻하고 너그러운 3D 플랫포머는 완벽한 대안이었다. 또한 Switch가 보급 정점에 달해 가족 단위 게임의 시장이 가장 두터웠던 시기였고, 커비 시리즈 30주년이라는 기념비적 맥락도 마케팅에 힘을 보탰다.

### (5) HAL의 장기 준비와 "연결된 프로젝트" 전략

성공은 하루아침에 오지 않았다. HAL은 직전작 《Star Allies》를 부분적으로 차세대 커비의 기반을 닦는 작업으로 활용했고, 두 작품을 하나의 연속된 프로젝트로 인식하며 수년간 3D 전환을 준비했다. 콘솔 메인 커비가 10년 넘게 부재했던 "컨셉이 맞물리지 않던 시기"를 인내한 끝에, 모든 조건이 맞아떨어진 시점에 출시한 것이다.

---

## 6. 비평적 시각 / 한계 / 논란

### 카메라

가장 자주 지적된 약점은 **카메라**다. 선형 스테이지 기반 3D 구조에서 카메라가 종종 플레이어에게 불리하게 작동해, 숨겨진 비밀이나 보물을 사각·구석·후방에 가려 놓는 경우가 있었다. 자유 회전이 제한된 시점 설계의 대가다. 다만 이는 치명적 결함이라기보다 "더 다듬을 수 있었던" 수준의 흠으로 평가된다.

### 낮은 난이도

본편의 표준 난이도는 코어 플레이어 일부에게 지나치게 쉽게 느껴졌다. 보스전은 즐겁지만 대체로 쉽게 격파되며, 회피 메카닉을 익히면 더욱 그렇다. 일부 유저는 시리즈가 "유아용 첫 플랫포머(babies first platformer)" 이상이 되기를 바란다고 토로하기도 했다. 그러나 이는 본질적으로 관점의 문제다. 커비 시리즈는 언제나 도전보다 위안을 주는, 편안한 어드벤처를 지향해 왔으며, 본작은 콜로세움·Treasure Road라는 별도 트랙으로 도전 욕구를 충실히 흡수했다. "쉬움"은 결함이 아니라 의도된 정체성이라는 것이 다수의 결론이다.

### 3D 전환의 본질적 한계

Edge가 지적했듯, 본작은 "이미 커비를 사랑하던 이들"에게는 더없이 만족스럽지만 "커비의 매력을 이해하지 못하던 이들"을 새로 설득하지는 못했다. 안전한 디자인을 택한 대가로, 《Mario Odyssey》급의 폭발적 혁신이나 장르의 천장을 깨는 야망까지는 보여 주지 못했다는 평이다. 즉 "흠잡을 데 없이 잘 만든 작품"이되 "장르를 재정의한 걸작"의 반열에는 살짝 못 미친다는 것이 비평적 합의에 가깝다.

---

## 7. 영향과 유산

### 시리즈에 미친 영향

《Forgotten Land》의 가장 직접적인 유산은 **"커비는 3D에서도 통한다"는 것을 상업적·비평적으로 동시에 증명한 것**이다. 본작 이전에는 《Kirby: Planet Robobot》(3DS, 2016)이 시리즈 최고작으로 널리 꼽혔으나, 《Forgotten Land》는 점수·판매·문화적 임팩트 모든 면에서 새로운 기준점이 되었다. 시리즈 최다 판매작이라는 기록은 향후 메인 커비가 나아갈 방향이 3D임을 사실상 확정했다.

### 산업적 의미

본작은 닌텐도의 "접근성 우선" 디자인 철학이 상업적으로 얼마나 강력한지를 다시 한번 입증했다. 실시간 난이도 전환, 발견을 보호하는 미션 공개 구조, 수집-강화의 명료한 인과 같은 장치들은 "넓은 대중을 막히지 않게 하면서도 코어를 만족시키는" 현대 패밀리 게임 설계의 교본으로 자주 인용된다. 특히 《Elden Ring》으로 대표되는 "고난도 = 깊이"라는 시대적 분위기 한가운데에서, 정반대 철학으로 700만 장을 넘긴 사실은 게임 디자인 다양성의 가치를 웅변한다.

### 문화적 의미와 후속

본작은 The Game Awards, BAFTA, New York Game Awards에서 잇따라 가족·키즈 부문을 석권하며 "최고의 가족 게임"의 대명사가 되었다. 그리고 그 유산은 2025년 8월 28일 발매된 **Nintendo Switch 2 Edition + 《Star-Crossed World》** 추가 캠페인으로 이어졌다. 신세대 하드웨어에서 향상된 비주얼과 새로운 모험을 더해, 출시 3년이 지나서도 IP의 생명력을 연장한 것이다. 커비의 3D 전환은 단발성 실험이 아니라 시리즈의 새로운 표준으로 정착했다.

### GDC를 통한 지식 공유

HAL의 개발진은 2023년 GDC 강연을 통해 3D 전환의 구체적 과정과 난제, 해법을 공개했다. 완전한 구형 실루엣이라는 캐릭터 디자인이 3D에서 방향 인지를 어렵게 만든 문제, 흡입·뱉기·점프 같은 기본 액션을 단순 3D 이식했을 때 의도대로 작동하지 않은 문제, 그리고 커비와 카메라의 위치를 추적해 "공격이 닿는 것처럼 보이는 범위"를 매핑하는 보정 시스템 등 — 이 경험담은 다른 개발자들에게도 2D-to-3D 전환의 실전 레퍼런스로 가치를 지닌다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
| --- | --- |
| 출시일 (Switch) | 2022년 3월 25일 |
| 출시일 (Switch 2 Edition + Star-Crossed World) | 2025년 8월 28일 |
| 개발사 / 퍼블리셔 | HAL Laboratory (Vanpool 협력) / Nintendo |
| 장르 | 3D 플랫포머 |
| 디렉터 | Tatsuya Kamiyama / 종합 감독 Shinya Kumazaki |
| Metacritic (Switch) | 85 / 100 |
| OpenCritic | 85 |
| 누적 판매 (2024-03-31) | 752만 장 (프랜차이즈 최다) |
| 일본 첫 이틀 물리판 | 380,060장 (시리즈 최고 물리 런칭) |
| 첫 15주 누적 | 455만 장 |
| 주요 수상 | TGA 2022 Best Family Game, BAFTA 2023 Family, NY Game Awards 2023 Best Kids Game, Japan Game Awards 2022 우수상 |
| 메인 월드 수 | 6개 |
| 난이도 모드 | Spring-Breeze (400 HP) / Wild (250 HP), 실시간 전환 가능 |

### 주요 메카닉 요약

| 시스템 | 설명 |
| --- | --- |
| Mouthful Mode | 자동차·자판기·트럭 등 거대 사물을 머금어 변형, 진행·퍼즐 중심. Copy Ability와 동시 보유 가능 |
| Copy Ability / Evolved | 설계도 수집 → 무기상 Waddle Dee에게 전달 → Star Coin + Rare Stone으로 진화형 해금 |
| Waddle Dee Town | 구출 인원에 따라 재건·확장되는 허브. 시설·미니게임 해금 |
| Treasure Road | 특정 능력 지정 타임 트라이얼. 빡빡한 목표 시간, Rare Stone 보상 |
| 콜로세움 | 본편 후 보스 러시형 고난도 챌린지 |

### 주요 인터뷰 / 강연 / 자료 링크

- Nintendo, "Ask the Developer Vol. 4: Kirby and the Forgotten Land — Part 1": https://www.nintendo.com/us/whatsnew/ask-the-developer-vol-4-kirby-and-the-forgotten-land-part-1/
- Nintendo Life, "Kirby and the Forgotten Land and Star Allies Were One Big 'Connected Project'": https://www.nintendolife.com/news/2022/08/kirby-and-the-forgotten-land-and-star-allies-were-one-big-connected-project-for-hal-laboratory
- Nintendo Wire, "Kirby directors explain process, challenges, and tweaks of going 3D in GDC Talk"(GDC 2023): https://nintendowire.com/news/2023/04/24/kirby-directors-explain-process-challenges-and-tweaks-of-going-3d-in-gdc-talk/
- Nintendo Dream 2022년 6월호 인터뷰 영문 번역: https://gigi9714.wordpress.com/2022/07/31/translation-of-the-kirby-and-the-forgotten-land-interview-from-the-june-2022-edition-of-nintendo-dream/

### 참고 자료 목록 (영어권 매체 중심)

- Wikipedia, "Kirby and the Forgotten Land": https://en.wikipedia.org/wiki/Kirby_and_the_Forgotten_Land
- Metacritic (Switch): https://www.metacritic.com/game/kirby-and-the-forgotten-land/
- OpenCritic: https://opencritic.com/game/12682/kirby-and-the-forgotten-land
- Game Developer, "Kirby and the Forgotten Land sells 4.55 million copies in four months": https://www.gamedeveloper.com/business/kirby-and-the-forgotten-land-sells-4-55-million-copies-in-four-months
- Shacknews, "Kirby and the Forgotten Land sold over 2.1 million units in just 2 weeks": https://www.shacknews.com/article/130296/kirby-and-the-forgotten-land-sold-over-21-million-units-in-just-2-weeks
- WiKirby, "Mouthful Mode": https://wikirby.com/wiki/Mouthful_Mode
- GameRant, "Kirby and the Forgotten Land: Ending Explained": https://gamerant.com/kirby-and-the-forgotten-land-morpho-knight-ending-lore-story-explained/
- NintendoSoup, "Kirby And The Forgotten Land Wins Best Family Game At The Game Awards 2022": https://nintendosoup.com/kirby-and-the-forgotten-land-wins-best-family-game-at-the-game-awards-2022/
- Nintendo Life, "Kirby Is Officially A BAFTA Winner": https://www.nintendolife.com/news/2023/03/kirby-is-officially-a-bafta-winner-takes-home-best-family-game
- Game8, "Difficulty Differences: Wild Mode vs Spring-Breeze Mode": https://game8.co/games/Kirby-and-the-Forgotten-Land/archives/371230

---

> 《Forgotten Land》는 야망의 크기로 승부한 작품이 아니다. 그것은 "무엇을 시도하지 않을지"를 정확히 아는 절제의 작품이다. 분홍 공이 30년 만에 정면을 바라보았을 때, HAL은 무리하게 달리는 대신 한 발 한 발 확실히 디뎠고, 그 신중함이 시리즈 최다 판매라는 보상으로 돌아왔다. 가끔은, 가장 안전한 길이 가장 멀리 간다.
