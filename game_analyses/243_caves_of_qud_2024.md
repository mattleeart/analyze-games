# Caves of Qud (2024) 심층 분석

> 17년의 개발, 9년의 얼리 액세스를 거쳐 마침내 1.0으로 도착한 과학 판타지 로그라이크. 2024년 OpenCritic 최고 평점 게임이자, "절차적 시뮬레이션이 곧 서사가 될 수 있다"는 명제를 가장 멀리 밀어붙인 작품.

---

## 1. 게임 개요

《Caves of Qud》는 미국의 초소형 인디 스튜디오 **Freehold Games**가 개발하고 **Kitfox Games**가 퍼블리싱한 로그라이크 RPG다. 두 공동 창립자 **Brian Bucklew**(프로그래밍·시스템 설계)와 **Jason Grinblat**(서사·월드 디자인)이 2007년부터 함께 만들기 시작했고, Freehold Games 법인은 2013년 3월 1일 공식 설립됐다. 첫 공개 베타는 2010년, Steam 얼리 액세스는 2015년 7월, 그리고 **1.0 정식 출시는 2024년 12월 5일**이다. Nintendo Switch 이식판은 2026년 2월 16일에 나왔다. (출처: [Wikipedia](https://en.wikipedia.org/wiki/Caves_of_Qud))

- **개발사**: Freehold Games (미국)
- **퍼블리셔**: Kitfox Games — 2023년 7월 1.0 퍼블리싱 계약 발표. Kitfox는 《Dwarf Fortress》 스팀판을 결승선까지 끌고 간 퍼블리셔로, 같은 계보의 "심층 시뮬레이션" 게임을 다룬다는 점에서 상징적인 조합이었다. ([PC Gamer](https://www.pcgamer.com/dwarf-fortresss-publisher-is-now-helping-the-best-early-access-roguelike-across-the-finish-line-after-8-years-on-steam/))
- **장르**: 로그라이크 / 롤플레잉, 과학 판타지(science fantasy), 포스트아포칼립스. 싱글플레이 전용.
- **플랫폼**: Windows, macOS, Linux, Nintendo Switch
- **엔진**: Unity
- **주요 크레딧**: 디자인 — Brian Bucklew, Jason Grinblat, Caelyn Sandel, Nick DeCapua / 아트 — Samuel Wilson, Cyril van der Haegen / 음악 — Craig(ory) Hamilton, Brandon Tanner
- **개발 기간/규모**: 2007년 발상, 약 17년에 걸친 제작. 얼리 액세스만 약 9년(2015–2024). 정규 인력 한 자릿수의 초소형 팀.

이 게임을 이해하는 가장 중요한 한 줄은 "개발 기간"이다. 17년이라는 시간은 단순한 지연이 아니라 설계 철학의 결과였다. Bucklew와 Grinblat은 인터뷰에서 "최대 수익보다는 긍정적인 라이프스타일과 좋은 게임"을 우선했다고 밝혔고, 그 결과 9년의 얼리 액세스 동안 거의 매달 패치를 내며 게임을 천천히 키웠다. 영향원으로는 고전 로그라이크 《ADOM》, 테이블탑 RPG 《Gamma World》와 《Dungeons & Dragons》, 그리고 무엇보다 《Dwarf Fortress》가 거론된다.

---

## 2. 게임 설명 — Qud라는 세계

### 무대와 시간대

《Caves of Qud》의 배경은 **Qud**라는 거대한 메사(mesa) 지대다. 무성한 정글과 고대 폐허가 뒤엉켜 있고, 북쪽의 거대한 산맥이 Svy·Opal·Yonth 세 강을 먹여 살린다. 그 한복판에는 하늘로 솟은 사이클롭스적 우주 엘리베이터 **the Spindle**이 박혀 있다. 남동쪽에는 유기 생명이 살 수 없는 불모의 **Deathlands**(죽음의 땅)가 펼쳐져 고대의 미친 기계들만이 움직이고, 서쪽에는 **Great Salt Desert**(대염사막)를 둘러싼 얕은 늪지가 있다. ([TV Tropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/CavesOfQud))

플레이어는 **Sultanate**(술탄국)가 멸망한 지 **1000년 후**의 시점에서 게임을 시작한다. Sultanate는 Qud 대부분을 지배했던 마지막 대문명으로, **Resheph**라는 인물이 이를 해체하면서 무너졌다. 그러나 그 이전에는 더 오래된 **Eaters of Earth**(대지를 먹는 자들)가 있었다. 이들은 성간 여행이 가능했던 초고도 문명으로, 술탄들의 유물과 sultan masks 같은 경이로운 물건들을 남겼다. 흥미로운 점은, 게임의 로어를 파고들수록 이 문명이 Resheph 이전부터 이미 가파른 쇠퇴에 들어서 있었다는 힌트가 드러난다는 것이다 — 즉 Qud는 "한 번의 멸망"이 아니라 "겹겹이 쌓인 멸망의 지층" 위에 서 있는 세계다. ([Wiki: Eaters](https://wiki.cavesofqud.com/wiki/Eaters))

### 무드/톤/아트 디렉션

비주얼은 ASCII 글리프 기반(타일셋 옵션 제공)의 레트로 미감을 고수한다. 그러나 단순한 향수가 아니라, 광대한 절차적 세계를 표현하기 위한 의도적 선택이다. 톤은 신비주의적이고 생물학적으로 그로테스크하다. 플레이어는 식물성 인간, 정신감응 능력자, 곤충 떼와 대화하는 자가 될 수 있고, 적의 팔다리를 잘라내거나 클론을 만들거나 몬스터를 정신 지배할 수 있다. 이 "anything goes" 무드는 Gamma World 식 핵폭발 이후 변이 생태계와 D&D식 던전 탐험을 한 그릇에 담은 결과다.

### 캐릭터/NPC와 사운드

고정 시작 마을 **Joppa**의 NPC들(예: 신성한 물을 다루는 인물들, 의뢰를 주는 마을 주민들)은 수공으로 제작돼 일관된 정체성을 갖는다. 반면 다른 마을의 인물들은 절차적으로 생성된다. 음악은 **Craig Hamilton**과 **Brandon Tanner**가 맡았다. 공식 사운드트랙은 32트랙·2시간 분량에 이르며(초기에는 14트랙으로 발표), 일부 트랙은 하루의 시간대·계절·습격(raid) 같은 맥락에 따라 다르게 재생되어 세계의 분위기를 입체적으로 만든다.

---

## 3. 핵심 시스템 / 메카닉

《Caves of Qud》의 진짜 정체성은 "콘텐츠"가 아니라 "시스템"에 있다. 거의 모든 것이 절차적으로 생성되고, 거의 모든 것이 서로 상호작용한다.

### 2단계 캐릭터 생성 — Mutant vs True Kin

캐릭터 생성은 두 갈래의 **genotype**에서 출발한다. ([TheGamer 가이드](https://www.thegamer.com/caves-of-qud-character-creation-guide/), [Wiki: True Kin](https://wiki.cavesofqud.com/wiki/True_Kin))

- **Mutated Human(돌연변이 인간)**: 스탯 분배 포인트를 **44점** 받는다. 70종 이상의 **Mutations**(돌연변이)를 보유·획득하며, 이는 신체 변형형(**Chimera**, 물리)과 정신능력형(**Esper**, 정신)으로 나뉜다. 돌연변이는 경험치를 쌓으면 레벨이 올라 패시브 스탯 보너스나 발동형 능력을 강화한다. 물리 돌연변이에는 **rapid advancement**라는 고유 메커니즘이 있어, 플레이어 레벨 5부터 이후 10레벨마다 게놈이 "흥분 상태"에 진입해 한 물리 돌연변이를 영구적으로 +3 강화할 기회를 준다.
- **True Kin(순혈 인류)**: 스탯 포인트를 **38점**으로 더 적게 받지만, 돌연변이가 없는 대신 선택한 **Caste**에서 더 큰 보너스를 받고, 레벨업 시 스킬 포인트를 더 많이 얻는다. 돌연변이 대신 **Cybernetics**(사이버네틱스)를 단 1개로 시작해, 탐험 중 발견한 것을 직접 설치한다. 사이버네틱스는 돌연변이보다 다소 강력하지만 직접 찾아야 한다.

각 genotype은 12개의 세부 분류를 갖는다 — 돌연변이는 **calling**, True Kin은 **caste**다. True Kin의 caste는 세 대형 아콜로지(arcology) 중 하나에 속한다: 성도 **Ekuemekiyye**(추가 출혈 저항), 빙결 도시 **Ibul**(탁월한 냉기 저항), **Yawningmoon**(탁월한 열 저항). 이 한 번의 선택이 시작 스탯·스킬·장비를 좌우하므로, 캐릭터 빌드는 사실상 게임 시작 전부터 시작된다.

### 절차적 역사 시스템 — 게임의 심장

Qud를 다른 로그라이크와 결정적으로 가르는 것이 **절차적 역사 생성**이다. 새 게임을 시작할 때마다 세계는 **5명의 절차적 술탄**의 통치기를 생성한다. 각 술탄에게는 이름, 생애의 사건들, 단편적 로어, 반복되는 테마가 모두 절차적으로 부여된다. 여기에 **6번째 술탄 Resheph**는 모든 플레이마다 고정으로 등장하며 항상 같은 로어를 갖는다. ([Wiki: World generation](https://wiki.cavesofqud.com/wiki/World_generation), [Wiki: Sultan histories](https://wiki.cavesofqud.com/wiki/Sultan_histories))

생성 순서가 핵심이다. 게임은 먼저 한 통치기에 해당하는 **지역과 장소**를 만든 뒤, 그 지역·장소(그리고 이전 통치기들의 것)를 **맥락(context)**으로 삼아 그 시대의 역사를 생성한다. 1대부터 5대 술탄은 각각 **10~22개(보통 11~14개)**의 사건을 역사에 갖는다. 첫 사건은 보통 술탄의 기원(후계자로 태어났거나 갓난아기로 발견됨)을 다룬다. 이렇게 만들어진 "신화적 전기(mythic biography)"는 게임 안의 유물·비석·역사 유적·sultan cult(술탄 숭배) 등에 흩뿌려져, 플레이어가 세계를 탐험하며 직접 짜맞추게 된다. 이 설계는 Grinblat이 2017년 발표한 연구 ["Subverting the Trope of the Heroic Biography"](https://www.pcgworkshop.com/archive/grinblat2017subverting.pdf)에 정리돼 있다.

이는 명백히 《Dwarf Fortress》의 역사 시스템에서 빌려온 것이다. Grinblat은 "Caves of Qud만큼 큰 영향을 받은 게임은 거의 없다(Few games have had as big an impact on Caves of Qud as DF)"고 말했다. 특히 역사가 "구전과 고대 문헌" 같은 역사적 기록을 통해 전해진다는 발상 — 즉 **편향과 상충하는 시점을 허용한다**는 점이 핵심이다. ([PC Gamer 라운드테이블](https://www.pcgamer.com/dwarf-fortress-and-caves-of-qud-roundtable-the-masters-of-simulation-talk-roguelikes-ai-and-making-the-infinite-compelling/))

### 월드맵과 절차 생성 기술

맵은 세 종류가 섞여 있다: (1) **고정**(Joppa 같은 수공 마을), (2) **완전 절차**(몬스터 소굴, 숨겨진 폐허), (3) **반절차**(항상 같은 위치지만 좌판·사람·상품이 매번 바뀌는 시장). 절차 생성의 기술적 깊이도 상당하다. Bucklew는 Roguelike Celebration 2019에서 **Wave Function Collapse** 알고리즘을 활용한 맵 생성을 강연했고, Bucklew와 Grinblat은 [GDC 강연](https://www.gdcvault.com/play/1026313/Math-for-Game-Developers-End)에서 마을을 그 자체의 역사·문화·건축 양식·이야기 전통·NPC·퀘스트와 함께 end-to-end로 생성하는 시스템을 시연했다.

### 코어 게임플레이 루프와 깊은 시뮬레이션

모먼트-투-모먼트 플레이는 턴제 그리드 탐험·전투다. 그러나 그 위에 **깊이 시뮬레이션된 물리·정치 시스템**이 얹혀 있어, 신체 부위 절단, 복제(클론), 정신 지배 같은 상호작용이 시스템 차원에서 결과를 낳는다. 화염은 번지고, 액체는 흐르고, 가스는 퍼진다. 이 "물질이 진짜처럼 행동하는" 시뮬레이션이 PC Gamer가 "내가 플레이해본 최고의 세계 시뮬레이션(the best one I've ever played)"이라 부른 근거다.

### 영구사망과 접근성

전통 로그라이크의 **영구사망(permadeath) 클래식 모드**와 함께, 체크포인트·세이브를 허용하는 **Roleplay 모드**를 제공해 진입 장벽을 낮췄다. PC Gamer는 이 게임이 동류 작품 중 "가장 현대적인 인터페이스와 조작(the best, most modern interface and controls in a game of its kind)"을 가졌다고 평했는데, ASCII 로그라이크에 대한 통념을 뒤집는 평가다.

---

## 4. 평가

### 종합 점수와 GOTY

1.0 출시 후 《Caves of Qud》는 평론가들의 "보편적 호평(universal acclaim)"을 받았다.

- **Metacritic**: 91/100 ([Metacritic](https://www.metacritic.com/game/caves-of-qud/))
- **OpenCritic**: 평점 95%, 추천율 100%. 그리고 **OpenCritic의 2024년 최고 평점 게임(올해의 게임)**으로 선정됐다. 《Hades II》, 《Balatro》, 《Satisfactory》를 모두 제친 결과다. ([PCGamesN](https://www.pcgamesn.com/caves-of-qud/open-critic-highest-rated))

### 주요 매체 리뷰

| 매체 | 점수 | 핵심 평 |
|---|---|---|
| PC Gamer (US) | 94% | "플레이·스토리·롤플레잉 자유에서 장르를 규정하는 성취(a genre-defining achievement in play, story, and roleplaying freedom)" |
| Eurogamer | 5/5 | 최고 등급 추천 |
| Edge | 8/10 | — |

PC Gamer의 Jonathan Bolding은 인터페이스와 조작을 극찬하고 세계 시뮬레이션을 "내가 플레이해본 최고"라 평했으며, PC Gamer는 이 게임을 **2024 올해의 로그라이크**로 선정하며 "불가능할 만큼 독창적인 레트로퓨처리즘 판타지"라 불렀다. ([PC Gamer 리뷰](https://www.pcgamer.com/games/roguelike/caves-of-qud-review/), [Best Roguelike 2024](https://www.pcgamer.com/games/roguelike/best-roguelike-2024-caves-of-qud/))

### 수상 이력

- **2025 Independent Games Festival (IGF)**: Excellence in Narrative 수상
- **2025 Hugo Award**: Best Game or Interactive Work 수상 — SF·판타지 문학계 최고 권위 상에서의 수상은, 이 게임의 서사가 게임계를 넘어 인정받았음을 보여준다
- **2024 D.I.C.E. Awards**: Strategy/Simulation Game of the Year 노미네이트
- **2025 Golden Joystick Awards**: Best Indie Game 노미네이트

### 상업 지표

SteamSpy 기준 Steam 소유자는 약 **20만~50만 명**으로 추정되며, 한 매출 추정 도구는 출시 이후 총매출을 약 **$10.1M**(약 100억 원)으로 본다. 출시 직후 스팀 평가는 "압도적으로 긍정적(Overwhelmingly Positive)"으로, 한 보도 시점 기준 약 11,985개 리뷰가 집계됐다. ([SteamSpy](https://steamspy.com/app/333640))

Freehold의 Brian Bucklew는 "우리가 기대했던 그 무엇보다 **100배 더 잘됐다**(100x better than anything we ever expected)"고 말했다. 그는 "대부분의 게임은 첫날 많이 팔리고 예측 가능하게 하락하지만" Qud는 그렇지 않았다며, 9년 얼리 액세스 누적 위에 1.0이 다시 큰 부스트를 준 비전형적 판매 곡선을 강조했다. ([GamesRadar](https://www.gamesradar.com/games/roguelike/after-thousands-of-overwhelmingly-positive-steam-reviews-caves-of-qud-dev-says-the-roguelike-rpg-has-done-100x-better-than-anything-we-ever-expected/))

### 평론-유저 괴리

이 작품은 평론과 유저의 방향이 거의 일치한다(둘 다 압도적 호평). 다만 그 호평이 "모두에게"가 아니라 "이 깊이를 감당할 의지가 있는 사람에게"로 자기 선택(self-selection)된다는 점이 특징이다. 즉 점수는 높지만, 그 점수를 매긴 모집단은 이미 하드코어 로그라이크에 호의적인 쪽으로 걸러져 있다.

---

## 5. 성공 요인 분석

### (1) 디자인 — "콘텐츠가 아니라 시스템을 만든다"

Qud의 성공은 절차적 시스템에 대한 우직한 투자에서 나왔다. 술탄 역사, Wave Function Collapse 맵, 마을의 문화·건축까지 절차 생성하는 설계는, 한정된 인력으로 사실상 무한에 가까운 콘텐츠를 만들어내는 레버리지였다. 작은 팀이 17년 동안 "콘텐츠를 손으로 채우는" 대신 "콘텐츠를 만드는 시스템을 다듬는" 데 시간을 쓴 결과, 다른 어떤 인디도 흉내 내기 어려운 깊이가 쌓였다.

### (2) 9년 얼리 액세스 운영 방법론

거의 매달 패치를 내며 커뮤니티와 함께 성장한 9년은 단점이 아니라 자산이었다. 출시 시점에 게임은 이미 검증된 충성 플레이어층과 방대한 콘텐츠를 갖고 있었고, 1.0은 그 위에 "완성"이라는 신호를 더해 신규 유입을 폭발시켰다. "최대 수익이 아니라 좋은 라이프스타일과 좋은 게임"이라는 철학이 역설적으로 상업적 성공을 낳은 셈이다.

### (3) 접근성과 현대적 UX

ASCII 로그라이크는 진입 장벽으로 악명 높지만, Qud는 타일셋·현대적 UI·Roleplay 모드·향상된 조작으로 그 벽을 낮췄다. PC Gamer가 "동류 최고의 인터페이스"라 평한 것은, 깊이를 희생하지 않으면서 더 넓은 청중에게 도달했다는 증거다.

### (4) 퍼블리셔 파트너십과 타이밍

2023년 **Kitfox Games**와의 파트너십은 마케팅·출시 운영의 전문성을 더했다. 《Dwarf Fortress》 스팀판을 성공시킨 퍼블리셔라는 점이 "심층 시뮬레이션 게임"이라는 정체성과 완벽히 맞아떨어졌다. 또한 2024년은 《Balatro》, 《Hades II》 등 인디 로그라이크/덱빌더가 평단의 주목을 받던 해였고, Qud는 그 한복판에서 "가장 깊은" 포지션을 차지했다.

### (5) 동시기 작품 대비 차별점

《Hades II》가 연출·내러티브의 완성도로, 《Balatro》가 중독적 단순함으로 승부했다면, Qud의 차별점은 **세계 자체의 절차적 생명력**이었다. 매 플레이마다 다른 역사를 가진 세계를 탐험한다는 경험은 다른 어느 경쟁작도 제공하지 못했다.

---

## 6. 비평적 시각 / 한계 / 논란

### 진입 장벽과 정보 과부하

접근성을 크게 개선했음에도, Qud는 여전히 매우 어려운 게임이다. 압도적인 시스템 수, 방대한 돌연변이·아이템·로어, 가혹한 영구사망은 다수의 캐주얼 플레이어를 튕겨낸다. 얼리 액세스 시절 일부 평가는 인터페이스가 여전히 혼란스럽다고 지적했다. 즉 "역대 최고 평점"이라는 타이틀의 모집단은 이미 이 장르에 헌신한 사람들로 자기 선택돼 있다.

### 절차적 서사의 양날

절차적 역사·마을은 무한한 다양성을 주지만, 동시에 손으로 쓴 서사가 주는 "작가적 응집력"은 약해질 수밖에 없다. 절차 생성된 술탄 전기는 신비롭지만 때로 무작위적·반복적으로 느껴질 수 있고, 모든 세부가 동등한 무게로 의미 있는 것은 아니다. 시스템이 만들어내는 이야기를 "의미"로 읽어내는 것은 상당 부분 플레이어의 몫이며, 이는 《Dwarf Fortress》가 안고 있는 것과 같은 구조적 긴장이다.

### 17년이라는 시간의 의미

상업적으로 성공했지만, 한 게임에 17년을 쓰는 개발 모델은 일반화할 수 없다. 이는 두 창립자의 특수한 라이프스타일 선택의 결과이지, 재현 가능한 비즈니스 전략이 아니다. "천천히, 오래"가 통한 것은 절차 생성이라는 레버리지와 결합됐기 때문이다.

---

## 7. 영향과 유산

### 장르적 위치 — DF 계보의 RPG적 완성

《Caves of Qud》는 《Dwarf Fortress》가 개척한 "절차적 역사·시뮬레이션이 곧 서사"라는 계보를, **싱글플레이 RPG**라는 더 접근하기 쉬운 그릇에 담아 완성도 높게 보여줬다. DF가 "수백 드워프의 정착지를 운영·방어"하는 게임이라면, Qud는 "한 캐릭터로 깊은 RPG를 살아내는" 게임이다. 두 작품은 PC Gamer의 합동 라운드테이블에서 "시뮬레이션의 거장들"로 함께 묶였다. ([PC Gamer 라운드테이블](https://www.pcgamer.com/dwarf-fortress-and-caves-of-qud-roundtable-the-masters-of-simulation-talk-roguelikes-ai-and-making-the-infinite-compelling/))

### 산업적 의미

Qud의 성공은 두 가지 메시지를 업계에 던졌다. 첫째, **얼리 액세스를 "출시 후 마케팅"이 아니라 "장기 공동 개발"로 진지하게 운영하면** 작은 팀도 거대한 깊이를 쌓을 수 있다. 둘째, **절차 생성은 콘텐츠 부족의 임시방편이 아니라, 그 자체로 게임의 핵심 미학이자 경쟁력**이 될 수 있다. 이는 후속 인디 시뮬레이션·로그라이크 개발자들에게 강력한 레퍼런스가 된다.

### 문화적 의미

2025년 **Hugo Award**(Best Game or Interactive Work) 수상은 특히 상징적이다. 게임의 절차적 서사가 SF·판타지 문학계의 최고 권위 상에서 인정받았다는 것은, "기계가 생성한 신화"도 진지한 서사 예술로 다뤄질 수 있음을 보여준다. IGF의 Excellence in Narrative 수상 역시 같은 맥락이다 — 작가가 한 줄 한 줄 쓰지 않은 서사가 "내러티브 우수성"으로 표창받은 드문 사례다.

### 모방과 확장

절차적 역사 생성과 깊은 시뮬레이션의 결합은 이후 인디 RPG/로그라이크가 참조하는 패턴이 되고 있다. Freehold는 Switch 이식과 확장 콘텐츠를 통해 IP를 이어가고 있으며, Bucklew는 "불가능해 보이는 문제를 푸는 것에 관심이 있다"며 추가 개발 의지를 밝혔다. ([RPG Site 인터뷰](https://www.rpgsite.net/interview/20000-brian-bucklew-caves-of-qud-interview-expansions-switch-port-unity-controller-support-coffee))

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
|---|---|
| 개발사 / 퍼블리셔 | Freehold Games / Kitfox Games |
| 발상 / EA / 1.0 | 2007 / 2015-07 / 2024-12-05 |
| Switch 이식 | 2026-02-16 |
| 엔진 | Unity |
| Metacritic | 91/100 |
| OpenCritic | 95% (추천 100%), 2024 최고 평점 게임 |
| PC Gamer (US) | 94% |
| Eurogamer / Edge | 5/5 / 8/10 |
| Steam 평가 | 압도적으로 긍정적 |
| Steam 소유자(추정) | 20만~50만 |
| 총매출(추정) | 약 $10.1M |
| 주요 수상 | IGF Excellence in Narrative(2025), Hugo Best Game(2025) |
| 돌연변이 수 | 70종 이상 |
| 절차적 술탄 | 5명(절차) + Resheph(고정), 술탄당 10~22 이벤트 |

### 주요 인터뷰 / 강연 / 자료

- AIAS Game Maker's Notebook — "17 Year Development Journey with Caves of Qud" 팟캐스트: [링크](https://interactive.libsyn.com/17-year-development-journey-with-caves-of-qud)
- GDC — "Math for Game Developers: End-to-End Procedural Generation in Caves of Qud"(마을 절차 생성): [GDC Vault](https://www.gdcvault.com/play/1026313/Math-for-Game-Developers-End)
- Jason Grinblat (2017) — "Subverting the Trope of the Heroic Biography"(신화적 전기 생성 논문): [PDF](https://www.pcgworkshop.com/archive/grinblat2017subverting.pdf)
- Brian Bucklew, Roguelike Celebration 2019 — Wave Function Collapse 맵 생성 강연
- Unity 사례 연구 — "Systems-driven design in Caves of Qud": [Unity](https://unity.com/resources/systems-driven-design-in-caves-of-qud)
- RPG Site 인터뷰 — Bucklew on 확장·Switch 이식: [링크](https://www.rpgsite.net/interview/20000-brian-bucklew-caves-of-qud-interview-expansions-switch-port-unity-controller-support-coffee)

### 참고 자료 목록

- [Wikipedia — Caves of Qud](https://en.wikipedia.org/wiki/Caves_of_Qud)
- [Metacritic — Caves of Qud](https://www.metacritic.com/game/caves-of-qud/)
- [PC Gamer — Caves of Qud review](https://www.pcgamer.com/games/roguelike/caves-of-qud-review/)
- [PC Gamer — Best Roguelike 2024](https://www.pcgamer.com/games/roguelike/best-roguelike-2024-caves-of-qud/)
- [PC Gamer — DF & Caves of Qud 라운드테이블](https://www.pcgamer.com/dwarf-fortress-and-caves-of-qud-roundtable-the-masters-of-simulation-talk-roguelikes-ai-and-making-the-infinite-compelling/)
- [PCGamesN — 2024 highest-rated game (OpenCritic)](https://www.pcgamesn.com/caves-of-qud/open-critic-highest-rated)
- [GamesRadar — "100x better than expected"](https://www.gamesradar.com/games/roguelike/after-thousands-of-overwhelmingly-positive-steam-reviews-caves-of-qud-dev-says-the-roguelike-rpg-has-done-100x-better-than-anything-we-ever-expected/)
- [Steam — Caves of Qud](https://store.steampowered.com/app/333640/Caves_of_Qud/)
- [Official Wiki — World generation](https://wiki.cavesofqud.com/wiki/World_generation) / [Sultan histories](https://wiki.cavesofqud.com/wiki/Sultan_histories) / [Mutations](https://wiki.cavesofqud.com/wiki/Mutations) / [True Kin](https://wiki.cavesofqud.com/wiki/True_Kin)
- [TV Tropes — Caves of Qud](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/CavesOfQud)
