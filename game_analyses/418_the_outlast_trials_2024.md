# 《The Outlast Trials》 (2024) 심층 분석

> 협동(co-op)이라는 단어와 호러라는 장르는 본래 어울리지 않는다. 호러는 고립을 먹고 자라고, 협동은 안도를 만든다. 《The Outlast Trials》는 이 모순을 정면으로 끌어안은 게임이다. Red Barrels는 캐나다 몬트리올의 소규모 독립 스튜디오로서, 자사가 정의한 "도망치는 호러(run-and-hide horror)" 공식을 멀티플레이어 라이브 서비스로 이식하는, 시리즈 사상 가장 위험한 도박을 감행했다. 2023년 5월 얼리 액세스, 2024년 3월 5일 정식 1.0 출시를 거치며 누적 300만 플레이어를 돌파한 이 게임은, 1인칭 도망 호러가 친구 4명과 함께 즐기는 반복형 PvE 라이브 게임으로도 성립할 수 있음을 증명했다.

---

## 1. 게임 개요

### 개발사·퍼블리셔

《The Outlast Trials》는 캐나다 몬트리올의 **Red Barrels**가 개발·자체 퍼블리싱한 1인칭 서바이벌 호러 게임이다. Red Barrels는 2011년 **Philippe Morin**, **David Chateauneuf**, **Hugo Dallaire** 세 사람이 설립한 인디 스튜디오로, 세 창립자는 각각 《Prince of Persia: The Sands of Time》, 《Assassin's Creed》, 《Uncharted: Drake's Fortune》 등 AAA 프로젝트를 거친 베테랑 개발자들이었다. Red Barrels의 가장 큰 특징은 **외부 투자나 퍼블리셔 없이 Outlast 시리즈 전편을 독립 자금으로 개발·배급해 왔다**는 점이다. 캐나다가 소유한 자생적 호러 IP로서, 《Outlast》(2013), 《Outlast 2》(2017)에 이어 《The Outlast Trials》는 시리즈의 세 번째 정식 작품이다.

### 출시일·플랫폼

- **공개**: 2019년 10월, Cold War 시대를 배경으로 한 프리퀄로 발표
- **클로즈드 베타**: 2022년 10월 28일~11월 1일
- **얼리 액세스(PC, Steam·Epic)**: 2023년 5월 18일
- **정식 1.0 출시**: 2024년 3월 5일 — PC(Windows)와 함께 PlayStation 4/5, Xbox One, Xbox Series X/S로 동시 콘솔 출시

당초 2021년 8월 출시를 목표로 했으나 COVID-19 팬데믹으로 지연되었다. 약 10개월간의 얼리 액세스를 거치며 콘텐츠와 시스템을 다듬은 뒤 콘솔 동시 출시로 1.0을 맞았다.

### 장르

1~4인 협동(co-op) **1인칭 서바이벌 호러**. 시리즈 전통의 비전투(무기 없음) 도망·은신 호러를 PvE 멀티플레이 / 라이브 서비스 구조에 결합했다. 단독 플레이도 완전히 지원하므로 솔로 호러 게임으로도 성립한다.

### 디렉터·주요 크레딧

- **디렉터**: Alex Charbonneau
- **프로듀서**: Charles Ayotte
- **작가(Writer)**: J. T. Petty — 시리즈 전작들의 각본을 맡아온 인물로, 영화·코믹 분야 경력을 가진 호러 전문 작가
- **작곡(Composer)**: Tom Salta — 《Halo》, 《Ghost Recon》 등으로 알려진 미국 작곡가
- **공동 창립자·총괄**: Philippe Morin(시리즈 전반의 비전 주도)

### 개발 기간·규모·엔진

엔진은 **Unreal Engine 4**다. 이는 시리즈에서 중요한 전환점인데, 《Outlast》와 《Outlast 2》는 Red Barrels의 자체 개량 엔진을 사용했으나, 《The Outlast Trials》를 위해 팀은 4~5개월에 걸쳐 Unreal 4로 이주했다. Morin은 인터뷰에서 Unreal 4가 "새 아이디어를 빠르게 테스트하고 반복(iterate)하게 해 주었다"고 밝혔다. 멀티플레이어 네트워킹, 동적 절차적 변주(아래 RNG 항목 참조), 라이브 운영을 감당하기 위한 선택이었다.

