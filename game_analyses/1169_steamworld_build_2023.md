# SteamWorld Build (2023) 심층 분석

> "Anno meets Dungeon Keeper." — 개발사 The Station이 직접 내건 한 줄 컨셉. 지상에서는 도시를 짓고, 지하에서는 던전을 캐는 이중 레이어 시뮬레이션. 《SteamWorld Build》는 13년 차 SteamWorld 프랜차이즈가 또 한 번 장르를 갈아탄 "장르 유랑"의 결과물이자, 동시에 그 모회사 Thunderful의 재정 붕괴라는 어두운 배경 위에 놓인 작품이다.

---

## 1. 게임 개요

《SteamWorld Build》는 2023년 12월 1일 출시된 도시 건설 + 던전 관리 하이브리드 시뮬레이션 게임이다.

- **개발사**: The Station (스웨덴 Thunderful Development 산하 스튜디오)
- **퍼블리셔**: Thunderful Publishing
- **출시일**: 2023년 12월 1일 (PC/콘솔 동시), 데이 원 Xbox Game Pass 포함
- **플랫폼**: Windows(PC), Nintendo Switch, PlayStation 4, PlayStation 5, Xbox One, Xbox Series X|S
- **장르**: 도시 건설(city builder) + 던전 관리/채굴 시뮬레이션
- **엔진**: Unity
- **개발 규모**: 약 40명 규모 팀, 개발 시작은 2020년 초로 알려짐
- **프랜차이즈 디렉터**: Brjánn Sigurgeirsson (SteamWorld 시리즈 창립자, Image & Form 설립자)
- **프로듀서**: Adam Vassée
- **작곡**: Ola Bäckström
- **출시 가격**: 정가 29.99달러 (예약구매 한정 26.99달러)

이 작품에서 가장 먼저 짚어야 할 사실은, **《SteamWorld Build》가 SteamWorld 역사상 처음으로 스웨덴 원조 스튜디오 Image & Form이 아닌 다른 팀의 손에서 만들어진 정식 시리즈 작품**이라는 점이다. SteamWorld 시리즈는 그동안 줄곧 Image & Form이 단독 개발해 왔지만, 2020년 Image & Form이 Thunderful Development로 통합된 이후 프랜차이즈는 Thunderful 그룹 산하의 다른 스튜디오로도 확장될 수 있는 IP가 되었다. 《SteamWorld Build》는 그 첫 사례로, The Station이라는 사내 다른 팀이 개발을 맡되 시리즈 창립자 Brjánn Sigurgeirsson이 프랜차이즈 디렉터로서 IP의 "본질"을 지키도록 감독하는 구조로 진행되었다. (출처: Wikipedia "SteamWorld Build", Pocket Tactics 인터뷰, VGC)

후일 작품의 평가를 이해하려면, 이 "IP 위탁 개발"이라는 구조가 중요한 맥락이 된다. SteamWorld는 늘 "다음에는 또 무슨 장르?"라는 기대를 받는 시리즈였고, Build는 그 기대를 한 번 더 충족하면서도, 동시에 원조 팀의 손때가 빠진 첫 외전이기도 했다.

---

## 2. 게임 설명 — 이 게임이 뭔지

### 세계관과 SteamWorld라는 우주

SteamWorld 시리즈의 세계는 인간이 사라진 뒤 증기로 움직이는 로봇(steambot)들이 문명을 이어가는 스팀펑크/서부극 풍의 우주다. 이 우주의 독특한 매력은 **"한 세계관, 여러 장르"**라는 점에 있다. 2010년 닌텐도 DSi용 《SteamWorld Tower Defense》(타워 디펜스)에서 출발해, 《SteamWorld Dig》(2013, 메트로배니아 채굴 액션)과 그 속편 《SteamWorld Dig 2》(2017), 《SteamWorld Heist》(2015, 턴제 전략 슈팅), 《SteamWorld Quest》(2019, 카드 기반 RPG)로 이어지며, 시리즈는 매번 전혀 다른 장르로 갈아탔다. "동일 IP에서 장르를 자유자재로 바꿔 온 거의 유일한 프랜차이즈"라는 평가는 여기서 나온다. (출처: Image & Form 위키, Wikipedia "SteamWorld Heist")

