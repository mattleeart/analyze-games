# Songs of Conquest (2024) 심층 분석

> 《Heroes of Might and Magic 3》가 남긴 빈자리를, 25년이 지나서야 채운 게임. 스웨덴의 8인 인디 스튜디오 Lavapotion이 2년의 얼리 액세스를 거쳐 2024년 5월 정식 출시한 《Songs of Conquest》는 "어드벤처 전략(adventure strategy)"이라는, 한때 죽었다고 여겨진 서브장르를 픽셀 아트와 에센스(Essence) 마법 시스템으로 되살려냈다. 본 분석서는 이 게임이 무엇이며, 어떤 시스템으로 작동하고, 왜 50만 장을 팔며 평단과 팬을 동시에 만족시켰는지를 영어권 자료를 토대로 정밀하게 다룬다.

---

## 1. 게임 개요

### 기본 정보

| 항목 | 내용 |
|------|------|
| 제목 | 《Songs of Conquest》 |
| 개발사 | Lavapotion (스웨덴 예테보리 / Gothenburg) |
| 퍼블리셔 | Coffee Stain Publishing |
| 장르 | 턴제 어드벤처 전략(turn-based adventure strategy) / 4X·택틱스 하이브리드 |
| 엔진 | Unity |
| 얼리 액세스 | 2022년 5월 10일 (Steam, GOG, Epic Games Store) |
| 정식 출시(1.0) | **2024년 5월 20일** (Windows, macOS) |
| 콘솔판 | 2024년 11월 12일 (PS5, Xbox Series X/S) |
| 모바일판 | 2025년 3월 13일 (Android, iOS) |
| Nintendo Switch | 2025년 6월 17일 |