개발 기간은 길었다. 얼리 액세스 시점 기준 약 6년에 걸쳐 개발되었으며, 《Outlast 2》(2017) 출시 직후 번아웃에 빠진 팀이 "다음 게임은 없을 것 같다"고 생각하던 시기에 출발했다. 정확한 인력·예산은 비공개지만, Red Barrels는 이 프로젝트를 계기로 **두 번째 개발팀을 신설**해 라이브 운영과 차기작(코드네임 Project Lupara, 추후 별개 신작) 병행 체제를 구축했다.

---

## 2. 게임 설명

### 컨셉

《The Outlast Trials》의 한 줄 컨셉은 "친구들과 함께 겪는 도망 호러"다. 시리즈 전통의 비전투 호러 — 적과 싸우지 않고 도망치고, 숨고, 어둠 속을 카메라(혹은 야시경)로 더듬으며 탈출하는 — 를 유지하되, 이를 **반복 플레이 가능한 "임무(Trial)" 단위**로 잘게 쪼개고, 그 임무를 최대 4인이 협동으로 클리어하는 구조로 재설계했다.

### 세계관·시대 배경

배경은 **1959년, Cold War(냉전)의 절정기**다. 시리즈 본편 《Outlast》(2013)와 《Outlast 2》보다 시간적으로 앞선 **프리퀄**로, 악의 근원인 **Murkoff Corporation**(머코프 사)의 기원을 다룬다. 머코프는 냉전기 미국에서 정부·군과 결탁해 **세뇌(brainwashing)와 마인드 컨트롤**을 연구하는 기업으로, 이는 실제 CIA의 비밀 마인드 컨트롤 프로그램 **MK Ultra**(1953~1973)를 노골적으로 모티프로 삼은 설정이다. 게임 내 "MK-Challenge"라는 명칭부터가 이 역사적 사건을 직접 가리킨다.

### 줄거리 (스포일러 포함)

[스포일러] 플레이어는 **Reagent(시약/반응체)**라 불리는 실험 대상이 된다. 머코프는 사회의 밑바닥에 있는 취약 계층 — 노숙자, 빈민, 사회로부터 버림받은 이들 — 을 "Charity Outreach Center(자선 봉사 센터)"라는 위장 시설로 유인한다. 새 삶의 기회를 주겠다는 제안에 속아 들어온 이들은 곧바로 납치되어 애리조나의 **Sinyala Facility(시냘라 시설)**로 이송된다. 거기서 Reagent들은 강제로 머코프의 "치료(therapy)" 프로그램에 투입된다.

이 "치료"의 실체는 **인격 파괴와 재구축**이다. 게임 설정 문서가 밝히는 머코프의 목표는 "자아를 부수는 것(Break the Self)" — 신병 훈련소나 사상 개조처럼, 피험자가 신성하거나 금기로 여기는 모든 것을 강제로 토해내게 만들어, 행동을 제약하던 도덕적·정서적 한계를 제거하는 것이다. 일련의 Trial을 모두 통과한 피험자는 "Reborn(재탄생)" 상태가 되어, 이론상 사회로 돌려보내져 머코프의 잠복 무기 — 명령에 따라 작동하는 인간 자산(sleeper agent) — 이 된다. 즉 플레이어가 게임을 "클리어"하는 것은 곧 머코프의 세뇌가 성공하는 것이라는, 냉소적이고 불온한 메타 서사가 깔려 있다.

### 캐릭터·주요 NPC