《SteamWorld Build》는 이 우주에 **도시 건설 + 던전 관리 시뮬레이션**이라는 또 하나의 장르를 추가했다.

### 줄거리 [스포일러 포함]

게임의 무대는 죽어가는 행성이다. 로봇들은 이 행성을 탈출해야 하며, 그러기 위해 오래전 잊힌 고대 기술 부품(로켓 부품)을 발굴해야 한다. 주인공은 **Jack Clutchsprocket**으로, 그는 피난민 무리를 이끌고 버려진 광산으로 향한다. 시간적 배경은 《SteamWorld Dig 2》의 사건들과 맞물린 시점으로 설정되어 있어, 시리즈 팬에게는 연속성의 즐거움을 준다.

[스포일러] 광산을 파 내려가면서 플레이어는 "Core"라는 수수께끼의 봇과 마주친다. 그러나 Core는 협력자가 아니라 **Vectron 하이브마인드(Vectron Hivemind)의 일부**임이 드러나는 기만적 존재다. 시리즈 단골 적성 세력인 Vectron이 다시 등장하는 셈이다. 결말에서 Trader라는 캐릭터가 자신을 희생해 탈출을 가능케 하지만, 하이브마인드는 들키지 않은 채 로봇들의 시스템에 침투한다 — 시리즈 후속을 위한 떡밥을 남기는 다소 씁쓸한 마무리다. (출처: Wikipedia "SteamWorld Build")

### 무드, 톤, 아트 디렉션

《SteamWorld Build》는 시리즈 특유의 **밝고 정갈한 카툰 스팀펑크 톤**을 유지한다. 황량한 사막 위에 점점 불어나는 아기자기한 로봇 마을, 그 아래로 음습하게 펼쳐지는 광산의 대비가 시각적 정체성을 만든다. 전반적으로 게임은 "느긋하고 chill한" 무드를 의도했다. 압박이 적고 패배가 거의 없는 설계(후술)는 단점이자 동시에 의도된 톤이었다.

### 사운드와 음악

음악은 Ola Bäckström이 맡았다. 시리즈 특유의 서부극/스팀펑크 정서를 도시 건설 게임의 잔잔한 BGM 톤에 녹여낸 사운드트랙으로, 게임의 느긋한 분위기를 뒷받침한다. (작곡 크레딧 출처: Wikipedia)

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

《SteamWorld Build》의 설계 핵심은 **"두 개의 게임을 한 화면 위아래로 포개 놓되, 둘이 서로 의존하게 만든다"**는 데 있다. 개발진은 인터뷰에서 두 게임플레이가 "서로 독립적이지 않도록" 신경 썼다고 강조했다. (출처: Pocket Tactics 인터뷰)

### 3-1. 지상: 도시 건설 (Anno 계열)

플레이어는 황무지에 도로, 인프라, 편의시설, 주택을 짓는다. 도시의 진척은 **인구 마일스톤(milestone)**으로 측정되며, 인구는 네 가지 계급(class)으로 나뉜다.

| 계급 | 역할 |
| --- | --- |
| Workers (노동자) | 비숙련 노동 |
| Engineers (엔지니어) | 중장비 운용 |
| Aristobots (귀족봇) | 각종 산업 운영 |
| Scientists (과학자) | 신기술 연구·개발 |