(출처: [Wikipedia](https://en.wikipedia.org/wiki/Songs_of_Conquest), [Steam](https://store.steampowered.com/app/867210/Songs_of_Conquest/))

### 개발사와 주요 크레딧

Lavapotion은 2017년 스웨덴 예테보리에서 게임·영화 업계 베테랑들이 모여 설립한 소규모 스튜디오다. 핵심은 "작지만 단단한 팀"이라는 점이다. GameDiscover의 분석에 따르면 초기 개발은 **단 4명**으로 시작해 2022년 얼리 액세스 시점에도 **약 8명** 규모였다. 50만 장 판매라는 결과를 생각하면 인당 생산성이 비범한 인디 케이스다.

주요 크레딧은 다음과 같다(출처: Wikipedia, GameRant 인터뷰).

- **Magnus Alm** — CEO 겸 프로듀서. Lavapotion 창업자 중 한 명이며, 인터뷰에서 "Lavapotion 창업자 전원이 《HoMM 3》의 열렬한 팬이었다"고 밝힌 인물.
- **Carl Toftfelt** — 리드 게임 디자이너. 시스템·밸런스·에센스 마법의 설계를 주도.
- **Patrik Liljecrantz** — 테크니컬 아티스트 / 프로그래머. 2.5D 렌더링 파이프라인의 핵심.
- **Niklas Borglund** — 리드 프로그래머.
- **Anders Gullmarsvik** — 아티스트.
- **Kim Tough** — 작가(narrative).
- **Reynir Helgason** — 작곡가. 게임의 정체성을 좌우하는 오리지널 사운드트랙을 담당.

### 개발 기간과 규모

개발은 **2017년 초**(일부 자료는 2017년 스튜디오 설립과 함께)부터 시작되었다. 2019년부터 2021년 5월까지 클로즈드 알파 신청자가 **2만 명 이상** 누적될 만큼, 정식 발매 이전부터 장르 팬덤의 기대를 모았다. GameDiscover는 "얼리 액세스 진입 전까지 약 5년을 들였다"고 정리한다.

당초 출시는 2020년 말로 예정되었으나 COVID-19의 영향 등으로 연기되어 2022년 5월 얼리 액세스로 첫 공개되었고, 이후 **2년간의 얼리 액세스**를 거쳐 2024년 5월 1.0 정식판에 도달했다. 즉 "기획→알파→얼리 액세스→정식"까지 약 7년이 걸린 셈으로, 인디 전략 게임으로서는 상당히 긴 호흡의 프로젝트다.

엔진은 Unity. 흥미로운 점은 순수 픽셀 아트로 출발했다가 개발 도중 2D 스프라이트와 3D 렌더링을 결합한 **2.5D**로 방향을 튼 것인데, 이 기술적 선택이 게임의 비주얼 정체성과 직결된다(3장·5장에서 상술).

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 한 줄 정의

《Songs of Conquest》는 **"맵을 탐험하며 영웅(Wielder)이 군대를 이끌고 자원과 도시를 확보하다가, 적과 마주치면 별도의 헥스(육각형) 전장에서 턴제 전투를 벌이는"** 게임이다. 이 구조는 1990년대 New World Computing의 《Heroes of Might and Magic》(이하 HoMM) 시리즈, 특히 1999년의 《HoMM 3》가 완성한 "어드벤처 맵 + 전술 전투 + 도시 건설"의 3각 구조를 거의 그대로 계승한다. PC Gamer는 이를 두고 "《Heroes of Might and Magic》과 《Total War》를 섞은 것"이라 표현했고, GamesRadar는 "Steam에서 HoMM에 견줄 만하다는 극찬을 받은 4X 택틱스 보석"이라 불렀다.

### 세계관과 톤

배경은 **에리안(Aerea)**이라 불리는 가공의 세계다. 여러 종족·국가가 각자의 신화와 이해관계를 안고 영토와 권력을 놓고 다툰다. 무드는 동화적이면서도 결코 가볍지만은 않은 "다크 판타지의 그림자가 드리운 잔혹동화" 톤이다. 개구리 종족이 노예 상태에서 봉기하거나, 몰락한 영지가 언데드를 일으켜 명맥을 잇는 등, 외형의 귀여움 뒤에 압제·부활·탐욕 같은 무거운 모티프가 깔려 있다.

작가 Kim Tough가 쓴 내러티브는 "팩션마다 한 편씩"이라는 캠페인 구조를 통해 전달된다. 1.0 정식판은 **팩션당 한 편씩, 총 4개의 스토리 캠페인**을 제공하며(얼리 액세스 시점 2편에서 두 편을 추가), 각 레벨이 비교적 길고 후반으로 갈수록 난도가 올라가도록 설계되었다. TheGamer 리뷰는 "공식 캠페인은 충실하고 점점 어려워지며, 흥미로운 캐릭터와 세계·팩션 정보를 제공한다"고 평했다.

### 4대 팩션 — 캐릭터이자 시스템

이 게임에서 "주요 캐릭터"는 개별 영웅이라기보다 **팩션 그 자체**다. 각 팩션이 고유한 미학·서사·플레이스타일을 가진 하나의 인격처럼 기능한다. 정식 출시 시점의 4대 팩션은 다음과 같다(출처: ScreenRant, GameSkinny, Songs of Conquest Wiki).

- **Arleon(아를레온)** — 용맹한 기사·종자·궁수에 숲의 마법 종족 **Faey**가 결합한, 전형적인 인간 왕국. 방어와 원거리 화력에 특화돼 있어 초보자 친화적이지만 숙련 상한도 높다. 주로 **Order(질서)**와 **Chaos(혼돈)** 에센스를 생성하며, 게임 내에서 유일하게 안정적인 Chaos 에센스 확보로 연쇄 번개(Chain Lightning) 빌드를 굴릴 수 있는 팩션으로 꼽힌다.
- **Barony of Loth(로스 남작령)** — 옛 영광을 되찾으려는 몰락한 영지. 미학은 언데드 중심이지만 인간 유닛도 다수 보유하며, **인간 유닛이 죽으면 언데드 'Risen'으로 되살아나** 계속 싸우는 고유 메커니즘이 큰 매력이다. 소모전에서 가장 끈질긴 "지구력의 팩션". 출시 당시 가장 인기 있는 팩션으로 거론되었다.
- **Rana(라나)** — 압제에서 봉기한 비인간 종족. 용·개구리·도마뱀인간·거북 등을 모티프로 한 늪지·부족 문화권. 초반 유닛이 약해 느리게 출발하지만 후반에 강력한 군세로 만개하며, 풍부한 마법 능력 덕에 마법 중심 플레이에 잘 맞는다.
- **Barya(바리아)** — 화약과 기계로 무장한 독립 상인 국가. 옛 아라비아 제국을 비롯한 다양한 문화권 미학을 차용했다. 강력한 근접·포병 유닛으로 정면 충돌에서 압도하지만 방어가 약해 장기 공성전에 취약하다.

(주: 일부 초기 보도는 Doneria 등 다른 명칭을 거론했으나, 정식 출시 기준 4대 팩션은 위 Arleon/Loth/Rana/Barya다. 2024년 12월 'Vanir' DLC, 그리고 이후 'Bleak East' 확장에서 Vanir·Roots 등 신규 팩션이 추가되었다.)

### 아트 디렉션 — "2.5D"의 발견

비주얼은 이 게임을 논할 때 빠질 수 없는 핵심이다. 개발팀은 처음에 **순수주의적 픽셀 아트**로 접근했다가, 작업을 진행하면서 2D와 3D를 섞는 실험을 시작했고, 결국 스스로 이를 **2.5D**라 부르게 되었다(출처: GamesHub, eXplorminate Q&A). 정교하고 유려한 스프라이트 애니메이션 위에, 줌인 시 적용되는 동적 조명과 피사계 심도(DoF) 같은 현대적 렌더링 기법이 얹힌다. 그 결과 "도트의 향수"와 "현대 그래픽의 깊이감"이 공존하는, 동시기 어떤 전략 게임과도 닮지 않은 독특한 룩이 탄생했다. 다수 리뷰가 "픽셀 아트 스타일이 매혹적(mesmerizing)"이라고 표현했다.

### 사운드와 음악 — "정복의 노래"라는 제목값

제목 그대로 음악은 게임의 정체성이다. 작곡가 **Reynir Helgason**의 오리지널 사운드트랙은 평론에서 "captivating(사로잡는다)"으로 반복 언급된다. 특히 PC Gamer는 "미션 사이에 음유시인들이 당신의 모험을 노래로 들려주는 **음악적 막간(musical interludes)**에 마음을 빼앗겼다"며, "게임 안에서 바드가 당신의 여정을 노래하는 일은 무척 드물다"고 평했다. 즉 사운드트랙이 단순 배경이 아니라, 서사 전달의 한 축으로 통합돼 있다는 점이 차별점이다. 오리지널 사운드트랙은 Steam·GOG·Epic 등에서 별도 판매될 만큼 완성도를 인정받았다.

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

이 장이 분석의 핵심이다. 《Songs of Conquest》는 HoMM의 골격을 차용하되, **에센스(Essence) 마법 시스템**이라는 독자적 메커니즘으로 차별화에 성공했다.

### 3-1. 코어 루프 — 어드벤처 맵과 전투의 이중 구조

게임은 두 층위를 오간다.

1. **어드벤처 맵(전략 층)** — 플레이어는 **Wielder(와일더)**라 불리는 영웅을 조종해 맵을 탐험한다. Wielder는 군대를 데리고 다니며 자원 더미를 줍고, 자원 채집지·중립 거점·도시를 점령하고, 퀘스트를 수행하고, 경험치로 성장한다. 이는 HoMM의 "히어로가 맵을 누비는" 그 감각과 사실상 동일하다.
2. **전투(전술 층)** — 적 Wielder나 중립 군세와 부딪치면 화면이 전환되어, **육각형(hex) 타일로 이루어진 별도의 전장**에서 턴제 전투가 벌어진다.

이 두 층위를 매 턴 오가는 리듬이 게임의 모먼트-투-모먼트를 이룬다. 탐험으로 군세를 키우고, 전투로 그 군세를 소모·검증하며, 다시 도시로 돌아와 보충하는 순환이다.

### 3-2. Wielder — 싸우지 않는 영웅

가장 중요한 설계 차이 중 하나는 Wielder의 역할이다. HoMM의 히어로처럼 군대를 이끌고 맵을 다니며 스킬과 군세를 가진다는 점은 같지만, **Wielder는 전투에 직접 참전하지 않는다.** 전장에서 Wielder의 역할은 **주문 시전(spell casting)에 한정**된다(출처: gamepressure). 즉 Wielder는 "물리적 유닛"이 아니라 "전장의 마법 사령탑"이다.

Wielder는 대략 세 가지 아키타입으로 나뉜다. (1) 유닛 버프 중심, (2) 마법 자체를 강화하는 중심, (3) 유틸리티·정찰 중심의 세 번째 유형으로, 이 세 번째 유형은 팩션마다 성격이 미묘하게 달라진다(출처: PC Gamer 분석). 이 구조 덕분에 같은 팩션이라도 어떤 Wielder를 키우느냐에 따라 전혀 다른 운영이 나온다.

### 3-3. 에센스(Essence) — 이 게임의 발명품

《Songs of Conquest》를 다른 HoMM 클론과 구분 짓는 결정적 메커니즘이 바로 **에센스**다. 작동 원리는 다음과 같다(출처: Songs of Conquest Wiki, gamepressure, CulturedVultures 컴뱃 가이드).

- 마나는 영웅 고정 스탯이 아니라, **전투 중 부대(troop)가 생성하는 자원**이다. 각 유닛 스택은 자신의 턴이 끝날 때 정해진 양·종류의 에센스를 생성한다.
- 에센스에는 여러 **타입**이 존재한다(질서 Order, 혼돈 Chaos, 창조 Creation, 파괴 Destruction, 무질서 Arcana 등 — 팩션·유닛마다 생성 타입이 다르다).
- 생성된 에센스는 **풀(pool)에 누적**되며, Wielder는 이 풀을 소비해 주문을 시전한다. 강력한 주문일수록 특정 타입의 에센스가 여러 개 필요하다.

이 설계의 천재성은 **"마법이 군대 구성에 종속된다"**는 점이다. 강한 주문을 쓰고 싶다면, 그 주문에 맞는 타입의 에센스를 생성하는 유닛을 군대에 편성해야 한다. 예컨대 Arleon이 연쇄 번개를 쓰려면 Chaos 에센스를 안정적으로 뽑는 유닛(예: Faey Rager)을 데려가야 한다. 즉 **"어떤 유닛을 데려가는가"가 곧 "어떤 마법을 쓸 수 있는가"를 결정**한다. 군 편성과 마법 전략이 분리되지 않고 하나로 묶이는 이 구조가, 단순한 HoMM 모방을 넘어선 디자인적 독창성의 핵심이다. 여러 리뷰가 "에센스와 유닛 조합의 활용은 독창적이다(unique)"라고 평가했다.

### 3-4. 전투 — 헥스 전장, 지형, 통제 구역

전투는 육각형 타일로 구성된 전장에서 턴제로 진행되며, **낮/밤 주기**의 영향을 받는다(출처: Songs of Conquest Wiki).

- **지형 고저** — 높은 타일에 선 부대는 공격·방어 보너스를 받는다. 고지 선점이 전술의 핵심 변수다.
- **유닛 스택과 상한** — 군대는 독립적으로 행동하는 여러 스택으로 나뉜다. 스택 크기에는 상한이 있어, 한 스택에 무한히 쌓아 단순 물량전으로 가는 것을 막고 전술성을 유지한다.
- **근접 vs 원거리** — 근접 유닛은 인접해야 공격 가능하고, 원거리 유닛은 여러 타일 너머를 친다.
- **통제 구역(Zone of Control)** — 근접 유닛은 인접 헥스에 통제 구역을 행사한다. 적이 이 구역을 통과하려 하면 근접 유닛이 **기회 공격(attack of opportunity)**을 무료로 가한다. 이는 무작정 적 후방 원거리 유닛에게 돌진하지 못하게 막는 위치 게임을 만든다.
- **패시브·액티브 능력** — 모든 유닛은 역할을 정의하는 패시브를 가지며, 일부는 자기 버프·파괴 가능 지형 설치·적 디버프 등 액티브 능력을 가진다.

이 모든 변수—고저, 통제 구역, 에센스 생성 타이밍, 낮/밤—가 맞물려, 표면적 단순함 뒤에 상당한 전술적 깊이를 형성한다.

### 3-5. 진행 구조 — 도시 건설과 경제

전략 층에서는 **도시 건설**이 군세의 토대다. 도시에 건물을 지어 유닛을 해금·생산하고, 경제를 굴린다. 자원 채집지를 확보해 골드와 각종 원자재를 모으고, 이를 도시 업그레이드와 군 보충에 투자하는 4X형 확장 루프가 작동한다. 캠페인은 이 확장을 시나리오 목표·제약과 결합해 단계적으로 가르친다.

### 3-6. 모드: 캠페인, 멀티플레이어, 맵 에디터

1.0 정식판이 제공하는 콘텐츠 폭은 인디 전략 게임 기준으로 후하다(출처: TurnBasedLovers, GameSpace, SteamDeckHQ).

- **캠페인** — 팩션당 1편씩 총 4편. 비교적 긴 레벨로 구성.
- **멀티플레이어** — 로컬·온라인 대전 모두 지원.
- **스커미시 맵** — 출시 직전 9개 맵 추가로 **거의 50개**에 달하는 맵 풀.
- **맵 에디터** — 정식 출시와 함께 대대적 UX 개편을 거쳤다. 패널·도구·속성을 명료하게 재배치해 인터페이스 측면에서 더 나은 에디터를 지향했고, 그 결과 커뮤니티가 커스텀 맵·캠페인을 활발히 제작하는 토대가 되었다.

### 3-7. 난이도·접근성·UI 철학

UI는 "복잡한 시스템을 가능한 한 다가가기 쉽게" 만드는 방향으로 설계되었다. 한 리뷰는 "콘텐츠가 가득하고, 다른 게임들이 도달하지 못한 세련된 광택(polished sheen)이 있으며, 집어 들고 바로 플레이하기 쉽고, 더 복잡한 요소조차 접근 가능하거나 넘어설 만하게 만드는 시스템들이 있다"고 정리했다. 다만 에센스·유닛·업그레이드·주문이 한꺼번에 얽히는 후반부의 학습 곡선은 신규 플레이어에게 부담이 될 수 있다(6장 참조).

---

## 4. 평가

### 4-1. 평론 점수

| 지표 | 점수 / 등급 |
|------|------------|
| Metacritic (PC) | **78 / 100** |
| OpenCritic | **'Strong'**, 평균 **82** (리뷰 13건) |
| Eurogamer | 3 / 5 (≈60) |
| Eurogamer Germany | 80 |
| GRYOnline.pl | 85 |
| Steam 유저 평가 | "Very Positive(매우 긍정적)", 약 87% (리뷰 약 7,000건) |

(출처: [Metacritic](https://www.metacritic.com/game/songs-of-conquest/), [OpenCritic](https://opencritic.com/game/13139/songs-of-conquest), [Steam](https://store.steampowered.com/app/867210/Songs_of_Conquest/))

종합하면 평단 78~82, 유저 87% 수준으로 **평론은 견고하고(Strong) 유저 호응은 더 뜨거운** 전형적 "팬 친화형 양작" 포지션이다.

### 4-2. 주요 평론 인용

- **PC Gamer** — "음악적 막간으로 내 마음을 훔친 훌륭한 택틱스 게임." 에센스·유닛 조합의 독창성과 사운드트랙의 서사 통합을 핵심 강점으로 꼽았다.
- **TechRadar** — 얼리 액세스 시점에 이미 "올해 최고의 전략 게임"이라 평했다. 미완성 상태에서도 완성도가 두드러졌다는 의미다.
- **TheGamer** — "턴제 전략을 향한 찬가를 부르라(Sing The Praises)"는 제목으로, "Lavapotion은 일류 인디 게임을 내놓았고, 어떤 경쟁작보다도 《Heroes of Might & Magic》의 정수를 더 잘 포착했다"고 극찬. 4대 팩션이 거의 완벽하게 밸런스가 잡혀 있고 각자 잘 캐릭터화되어 있다는 점, 방대한 콘텐츠를 강점으로 들었다.
- **GodisaGeek / Gamereactor / eXplorminate** — "픽셀 아트로 빚은 전략 보석", "Heroes of Might and Magic의 재발명", "Lavapotion이 개인적 색채를 솜씨 있게 더한 존경 어린 헌사"로 평가.
- **Eurogamer (3/5)** — 상대적으로 보수적인 평가로, 장르 팬에게는 훌륭하나 장르의 경계를 새로 밀어붙이지는 않는다는 톤(6장에서 상술).

### 4-3. 상업 지표

가장 인상적인 숫자는 **판매량**이다. 2024년 5월, Lavapotion과 Coffee Stain Publishing은 **50만 장 판매**를 공식 발표했다(출처: GodisaGeek, GameWorldObserver, Worthplaying). 8인 규모 스튜디오가 약 2년의 얼리 액세스를 거쳐 도달한 수치라는 점에서 상업적으로 명백한 성공이다. 또한 GameDiscover는 출시 이후 **연간 매출이 꾸준히 성장**해 왔으며, 할인과 신규 콘텐츠가 지속적 판매 모멘텀을 견인했다고 분석한다. 얼리 액세스 단계에서는 GOG.com 2022년 출시작 중 베스트셀러 상위 3위에 들기도 했다.

### 4-4. 수상·노미네이션

정식 출시 이전인 **E3 2021의 PC Gaming Show에서 "Most Anticipated(가장 기대되는 작품)"** 부문에 선정되며 출시 전부터 주목받았다(출처: Wikipedia). 이는 장르 팬덤과 미디어가 출시 한참 전부터 이 게임을 "HoMM의 후계자 후보"로 점찍었음을 보여준다.

### 4-5. 평론-유저 괴리

Metacritic 78 대 Steam 87%의 간극은 전형적이지만 의미가 있다. 평단은 "장르를 새로 정의하지는 않는다"는 점에 점수를 깎는 경향이 있는 반면, **이런 게임을 25년간 기다려온 골수 어드벤처 전략 팬덤은 "내가 원하던 바로 그것"을 만나 더 높은 만족도를 보인다.** 즉 이 게임의 평가 구조 자체가, 그 팬덤을 정확히 겨냥한 제품이라는 정체성을 그대로 반영한다.

---

## 5. 성공 요인 분석 (핵심)

### 5-1. "올바른 영감"을 골랐다 — 죽은 서브장르의 선점

GameDiscover의 분석 제목이 정곡을 찌른다: **"Songs of Conquest는 어떻게 올바른 영감을 골라 50만 장을 팔았나."** 핵심은 **"classic adventure strategy"라는, 사실상 비어 있던 서브장르를 정조준**한 것이다. CEO Magnus Alm의 말: "Lavapotion 창업자 전원이 《HoMM 3》의 열렬한 팬이었다. 우리는 이런 종류의 게임에 헌사를 바치는 무언가를 만들고 싶었다."

《HoMM 3》(1999) 이후, 시리즈는 후속작들의 평가 부침과 IP 부침을 겪었고, 정통 어드벤처 전략의 갈증을 채워줄 신작은 사실상 부재했다. Lavapotion은 이 25년의 공백을 정확히 겨눴다. **수요는 명백히 존재하는데 공급이 끊긴 시장**을 선점한 것—이것이 디자인 이전에 작동한 가장 큰 전략적 결정이다.

### 5-2. 모방이 아니라 "한 가지 발명"을 더했다 — 에센스 시스템

단순한 헌사로 그쳤다면 "괜찮은 HoMM 클론" 이상이 되지 못했을 것이다. 결정적 차별화는 **에센스 마법 시스템**(3-3 참조)이다. 마법 자원을 영웅 스탯에서 떼어내 군대 구성에 종속시킴으로써, 군 편성·마법·전술이 하나의 의사결정으로 통합되는 새로운 깊이를 만들었다. "친숙한 골격 + 한 가지 강력한 신규 메커니즘"은 장르 부활작의 모범 공식이며, 이 게임은 그것을 정확히 실행했다.

### 5-3. 비주얼·음악이라는 즉각적 차별점

2.5D 픽셀 아트와 Reynir Helgason의 사운드트랙은 트레일러·스크린샷만으로도 "이 게임 뭐지?"를 유발하는 즉각적 후크였다. 특히 음악적 막간은 "Songs of Conquest"라는 제목값을 실제 메커니즘으로 구현해, 마케팅 메시지와 제품 경험이 일치하는 보기 드문 사례를 만들었다. 비주얼과 음악은 위시리스트 전환의 강력한 동력이었다.

### 5-4. 얼리 액세스 운영의 모범 — "거의 매월 업데이트"

상업적 성공의 운영적 토대는 **꾸준한 얼리 액세스 관리**다. GameDiscover에 따르면 Lavapotion은 1.0까지 **"거의 매월" 업데이트**를 이어갔다. 2019~2021년 이미 2만 명 이상의 클로즈드 알파 신청을 모았고, Discord·공식 블로그로 커뮤니티와 지속 소통했다. 이 "신뢰의 누적"이 얼리 액세스 매출, 입소문, 1.0 출시 모멘텀으로 복리처럼 불어났다.

### 5-5. 퍼블리셔 선택 — Coffee Stain Publishing

《Satisfactory》·《Goat Simulator》·《Valheim》(퍼블리싱) 등으로 인디 히트 제조 노하우를 쌓은 **Coffee Stain Publishing**과의 협업은 마케팅·플랫폼·로드맵 측면에서 작은 팀의 약점을 보완했다. 같은 스웨덴 기반이라는 점도 협업 효율을 높였을 것이다.

### 5-6. 명확한 타깃과 "evergreen" 전략

Magnus Alm은 목표를 "**무료 업데이트와 DLC로 아주 오래 살아남는 에버그린 타이틀**"로 명시했다. 실제로 2024년 12월 'Vanir' DLC, 이후 콘솔·모바일·Switch 다중 플랫폼 전개, 'Bleak East' 확장(Vanir·Roots 신규 팩션) 등으로 생명주기를 늘려가며, "출시가 끝이 아니라 시작"이라는 현대 인디의 장기 운영 모델을 충실히 따른다.

### 5-7. 동시기 작품 대비 차별점

같은 시기 전략·택틱스 시장에는 여러 강자가 있었지만, **"정통 HoMM식 어드벤처 전략 + 독자 마법 시스템 + 2.5D 아트 + 서사형 음악"의 조합을 모두 갖춘 작품은 사실상 이것뿐**이었다. 경쟁이 아니라 공백을 정확히 메운 포지셔닝이 핵심 차별점이다.

---

## 6. 비평적 시각 / 한계 / 논란

극찬 일색은 아니다. 평단 78점이라는 숫자가 가리키는 약점들이 분명히 있다.

### 6-1. 학습 곡선과 신규 진입 장벽

가장 자주 지적되는 약점은 **복잡성**이다. 에센스·유닛·업그레이드·주문이 한꺼번에 얽히면, 게임을 배우기가 만만치 않다. TurnBasedLovers 1.0 리뷰는 "에센스와 유닛 조합의 사용은 독창적이지만, 시너지를 찾기 어려운 신규 플레이어에게는 부담스러울 수 있다(daunting)"고 짚었다. 강점인 에센스 시스템이 동시에 진입 장벽이라는 양날의 검이다.

### 6-2. 캠페인 난이도 곡선

여러 리뷰가 **캠페인 난이도 곡선의 불균형**을 지적한다. 특정 구간에서 난도가 급격히 튀거나 고르지 못하다는 불만이다. TheGamer 역시 "싱글플레이어 캠페인에 몇 가지 결함이 있다"고 인정하면서도 전반적 완성도는 높게 평가했다.

### 6-3. UI·조작의 사소한 불편

전장이나 맵의 일부 지점에서 **클릭이 까다로운(finicky)** 순간이 있다는 지적이 있다. 좁은 통로를 지나가게 할 때 특히 그렇다. 치명적 결함은 아니지만 매끄러움을 해치는 마찰 요소다.

### 6-4. "장르의 경계를 넓히지는 않는다"

가장 본질적인 비평은 야심의 범위다. Eurogamer가 3/5에 그친 이유이기도 한데, **이 게임은 자기가 어떤 게임인지·누구를 위한 게임인지 정확히 알지만, 장르의 경계를 새로 밀어붙이지는 않는다.** 기존 팬에게는 탁월한 선택이지만, "혁신"을 기대하는 평론가에게는 보수적으로 비친다. 강점(헌사)과 약점(헌사에 머묾)이 동전의 양면이다.

### 6-5. 큰 논란은 없었다

주목할 점은, 약탈적 MTX·론칭 참사·운영 스캔들 같은 **큰 논란이 사실상 없었다**는 것이다. 정공법 패키지 게임에 정직한 DLC·무료 업데이트 모델을 택했고, 얼리 액세스 약속을 성실히 지켰다. "조용하지만 신뢰받는 출시"는 그 자체로 이 게임의 미덕이다.

---

## 7. 영향과 유산

### 7-1. "어드벤처 전략 부활"의 깃발

《Songs of Conquest》의 가장 큰 의미는, **HoMM식 어드벤처 전략이 여전히 상업적으로 유효한 장르임을 50만 장으로 입증**했다는 점이다. 오랫동안 "틈새·향수"로 치부되던 서브장르가, 정공법으로 잘 만들면 충분한 시장이 있다는 증거가 되었다. 이는 후발 인디·중견 개발사에 "잊힌 클래식 장르를 현대적으로 되살리기"의 강력한 레퍼런스로 작동한다.

### 7-2. 에센스 시스템 — 디자인 레퍼런스

군 편성과 마법 자원을 결합한 에센스 시스템은, "친숙한 장르에 단 하나의 구조적 발명을 더해 차별화한다"는 디자인 교훈의 모범 사례로 인용될 만하다. 향후 유사 장르 게임이 "마법 자원을 어떻게 설계할 것인가"를 고민할 때 비교 대상이 될 것이다.

### 7-3. 인디 운영 방법론의 사례

8인 규모 팀이 (1) 명확한 타깃 장르 선점, (2) 한 가지 핵심 발명, (3) 강력한 비주얼·음악 후크, (4) 거의 매월 얼리 액세스 업데이트, (5) 검증된 퍼블리셔 협업, (6) 다중 플랫폼·DLC 에버그린 전개로 성공을 빚어낸 과정은, 소규모 인디 전략 게임의 사업·운영 교본에 가깝다.

### 7-4. 다중 플랫폼 확장

정식 출시 후 콘솔(PS5, Xbox Series, 2024년 11월) → 모바일(iOS/Android, 2025년 3월) → Nintendo Switch(2025년 6월)로 이어진 플랫폼 확장은, 턴제·헥스 기반 어드벤처 전략이 터치·핸드헬드 환경에도 잘 이식될 수 있음을 보여주며 장르의 도달 범위를 넓혔다. GamesRadar는 모바일 진출 발표를 "Steam에서 HoMM에 견줄 만하다는 극찬을 받은 4X 택틱스 보석"이라는 표현으로 다뤘다.

### 7-5. 문화적 의미 — "헌사가 원작을 넘본다"

여러 평론이 공통적으로 "Lavapotion이 《HoMM》의 정수를 어떤 경쟁작보다 잘 포착했다"고 평가했다는 점은 의미심장하다. 헌사로 출발한 작품이, 원작 IP의 부진 속에서 사실상 **장르의 현역 대표주자 지위를 물려받은** 보기 드문 사례다. 이는 IP가 식어도 그 게임이 준 경험에 대한 수요는 죽지 않는다는, 게임 문화의 한 단면을 보여준다.

---

## 8. 부록

### 8-1. 핵심 통계 표

| 항목 | 수치 / 내용 |
|------|------------|
| 개발사 규모 | 초기 4명 → 얼리 액세스 시 약 8명 |
| 개발 시작 | 2017년 (스튜디오 설립과 함께) |
| 클로즈드 알파 신청 | 2만 명 이상 (2019~2021) |
| 얼리 액세스 | 2022년 5월 10일 |
| 정식 출시 | 2024년 5월 20일 |
| 판매량 | 50만 장 (2024년 5월 기준) |
| Metacritic | 78 / 100 (PC) |
| OpenCritic | 'Strong', 평균 82 |
| Steam 유저 평가 | Very Positive, 약 87% (리뷰 약 7,000건) |
| 정식판 팩션 수 | 4 (Arleon, Barony of Loth, Rana, Barya) |
| 정식판 맵 수 | 약 50개 |
| 캠페인 | 팩션당 1편, 총 4편 |
| 엔진 | Unity |
| 퍼블리셔 | Coffee Stain Publishing |

### 8-2. 주요 인터뷰·심층 자료

- GameDiscover — "How Songs Of Conquest chose the right inspiration & sold 500k!" (Magnus Alm 인용, 개발 규모·운영 분석): https://newsletter.gamediscover.co/p/how-songs-of-conquest-chose-the-right
- GameRant — "Songs of Conquest Interview: Lavapotion Designer Talks Early Access, Future Plans" (Carl Toftfelt): https://gamerant.com/songs-of-conquest-interview-carl-toftfelt-history-early-access-development/
- eXplorminate — "Songs of Conquest Q&A" (아트 디렉션·2.5D 결정): https://explorminate.org/songs-of-conquest-qa/
- PC Gamer — "Songs of Conquest is a mix of Heroes of Might and Magic and Total War": https://www.pcgamer.com/songs-of-conquest-is-a-mix-of-heroes-of-might-and-magic-and-total-war/

### 8-3. 주요 평론·기사

- Metacritic: https://www.metacritic.com/game/songs-of-conquest/
- OpenCritic: https://opencritic.com/game/13139/songs-of-conquest
- TheGamer 리뷰: https://www.thegamer.com/songs-of-conquest-review/
- PC Gamer — "stole my heart with musical interludes": https://www.pcgamer.com/songs-of-conquest-is-a-great-tactics-game-that-stole-my-heart-with-musical-interludes/
- TechRadar — "best strategy game of the year so far": https://www.techradar.com/features/you-need-to-play-this-new-strategy-game-even-though-its-not-finished
- eXplorminate 리뷰 — "A Reinvention of Heroes of Might and Magic": https://explorminate.org/songs-of-conquest-a-review/
- GodisaGeek — 50만 장 판매·로드맵: https://www.godisageek.com/2024/05/songs-of-conquest-has-now-sold-500000-units-post-launch-roadmap-revealed/
- TurnBasedLovers — 1.0 리뷰: https://turnbasedlovers.com/review/songs-of-conquest-1-0-impressions/

### 8-4. 시스템·세계관 레퍼런스

- Songs of Conquest Wiki — Magic / Combat: https://songsofconquest.fandom.com/wiki/Magic , https://songsofconquest.fandom.com/wiki/Combat
- gamepressure — Wielders and spells: https://www.gamepressure.com/songs-of-conquest/wielders-and-spells/z4fc74
- ScreenRant — Every Playable Character & Faction At Launch: https://screenrant.com/songs-of-conquest-playable-factions-barony-lolth-arleon/
- GameSkinny — All Factions Explained: https://www.gameskinny.com/tips/all-songs-of-conquest-factions-explained/
- CulturedVultures — Combat Guide (Terrain, Magic, Troops): https://culturedvultures.com/songs-of-conquest-combat-guide-terrain-magic-troops/
- Wikipedia: https://en.wikipedia.org/wiki/Songs_of_Conquest

### 8-5. 공식

- 공식 사이트: https://www.songsofconquest.com/
- 개발사: https://www.lavapotion.com/
- Steam: https://store.steampowered.com/app/867210/Songs_of_Conquest/

---

*본 분석서는 2026년 6월 기준 영어권 공개 자료(Metacritic, OpenCritic, PC Gamer, TheGamer, TechRadar, eXplorminate, GameDiscover, GameRant, Wikipedia, 공식 위키 등)를 토대로 작성되었다. 판매량·점수 등 수치는 출처 발표 시점 기준이며, 이후 변동될 수 있다.*