- **Reagent**: 플레이어 캐릭터. 외형·복장을 커스터마이즈할 수 있으며 고유한 서사적 정체성은 약하게 처리해 "익명의 피험자" 느낌을 살린다.
- **Easterman 박사 / The Pop**: 머코프 측 관리자. 무미건조하고 사무적인 어조로 비인간적 실험을 지시해 공포를 배가한다.
- **Prime Asset(주요 적)들**: 머코프가 만들어 낸 광기의 살해자들. 각자 강렬한 테마와 동선 패턴을 가진 보스급 적이다.
  - **Mother Gooseberry**: 동요 가수 콘셉트의 여성 적. "Daddy"라는 오리 인형(주둥이에 드릴이 달린)을 들고 끊임없이 노래하며 추격한다. 빠르고 집요해 떨쳐내기 어렵다.
  - **The Pusher**: 맵 곳곳의 흰 셔터에서 튀어나와 물리 피해 대신 환각 가스를 분사한다. 정신력(sanity)을 깎고 Skinner Man을 소환한다.
  - **The Skinner Man**: 정신력 게이지가 완전히 바닥나면 등장하는 환각 존재. Easterman 박사의 일그러진 형상으로, 정신을 회복할 때까지 따라붙는다.
  - **Franco Barbi(추가 콘텐츠)**: Season 1에서 추가된 세 번째 Prime Asset.
  - 그 외 다수의 일반 적(Rig 보유 적 포함)이 맵을 배회한다.

### 무드·톤·아트 디렉션

시리즈 특유의 **신체 훼손(body horror), 끈적한 어둠, 위생과 광기가 뒤섞인 시설 미학**을 1950~60년대 냉전 미학으로 재포장했다. 빛바랜 흑백 선전물, 정신병원/실험실 인테리어, 동요와 군중 통제의 공포를 섞은 카니발/고아원/경찰서 등 다양한 테마 맵이 등장한다. 어둠 속에서 야시경(green night vision) 시야로 더듬는 시리즈의 시그니처 연출은 여기서도 핵심이다.

### 사운드·음악

작곡가 **Tom Salta**가 음악을 맡아, 냉전기의 불안과 기관(institution)의 차가움을 표현하는 사운드스케이프를 구축했다. 사운드 디자인은 시리즈에서 늘 호평받는 요소로, 멀리서 들려오는 적의 발소리·노랫소리, 적이 가까워질 때의 음향 신호가 긴장의 핵심 도구로 작동한다. 여러 리뷰가 "어둠 속에서의 사운드 디자인이 소름 끼치게 훌륭하다"고 평가했다.

---

## 3. 핵심 시스템 / 메카닉

### 코어 게임플레이 루프 (moment-to-moment)

기본 루프는 시리즈 전통을 따른다: **싸우지 말고 도망치고 숨어라.** 플레이어는 무기를 들지 않는다. 적을 만나면 달리거나, 사물함·드럼통·침대 밑에 숨거나, 창문·구멍으로 빠져나간다. 어둠 속에서는 야시경으로 시야를 확보하지만 야시경에는 배터리(혹은 사용 자원) 제약이 있다. 적을 일시적으로 따돌리기 위해 벽돌·병을 던지거나 후술할 Rig를 쓴다.

이 위에 《The Outlast Trials》가 새로 얹은 것이 **목표 지향 임무 구조**다. Trial에 진입하면 머코프가 부여하는 일련의 목표 — 예컨대 특정 인물을 찾아 끔찍한 처형을 집행하거나, 물건을 모아 특정 장치를 가동하거나, 시체를 옮기는 등 — 를 수행하고 출구로 탈출해야 한다. 단순 탈출이 아니라 "임무 수행 + 탈출"이라는 구조가, 시리즈를 반복 플레이에 적합하게 만든 핵심 설계 변경이다.

### 진행 구조: Trial과 MK-Challenge, 로비 메타

- **Trial**: 서사 중심의 긴 "치료" 미션. 일정한 시간이 소요되는 본격 임무로, 클리어 시 핵심 보상을 준다.
- **MK-Challenge**: 기존 맵의 일부를 변형·재구성한 짧은 도전 미션. Trial 사이에 빠르게 소화하는 콘텐츠다.
- **The Sleep Room(개인 방)**: 플레이어의 거점. 임무 사이에 휴식하고, 외형·방을 꾸미고, 진척도를 관리한다.
- 모든 Trial과 MK-Challenge를 완수하면 "Reborn(재탄생)" 상태에 도달한다. 이는 사실상 본편 1회차 완주에 해당하며, Red Barrels에 따르면 **120만 명 이상의 플레이어가 Reborn에 도달**했다.

### RIG(리그) — 능동 스킬 시스템