이 구조의 진수는 **"수요의 단계적 상승"**에 있다. 각 계급의 로봇은 다음 계급으로 승급(upgrade)되기 위해 충족해야 할 욕구(needs)가 정해져 있다. 예컨대 Worker는 잡화점(general store)과 서비스 스테이션(service station) 접근이 필요하지만, Engineer로 승급하면 갑자기 숯(charcoal), 햄버거, 측량 사무소(surveyor's office) 같은 새로운 욕구가 생긴다. 즉 인구가 늘고 계급이 올라갈수록 플레이어는 **점점 더 복잡한 공급망**을 새로 깔아야 한다. (출처: Wikipedia, The Geekly Grind, mejoress 가이드)

이는 Anno 시리즈의 "주민 등급별 욕구 충족" 구조를 SteamWorld식으로 단순·명료화한 것이다.

### 3-2. 경제와 생산 사슬

경제 관리가 게임의 중심축이다. 일부 품목은 여러 상품의 재료로 쓰이기 때문에, 어느 한 자원을 너무 적게 생산하면 공급망 전체가 막힌다. 게임은 **ledger(원장) 기능**을 제공해 모든 생산 품목의 수요·공급을 한눈에 보여준다. 무언가가 부족하면 공장을 더 짓거나 공급망 전체를 확장해야 한다. (출처: The Geekly Grind, cogconnected)

돈은 주로 **주거세(residential tax)**로 들어온다. 주거 건물의 욕구가 하나 충족될 때마다 10초마다 추가 수입이 발생하는 식이다. (출처: 검색 요약, LadiesGamers/mejoress 가이드)

### 3-3. 지하: 광산 = 던전 관리 (Dungeon Keeper 계열)

화면 아래로 내려가면 전혀 다른 게임이 펼쳐진다. 광산은 **여러 층(level)으로 나뉜 채굴/방어 공간**이며, 지상의 도시 생산을 떠받치는 핵심이다. 광산 운영 방식은 지상의 도시와 다르다 — 플레이어는 광부(Miners), 탐광꾼(Prospectors), 정비공(Mechanics), 경비(Guards) 같은 직군의 인원을 직접 배치하는 대신, **각 직군에 할당할 바닥 면적(floor space)을 사들이는 방식**으로 그 수를 간접 관리한다.

- **Prospectors(탐광꾼)**: 광맥, 농장, 추출기에서 자원을 채취해 갱도(mineshaft)를 통해 지상으로 운반한다.
- **Mechanics(정비공)**: 기계를 짓고 수리한다.
- **Guards(경비)**: 지하의 위협으로부터 방어한다.

깊이 내려갈수록 Ironium, Oil, Plastishrooms, Vectron Scrap 같은 더 희귀한 자원을 얻지만, 붕괴(collapses)나 크립(creep) 공격 같은 위험도 커진다. (출처: 검색 요약, Steam 커뮤니티 가이드, mejoress)

### 3-4. 코어 루프 (모먼트-투-모먼트)

게임의 코어 루프는 대략 이렇게 돈다. (1) 지상에서 주택과 편의시설을 지어 인구·세수를 늘린다 → (2) 늘어난 인구의 새 욕구를 충족할 공급망을 깐다 → (3) 그 공급망에 필요한 원자재를 지하 광산에서 캐낸다 → (4) 광산을 더 깊이 파면 새 자원·위협이 등장하고, 이를 막을 경비·정비 인력을 늘려야 한다 → (5) 충분한 고대 로켓 부품을 모으면 탈출(=클리어)에 다가간다. 지상과 지하가 자원·인력을 두고 끊임없이 핑퐁을 주고받는 구조다.

### 3-5. 진행 구조와 난이도

게임은 5개의 맵(settings)에 걸친 캠페인으로 구성된다. 난이도 옵션이 있어 낮은 난이도에서는 매우 느긋하게, 위협을 거의 신경 쓰지 않고 즐길 수 있다. 핵심 설계 철학은 **"접근성과 관용(forgiveness)"**이다. 게임 오버가 사실상 없고, 위기 후 재건이 강제되는 일도 거의 없다. 이는 장르 입문자에게는 큰 장점이지만, 하드코어 시뮬레이션 팬에게는 긴장감 부족으로 받아들여졌다(6번 항목 참조).

### 3-6. Mechanized DLC (2024) — 전투 강화

출시 약 4개월 뒤인 **2024년 4월 4일**, 유료 확장 《SteamWorld Build: Mechanized》가 출시되었다. 이 DLC는 다음을 추가했다. (출처: steamworldgames.com 공식, Steam, Nintendo Everything)

- **Mech(메크)**: 블록을 들어 올리고 부수며 적과 싸우는 거대 로봇 동반자. 도시에 새 건물 "The Mech Centre"를 지으면 고유 업그레이드를 받을 수 있다.
- **새 보스 Abomination**: 여러 Vectron 적이 합쳐진 강적으로, 방어를 소홀히 하면 무너뜨린다.
- 콘텐츠 추가: 새 광산 기능 8종, 고유 기능 블록 10종, "machine" 오브젝트 6종, 비(非)블록 아이템 2종, 신규 건물 1종, 신규 보스 1종.

Mechanized는 출시 당시 비판받았던 "전투·위협의 빈약함"을 보강하려는 시도였다는 점에서 의미가 있다.

---

## 4. 평가

### 4-1. 평론 점수 (집계)

| 매체/집계 | 점수 |
| --- | --- |
| OpenCritic | 77/100 ("Strong"), 평론가 54명, 추천율 70%, 상위 33% |
| Metacritic (PC/Switch) | 약 74 — "mixed or average" |
| Metacritic (PS5/Xbox Series) | "generally favourable" |
| IGN | 7/10 |
| PC Gamer | 69/100 |

(출처: OpenCritic, Metacritic, IGN, PC Gamer)

플랫폼별로 Metacritic 등급이 갈린 점이 흥미롭다 — PC와 Switch판은 "mixed or average", PS5와 Xbox Series판은 "generally favourable"로 집계되었다. (출처: Wikipedia "SteamWorld Build")

### 4-2. 주요 평론 인용

**IGN (7/10)**은 "이미 눈앞에 있는 것을 충분히 파악한 뒤에야 새 복잡성을 더해 나가는 영리한 장르 접근"이라 평하며, "단순하지만 재미있는 도시 건설 게임을, 던전을 짓는 채굴 요소와 영리하게 결합해 빠르고 캐주얼하게 굴러가도록 만들었다"고 호평했다. SteamWorld 특유의 "어떤 장르에도 적용되는 공식"이 다시 통했다는 것이다. 다만 "잘 플레이해야 할 압박이 거의 없고, 어느 시점부터는 결국 시간만이 변수임이 분명해진다"며 캠페인이 "환영받는 기간보다 오래 머문다(overstays its welcome)"고 지적했다. (출처: IGN, 검색 요약)

**PC Gamer (69/100)**의 평결은 가장 신랄했다. "느긋하고 경쾌하지만, 장르 팬을 만족시키고 SteamWorld라는 이름값에 부응할 만한 실속(substance)이 부족하다." 구체적으로 "결코 정신없어지지 않고, 정말 크게 잘못될 일이 없으며, 게임 오버의 위협이 없다 — 위기 뒤에 재건할 필요조차 없다"고 비판했다. 동시에 "있는 그대로 받아들이면 매력적이고 매우 chill하게 빠른 도시 건설을 즐길 수 있는 게임이며, 특히 장르에 처음 발을 들이는 사람, 어린 게이머에게 훌륭한 입문작"이라고 균형을 잡았다. (출처: PC Gamer)

**PCGamesN, TheSixthAxis, Gamereactor, cogconnected** 등도 대체로 "독창적이고 만족스러운 진척감을 주는 하이브리드지만 깊이·수명(longevity)이 아쉽다"는 일관된 결을 보였다. 특히 "5개 맵에 걸쳐 개발진의 변주(resourcefulness)가 제한적"이라는 지적이 반복됐다. (출처: 검색 요약, OpenCritic/Metacritic 집계)

### 4-3. 상업 지표와 모회사 맥락

판매량 같은 정확한 단독 수치는 공개되지 않았다. [추정] 다만 모회사 Thunderful Group의 재무 상황은 명확히 부정적이었다. Thunderful은 2023 회계연도에 **약 6억 940만 스웨덴 크로나(약 5,920만 달러)의 순손실**을 기록했고, "최근 몇 년간의 과잉 투자(over-investments)"를 원인으로 지목했다. 2024년 1월에는 **전체 인력의 약 20%, 약 100명 감원** 계획을 발표했고, 같은 해 11월 추가 구조조정으로 80~100명이 더 해고됐다. CEO는 "외부 파트너 게임을 퍼블리싱하는 방향으로 전환해 고정비를 줄이겠다"고 밝혔다. (출처: Game Informer, GameSpot, Game Developer, PocketGamer.biz, Console Creatures)

즉 《SteamWorld Build》는 평론상 무난한 성적을 거뒀음에도, 회사 전체가 흔들리는 시기에 출시되었고 시리즈 자매작들(예: 《SteamWorld Heist 2》)도 내부 매출 목표를 채우지 못했다는 보도가 있다. 작품의 "성공"을 평가할 때 이 거시 맥락을 빼놓을 수 없다.

### 4-4. 유저 평가

Steam에서 유저 반응은 대체로 긍정적이었다. 특히 "편안하고 접근성 높은 도시 건설"이라는 점이 호평받았다. 다만 평론과 마찬가지로 "엔드게임 콘텐츠와 도전 부족, 비교적 짧은 수명"이 반복 지적되었다. Mechanized DLC 출시 후에는 추가 깊이를 환영하는 반응도 있었다.

---

## 5. 성공 요인 분석

### 5-1. 디자인: "두 장르의 의존적 결합"

가장 큰 성공 요인은 **두 게임을 단순 병치하지 않고 자원·인력으로 묶었다**는 점이다. 지상 도시의 욕구가 지하 채굴을 끌어내고, 지하의 위험이 다시 지상의 경제 결정을 압박한다. "Anno meets Dungeon Keeper"라는 한 줄 컨셉이 마케팅 카피를 넘어 실제 메카닉으로 구현된 것이 핵심이었다. (출처: VGC, Pocket Tactics)

### 5-2. 점진적 복잡성(progressive disclosure)

여러 평론이 공통으로 칭찬한 지점은 **새 레이어를 한꺼번에 쏟지 않고, 앞 단계를 익힌 뒤에야 다음 복잡성을 펼치는 설계**다. 도시 건설 장르의 진입 장벽(수많은 메뉴와 그래프)을 낮추면서도 "발견과 의외성(discovery and surprise)"을 유지했다. 입문자 친화성과 시리즈 톤이 맞물린 결과다.

### 5-3. SteamWorld IP의 브랜드 자본

13년간 장르를 갈아타며 쌓은 **"SteamWorld는 늘 다른 장르로 우리를 놀라게 한다"**는 브랜드 기대가 마케팅 자산이 되었다. 도시 건설로의 전환은 그 자체로 화제성이 있었다. 출시 당일 무료 데모를 함께 풀어 진입 장벽을 더 낮춘 것도 영리했다. (출처: Wikipedia, 2023년 1월 발표·데모)

### 5-4. 출시 전략: 멀티플랫폼 + Game Pass 데이 원

PC, Switch, PS4/5, Xbox One/Series를 **전 플랫폼 동시 발매**하고, Xbox Game Pass에 데이 원으로 올려 노출과 플레이어 베이스를 빠르게 확보했다. 29.99달러라는 합리적 가격대도 캐주얼·입문자층을 겨냥한 포지셔닝과 맞았다. (출처: ResetEra, Gamerant, Wikipedia)

### 5-5. 동시기 작품 대비 차별점

같은 시기 도시 건설 장르에는 《Cities: Skylines II》(2023, 무거운 정통 시뮬레이션) 같은 헤비급이 있었다. 《SteamWorld Build》는 정반대 포지션 — **"가볍고 chill하며 두 장르를 섞은 입문용 빌더"**로 차별화해, 정통 시뮬레이션의 피로감을 피하려는 라이트 유저층을 흡수했다. PC Gamer가 "장르 첫 입문작으로 훌륭하다"고 한 것이 이 포지셔닝의 정확한 요약이다.

---

## 6. 비평적 시각 / 한계 / 논란

### 6-1. 긴장감과 실패의 부재

가장 반복된 비판은 **"위기와 게임 오버가 없다"**는 점이다. PC Gamer는 "정말 크게 잘못될 일이 없고, 위기 후 재건이 필요 없다"고 했고, IGN도 "잘 플레이할 압박이 거의 없으며 결국 시간만이 변수"라고 지적했다. Dungeon Keeper의 방어 긴장감, Anno의 경제 붕괴 위험 같은 짜릿함이 약하다는 것이다. 이는 접근성을 위해 의도된 설계였지만, 장르 베테랑에게는 "실속 부족"으로 읽혔다.

### 6-2. 수명과 콘텐츠 폭의 한계

"5개 맵에 걸쳐 개발진의 변주가 제한적", "수명이 짧고 엔드게임이 빈약하다"는 지적이 여러 매체에서 나왔다. IGN은 후반부에 캠페인이 "환영받는 기간보다 오래 머물며" 후반 목표가 경직되고 지루한 그라인드로 변한다고 했다. 컨셉 자체는 더 큰 게임으로 확장될 수 있었는데 그러지 못했다는 아쉬움이다.

### 6-3. "SteamWorld라는 이름값" 논란

PC Gamer의 평결("SteamWorld라는 이름값에 부응할 실속이 부족")은 이 작품이 짊어진 부담을 단적으로 보여준다. 《Dig》, 《Heist》 같은 전작들이 각 장르에서 높은 완성도로 호평받았던 반면, Build는 "괜찮지만 시리즈 평균에는 못 미친다"는 인식이 형성됐다. **원조 Image & Form이 아닌 외부 팀(The Station)이 처음 만든 작품**이라는 점과 맞물려, "본질이 옅어졌다"는 시각도 일부 존재했다.

### 6-4. 거시적 논란: 모회사 붕괴

작품 외적으로는 Thunderful Group의 대규모 손실과 두 차례 감원이 가장 큰 그림자다. Build가 직접 원인은 아니지만, 회사의 자체 개발 축소·외부 퍼블리싱 전환 결정 속에서 SteamWorld 프랜차이즈의 향후 자체 개발 여력 자체가 위협받게 되었다. (출처: Game Informer, Game Developer 등)

---

## 7. 영향과 유산

### 7-1. SteamWorld 프랜차이즈의 "장르 확장" 전략 검증

《SteamWorld Build》는 "이 IP는 어떤 장르든 갈 수 있다"는 Thunderful의 전략(VGC: "no genre is off the table")을 한 번 더 실증했다. 타워 디펜스 → 채굴 액션 → 턴제 전략 → 카드 RPG → 도시 건설로 이어진 장르 유랑의 다섯 번째 큰 분기점인 셈이다. 동시에, **IP를 원조 팀 밖으로 위탁해도 시리즈를 이어갈 수 있다**는 운영 모델을 시험한 첫 사례이기도 하다.

### 7-2. 캐주얼 도시 건설의 자리매김

Build는 정통 헤비 시뮬레이션과 모바일식 간단 빌더 사이의 빈틈, 즉 **"콘솔/PC에서 즐기는 가볍고 테마 있는 입문용 시티 빌더"**라는 틈새를 보여줬다. 이 포지션은 입문자·라이트 유저에게 도시 건설 장르의 매력을 전하는 통로로 기능했다.

### 7-3. DLC를 통한 사후 보강

Mechanized DLC는 출시 시 지적된 "전투·위협 빈약"을 메크와 신규 보스로 보강하려는, 라이브 사후 운영의 표본을 보여줬다. 또한 2025년 1월 9일에는 PS5와 Switch용 **물리(패키지) 판**이 출시되며 수명을 한 번 더 연장했다. (출처: thegg.net, GodisaGeek)

### 7-4. 산업적 의미

Build의 유산은 작품 자체보다, 그 출시를 둘러싼 **인디 퍼블리셔 Thunderful의 위기**라는 산업적 사건과 함께 기억된다. 평론상 무난하고 멀티플랫폼·Game Pass 전략을 갖춘 게임조차도, 과잉 투자와 수익성 압박 속에서 회사를 구하지 못한다는 사실은 2023~2024년 게임 업계 구조조정 흐름의 한 단면이었다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
| --- | --- |
| 개발사 | The Station (Thunderful Development 산하) |
| 퍼블리셔 | Thunderful Publishing |
| 출시일 | 2023년 12월 1일 (전 플랫폼 동시) |
| 플랫폼 | PC(Windows), Switch, PS4, PS5, Xbox One, Xbox Series X\|S |
| 엔진 | Unity |
| 팀 규모 | 약 40명 |
| 개발 시작 | 2020년 초 |
| 프랜차이즈 디렉터 | Brjánn Sigurgeirsson |
| 프로듀서 | Adam Vassée |
| 작곡 | Ola Bäckström |
| 정가 | 29.99달러 |
| OpenCritic | 77/100 ("Strong"), 추천율 70% |
| Metacritic | PC/Switch 약 74 (mixed/average), PS5/Xbox 호평 |
| IGN | 7/10 |
| PC Gamer | 69/100 |
| 주요 DLC | 《SteamWorld Build: Mechanized》 (2024년 4월 4일) |
| 물리판 | PS5/Switch, 2025년 1월 9일 |

### SteamWorld 시리즈 연표 (요약)

| 연도 | 작품 | 장르 |
| --- | --- | --- |
| 2010 | SteamWorld Tower Defense | 타워 디펜스 |
| 2013 | SteamWorld Dig | 메트로배니아 채굴 액션 |
| 2015 | SteamWorld Heist | 턴제 전략 슈팅 |
| 2017 | SteamWorld Dig 2 | 메트로배니아 채굴 액션 |
| 2019 | SteamWorld Quest | 카드 기반 RPG |
| 2023 | SteamWorld Build | 도시 건설 + 던전 관리 |
| 2024 | SteamWorld Heist 2 | 턴제 전략 (속편) |

### 주요 인터뷰·자료

- Pocket Tactics, "SteamWorld Date Racing, and why SteamWorld can go anywhere" (The Station 인터뷰)
- VGC, "Thunderful says no genre is off the table for new SteamWorld games"

### 참고 자료 (영어권 매체 중심)

- Wikipedia, "SteamWorld Build" — https://en.wikipedia.org/wiki/SteamWorld_Build
- IGN, "SteamWorld Build Review" (7/10)
- PC Gamer, "SteamWorld Build review" (69/100) — https://www.pcgamer.com/steamworld-build-review/
- PCGamesN, "SteamWorld Build review" — https://www.pcgamesn.com/steamworld-build/review
- TheSixthAxis, "SteamWorld Build Review" — https://www.thesixthaxis.com/2023/11/27/steamworld-build-review/
- OpenCritic, "SteamWorld Build" — https://opencritic.com/game/15732/steamworld-build
- Metacritic, "SteamWorld Build" — https://www.metacritic.com/game/steamworld-build/
- ResetEra, "SteamWorld Build - Review Thread"
- cogconnected, "SteamWorld Build Review - Economy of Scale" — https://cogconnected.com/review/steamworld-build-review/
- The Geekly Grind, "SteamWorld Build [Review]"
- 공식, "Mechanized DLC for SteamWorld Build OUT NOW" — https://steamworldgames.com/steamworld-build/news/mechanized-dlc-out-now
- Game Informer, "Thunderful Group ... To Lay Off Roughly 100 People"
- Game Developer, "Thunderful laying off 20 percent of staff"
- PocketGamer.biz, "Thunderful lost $59 million in 2023"
- GameSpot, "Indie Publisher Thunderful To Lay Off 20% Of Its Workforce"

---

*본 분석서는 2023년 12월 출시판과 2024년 Mechanized DLC를 기준으로 작성되었으며, 판매량 등 비공개 수치는 [추정]으로 표기하고 검증 가능한 출처만 인용했다.*