시리즈 최초의 **능동 능력 시스템**이다. RIG는 머코프가 Reagent에게 주입하는 보조 장비/약물로, 플레이어는 6종 중 하나를 골라 장착한다. 대표적인 효과는 다음과 같다.

- **Stun(전격)**: 적을 일시 기절시킨다.
- **X-Ray(투시)**: 벽 너머 적·아군·목표를 본다.
- **Heal(치유)**: 자신/아군 체력 회복.
- **Blind(섬광)**: 적의 시야를 일시 차단.
- **Barricade(바리케이드, 추가 콘텐츠)**: Season 1에서 추가된 RIG.

RIG는 쿨다운과 충전 자원을 두고 운용되며, 적을 직접 죽이는 무기가 아니라 **도주·교란·지원**에 초점이 맞춰져 있어 "비전투 호러"라는 시리즈 정체성을 깨지 않는다.

### Prescription(처방) — 패시브/소모 강화

Prescription과 후술할 Amp는 영구·반영구 강화 시스템이다. Prescription은 캐릭터의 패시브 능력을 정의하며, 예컨대 쓰러진 동료를 발로 차서 깨우거나(Kick to Help) 빈사 상태 동료를 즉시 살리는(Lifesaver) 등 협동 지원 능력, 은신·이동·소음 관리 능력을 부여한다. 플레이어는 진척에 따라 처방 슬롯을 해금하고 빌드를 조합한다.

### Amp(앰프) — 영구 능력치 강화

Amp는 더 영구적인 능력치 강화로, 야시경 효율, 달리기 지속, 회복 효율 등 기초 스탯을 상향한다. 게임 내 화폐로 구매·업그레이드하며, RIG·Prescription·Amp의 조합이 곧 캐릭터 빌드를 형성한다. 이는 로그라이트적 메타 진척(meta-progression)을 호러에 이식한 부분이다.

### 정신력(Sanity)과 Psychosis 시스템

물리 체력 외에 **정신력(mental/sanity 게이지)**이 별도 자원으로 존재한다. The Pusher의 환각 가스나 특정 적·트랩에 노출되면 정신력이 깎이고, 완전히 바닥나면 환각 존재 **Skinner Man**이 출현해 플레이어를 쫓는다. 정신력은 안정제(Antidote) 등으로 회복한다. 이는 신체적 위협과 정신적 위협을 분리해 공포의 층위를 늘린 장치다.

### 자원 관리·경제

맵에는 야시경 배터리, 회복 아이템, 안티도트, 던질 수 있는 병·벽돌, 자물쇠를 따는 데 쓰는 도구 등이 무작위 분포한다. 적의 추격을 피하며 이 자원을 긁어모으는 "스캐빈징"이 moment-to-moment 텐션의 한 축이다. 클리어 보상으로 얻는 게임 내 화폐는 Amp 업그레이드와 외형 커스터마이즈에 투입된다.

### 멀티플레이·협동 시스템

핵심 차별점이다. 한 Trial을 **혼자(1인), 또는 2·3·4인 팀**으로 도전할 수 있다. 협동은 강제되지 않으며 필수 목표는 솔로로도 달성 가능하다. 그러나 인원이 늘수록:

- 맵을 배회하는 **적의 수가 증가**해 난도가 올라간다.
- 쓰러진 동료를 일으켜 세우는 부활 메커니즘이 작동해, 한 명이 잡혀도 팀이 살릴 수 있다.
- 역할 분담과 동선 조율(coordination)이 사실상 필수가 된다 — 누군가는 미끼로, 누군가는 목표 수행으로.

Red Barrels가 멀티플레이로 방향을 튼 계기 자체가 "플레이어들이 컨트롤러를 돌려가며 함께 비명 지르고 웃는" 온라인 현상의 관찰이었다. "공포를 함께 경험한다면 어떨까"라는 질문이 설계의 출발점이었다.

### 절차적 변주(RNG)와 재플레이성

같은 Trial이라도 적 배치, 목표 위치, 일부 레이아웃 요소가 변주되도록 설계해 반복 플레이의 신선도를 유지하려 했다. 이는 라이브 서비스 PvE로서 장기 수명을 확보하기 위한 핵심 설계다.

### 라이브 운영 / 시즌 / MTX

- **무료 콘텐츠 업데이트** 중심으로 운영된다. 새 맵·미션·적·RIG·게임 모드가 무료로 추가된다.
- 외형 커스터마이즈를 위한 **유료 코스메틱 팩**(예: Exotica Pack)이 수익 모델이며, 게임플레이 능력은 판매하지 않는 비(非)P2W 기조다.
- **시즌제**: Season 1 "Project Lupara"(2024년 7월 16일)부터 시즌 단위 운영. 한정 이벤트(Toxic Shock, Bambino, Countdown, Winter Kills 등)를 순환 제공하고, 커뮤니티 투표로 주간 이벤트를 정하는 "Flashback Therapy" 체제도 도입했다.

### 난이도·접근성

인원 수에 따른 동적 난도, 다양한 빌드 조합, 솔로/협동 선택지가 폭넓은 난이도 곡선을 만든다. 호러 강도가 매우 높은 게임이므로(고어·정신적 충격), 시리즈 전통대로 강도 높은 콘텐츠 경고가 있다.

### UI/UX 디자인 철학

몰입을 해치지 않는 최소 HUD를 지향하되, RIG·Amp·Prescription·시즌 콘텐츠가 늘면서 메뉴 복잡도가 증가했다. Season 1에서 "UI 전면 개편(UI overhaul)"을 단행한 것은 라이브 서비스화에 따른 정보량 증가에 대응한 조치다.

---

## 4. 평가

### Metacritic / OpenCritic

정식 1.0 출시 기준 평점은 플랫폼별로 갈렸다.

| 플랫폼 | Metacritic 평론 점수 |
|---|---|
| PlayStation 5 | 75 |
| Xbox Series X | 74 |
| PC | 69 |

OpenCritic 기준 평론가 추천율은 약 62%로 집계되었다. 전반적으로 "generally favorable(대체로 호의적)"에서 "mixed-to-positive(중립~긍정)" 사이에 위치한다. 유저 점수는 Metacritic 기준 7.5 수준으로 평론보다 후한 편이었다.

### 주요 평론 인용

- **IGN — 7/10**: "The Outlast Trials is a bloody cooperative horror game that burns brightly, but fizzles after a few enjoyable hours."(피로 물든 협동 호러로 강렬하게 타오르지만, 즐거운 몇 시간이 지나면 김이 빠진다.)
- **GameSpot — 8/10**: "The Outlast Trials is excessive and frantically enjoyable — but can occasionally tip over into frustration more than fear."(과잉이고 광적으로 즐겁지만, 때때로 공포보다 좌절로 기운다.)
- **PC Gamer**: "...one of the best co-op horror games."(최고의 협동 호러 게임 중 하나)라며 "메스꺼울 정도(makes me sick to my stomach)"라는 표현으로 강도를 호평.
- **Windows Central**: "Outlast becoming a terrifying, story-driven multiplayer game was not on my bingo card for 2024."(Outlast가 무섭고 서사적인 멀티플레이 게임이 될 줄은 예상 못 했다.)

평론의 일관된 논지는 "협동 호러로서의 독창성과 강도는 높지만, 수 시간 후 반복 피로가 온다"였다.

### 상업 지표 (판매·플레이어)

- **얼리 액세스 출시 첫 주 50만 장 이상** 판매. Steam 동시 접속 최고치는 2023년 5월 21일 **36,689명**(SteamDB/Steam Charts 기준).
- **2023년 7월 100만 장 돌파**, **2023년 12월 시점 150만 장 이상** 판매.
- **2024년 4월 200만 명 돌파**(Toxic Shock 업데이트 시점), **2025년 누적 300만 플레이어 돌파**.
- **120만 명 이상의 플레이어가 "Reborn"(본편 1회차 완주)** 달성.

자체 자금으로 운영되는 독립 스튜디오의 라이브 서비스 호러로서는 매우 견고한 성과다.

### 유저 평가

Steam 유저 평가는 출시 전반에 걸쳐 강한 호평("매우 긍정적" 수준)을 유지했다. 특히 친구들과 함께하는 협동 경험에 대한 만족도가 높았고, 무료 업데이트 중심 운영과 비(非)P2W 기조가 커뮤니티 신뢰를 쌓았다.

### 평론-유저 괴리

평론(특히 PC 69점)은 "반복성"을 비교적 엄격히 감점한 반면, 유저는 "친구와의 반복 플레이가 곧 콘텐츠"라는 라이브 게임 특유의 가치 평가로 더 후하게 매겼다. 솔로 평론 환경에서 측정된 반복 피로가, 실제 협동 플레이 환경에서는 사회적 재미로 상쇄되는 전형적인 멀티플레이 게임 괴리 패턴이다.

---

## 5. 성공 요인 분석

### 1) "도망 호러 + 협동"이라는 미개척 교차점 선점

호러 협동 PvE 시장에는 《Dead by Daylight》(비대칭 PvP)나 《Phasmophobia》(조사형 호러)가 있었지만, **무기 없는 1인칭 도망 호러를 정통 4인 PvE로 구현한 사례는 사실상 없었다.** Red Barrels는 이미 시리즈로 검증된 "run-and-hide" 공포 공식을 협동으로 확장함으로써, 경쟁이 적은 틈새를 자사의 강점으로 점유했다.

### 2) IP 자산의 영리한 재활용

10년 넘게 쌓인 Outlast 세계관 — 머코프, 정신병원 호러, body horror 미학 — 을 그대로 가져와, 신규 시스템(RIG, 빌드, 시즌)만 얹었다. 이는 신규 IP보다 위험이 낮고, 시리즈 팬층을 초기 동력으로 확보하게 했다. 동시에 MK Ultra라는 실제 역사 소재가 세계관에 무게와 화제성을 더했다.

### 3) 라이브 서비스 친화적 구조 설계

게임을 "긴 단일 캠페인"이 아니라 **재플레이 가능한 임무 단위(Trial/MK-Challenge) + 메타 진척(Amp/Prescription) + 시즌 이벤트**로 분해한 것이 결정적이다. 이 구조 덕분에 무료 콘텐츠를 지속 투입하며 수명을 늘릴 수 있었고, 실제로 출시 후 수년간 플레이어 수가 우상향했다.

### 4) 얼리 액세스의 모범적 활용

약 10개월의 얼리 액세스 동안 밸런스·콘텐츠·성능을 다듬고 커뮤니티 피드백을 수렴했다. 첫 주 50만 장이라는 초기 자금과 검증을 확보한 뒤 콘솔 동시 1.0으로 확장한 단계적 출시는, 자체 자금 독립 스튜디오로서 리스크를 분산한 영리한 전략이었다.

### 5) "함께 비명 지르는" 콘텐츠의 시대성

스트리밍·클립 문화에서 협동 호러는 폭발적 바이럴 소재다. Red Barrels의 멀티플레이 전환 자체가 이 현상의 관찰에서 출발했고, 결과적으로 트위치·유튜브에서의 노출이 마케팅을 대체하는 선순환을 만들었다.

### 6) 비(非)P2W 무료 업데이트 신뢰

능력이 아니라 외형만 파는 코스메틱 수익 모델, 그리고 새 맵·적·모드를 무료로 푸는 운영 기조가 커뮤니티의 장기 신뢰를 구축했다. 라이브 서비스 게임 다수가 신뢰 붕괴로 무너지는 시대에 이는 중요한 차별점이었다.

### 동시기 작품 대비 차별점

- 《Dead by Daylight》: 비대칭 PvP / 본작은 협동 PvE.
- 《Phasmophobia》: 조사·관측형, 직접 추격 위협 약함 / 본작은 직접 추격·도주가 핵심.
- 《Lethal Company》(2023): 코미디·물리 기반 협동 호러 / 본작은 진지한 body horror와 서사.

---

## 6. 비평적 시각 / 한계 / 논란

### 1) 반복 피로 (가장 일관된 비판)

거의 모든 평론이 지적한 약점. 수 시간이 지나면 같은 적, 같은 은신·스캐빈징 루프를 반복하게 되고, 절차적 변주에도 불구하고 신선도가 떨어진다. IGN이 "몇 시간 뒤 김이 빠진다"고 한 것이 대표적이다. 임무 다양성과 적 종류의 한계가 장기 단독 플레이의 발목을 잡는다.

### 2) 협동 ↔ 공포의 트레이드오프

본작의 정체성 자체에 내장된 딜레마. 여러 평론이 "함께 하면 더 재미있지만, 그 재미는 분위기와 공포의 희생 위에 성립한다"고 짚었다. 동료가 곁에 있다는 안도감, 채팅과 웃음은 호러의 핵심인 고립감을 약화시킨다. 역으로 "진짜 공포는 혼자 할 때 나온다"는 평가가 많았는데, 이는 게임이 솔로와 협동 양쪽에서 최적화되기 어려운 구조적 모순을 안고 있음을 보여준다.

### 3) 좌절로 기우는 난도 스파이크

GameSpot이 "공포보다 좌절로 기운다"고 한 부분. 적의 집요한 추격(특히 Mother Gooseberry처럼 빠르고 떨쳐내기 어려운 적), 정신력 고갈 연쇄 등이 무서움이 아니라 짜증으로 체감되는 순간이 있다는 지적이다.

### 4) 단일 플레이 게임으로서의 어중간함

여러 평론이 "단일 플레이어 게임으로는 마크에 못 미친다"고 보았다. 본편 《Outlast》가 제공한 응축된 일회성 서사 공포에 비해, Trial 구조는 서사가 파편적이고 반복적이라 서사 호러 팬에게는 갈증을 남긴다.

### 5) PC 평점이 낮았던 이유

PC Metacritic 69점은 콘솔보다 낮은데, 초기 PC 버전의 성능·밸런스 이슈, 그리고 PC 평론이 비교 기준으로 삼는 호러 작품군의 눈높이가 영향을 미친 것으로 보인다.

특기할 만한 대형 운영 논란(가챠·소액결제 스캔들 등)은 없었다는 점이 본작 운영의 강점이기도 하다.

---

## 7. 영향과 유산

### 장르적 영향

《The Outlast Trials》는 **"도망 호러의 라이브 서비스화"가 상업적으로 성립함을 입증**했다. 비전투·도주 중심 호러를 반복형 PvE로 만들 수 있다는 선례는, 이후 협동 호러 장르 설계의 한 참조점이 되었다. 《Dead by Daylight》가 비대칭 PvP로, 《Lethal Company》가 코미디 협동으로 시장을 키운 흐름 속에서, 본작은 "진지한 서사형 협동 PvE 호러"라는 또 하나의 축을 세웠다.

### 후속 / 확장

Red Barrels는 본작을 "게임이라기보다 TV 시리즈에 가깝다"고 표현하며 장기 운영을 천명했다. 시즌 단위 무료 업데이트(Project Lupara 등)로 콘텐츠를 지속 확장했고, 이 운영 경험과 인력 증강(두 번째 팀 신설)을 바탕으로 시리즈의 다음 단계(차세대 Outlast 프로젝트)로 이어갈 토대를 마련했다. 한 시니어 디자이너는 "Trials 대신 Outlast 3를 만들었다면 더 빨리 출시했을 것"이라고 회고하기도 했는데, 이는 멀티플레이·라이브 전환이 그만큼 큰 모험이었음을 방증한다.

### 산업적 의미

**외부 투자 없는 독립 스튜디오가 자생적으로 라이브 서비스 호러 IP를 성공시킨 모범 사례**다. 캐나다(몬트리올) 게임 생태계에서 자체 소유 IP를 장기 운영 자산으로 키운 점, 그리고 비(非)P2W 무료 업데이트 모델로 신뢰를 유지하며 300만 플레이어에 도달한 점은, 대형 퍼블리셔의 라이브 서비스가 잇따라 실패하던 시기에 더욱 두드러진다.

### 문화적 의미

MK Ultra라는 실제 냉전기 비윤리 실험을 게임 메커니즘(세뇌=클리어=Reborn)으로 번역해, "플레이어가 세뇌당하는 것이 곧 게임 진행"이라는 불온한 메타 서사를 구현했다. 또한 스트리밍 시대에 "친구와 함께 비명 지르는 호러"라는 사회적 콘텐츠 포맷을 정착시키는 데 기여했다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
|---|---|
| 개발사 / 퍼블리셔 | Red Barrels (자체 퍼블리싱) |
| 디렉터 | Alex Charbonneau |
| 작가 | J. T. Petty |
| 작곡 | Tom Salta |
| 엔진 | Unreal Engine 4 |
| 장르 | 1~4인 협동 1인칭 서바이벌 호러 |
| 공개 | 2019년 10월 |
| 클로즈드 베타 | 2022년 10월 28일~11월 1일 |
| 얼리 액세스(PC) | 2023년 5월 18일 |
| 정식 1.0 출시 | 2024년 3월 5일 (PC·PS4/5·Xbox One/Series) |
| 배경 | 1959년 냉전기, 애리조나 Sinyala Facility |
| Metacritic | PS5 75 / Xbox Series X 74 / PC 69 |
| OpenCritic 추천율 | 약 62% |
| IGN | 7/10 |
| GameSpot | 8/10 |
| EA 첫 주 판매 | 50만 장 이상 |
| Steam 최고 동접 | 36,689명 (2023-05-21) |
| 누적 플레이어 | 300만+ (2025) |
| "Reborn" 달성 | 120만+ |
| Season 1 | Project Lupara (2024-07-16) |

### 주요 인터뷰·자료

- Game Developer, "Horror in the Making: How Red Barrels outlasted Outlast" — 시리즈와 스튜디오 진화사
- MobileSyrup (2024-07) — Philippe Morin 인터뷰, 《The Outlast Trials》의 진화와 캐나다 자생 IP
- DualShockers — Alex Charbonneau·Philippe Morin 인터뷰, 게임의 미래 비전
- GamingBolt — "The Outlast Trials is 'More Like a TV Series'" (Red Barrels 운영 철학)
- PlayStation.Blog (2024-07-16) — Project Lupara 비하인드신

### 참고 자료 목록 (영어권 매체 중심)

- [The Outlast Trials — Wikipedia](https://en.wikipedia.org/wiki/The_Outlast_Trials)
- [The Outlast Trials Reviews — Metacritic](https://www.metacritic.com/game/the-outlast-trials/)
- [The Outlast Trials Critic Reviews — OpenCritic](https://opencritic.com/game/14938/the-outlast-trials/reviews)
- [The Outlast Trials — Steam](https://store.steampowered.com/app/1304930/The_Outlast_Trials/)
- [The Outlast Trials — SteamDB charts](https://steamdb.info/app/1304930/charts/)
- [The Outlast Trials Has Reached 3 Million Players — GamingBolt](https://gamingbolt.com/the-outlast-trials-has-reached-3-million-players)
- [The Outlast Trials passes 2M player milestone — GamesBeat](https://gamesbeat.com/the-outlast-trials-gets-toxic-shock-update-passes-2m-player-milestone/)
- [How Red Barrels outlasted Outlast — Game Developer](https://www.gamedeveloper.com/design/horror-in-the-making-how-red-barrels-outlasted-i-outlast-i-)
- [Montreal's Red Barrels on the evolution of The Outlast Trials — MobileSyrup](https://mobilesyrup.com/2024/07/27/montreal-red-barrels-the-outlast-trials-project-lupara-philippe-morin-interview/)
- [Project Lupara behind-the-scenes — PlayStation.Blog](https://blog.playstation.com/2024/07/16/the-outlast-trials-a-behind-the-scenes-look-at-project-lupara/)
- [The Outlast Trials makes me sick to my stomach — PC Gamer](https://www.pcgamer.com/games/horror/the-outlast-trials-makes-me-sick-to-my-stomach-but-thats-just-because-its-one-of-the-best-co-op-horror-games/)
- [The Outlast Trials review — Windows Central](https://www.windowscentral.com/gaming/the-outlast-trials-review)
- [Every Enemy In The Outlast Trials, Ranked — TheGamer](https://www.thegamer.com/the-outlast-trials-every-enemy-ranked/)
- [The Outlast Trials lore, explained — Dot Esports](https://dotesports.com/outlast/news/the-outlast-trials-lore-explained)

---

*본 분석서는 영어권 매체·공식 자료를 기반으로 작성된 한국어 심층 분석이며, 평점·판매·플레이어 수치는 출시 시점부터 2025년까지 보고된 공개 수치를 종합한 것이다.*
