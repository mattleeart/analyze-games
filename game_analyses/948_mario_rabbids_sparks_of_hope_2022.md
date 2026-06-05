# 《Mario + Rabbids Sparks of Hope》 (2022) 심층 분석

> "게임 역사상 가장 기묘한 엘리베이터 피치 중 하나를, Ubisoft Milan과 Paris는 마리오 최고의 스핀오프 중 하나로 바꿔놓았다." — 《Polygon》

닌텐도의 간판 IP 《Super Mario》와 Ubisoft의 컬트 캐릭터 《Rabbids》를 섞어 만든 턴제 전술(tactics) 게임. 2017년 첫 작 《Mario + Rabbids Kingdom Battle》이 "농담 같은 발상"을 GOTY급 완성도로 증명한 뒤, 2022년 그 속편 《Sparks of Hope》가 등장했다. 이 분석서는 게임의 정체, 핵심 메카닉(특히 그리드를 버린 자유 이동 전투), 평가, 성공 요인과 한계, 그리고 "비평적 성공·상업적 실망"이라는 역설적 유산을 영어권 자료를 토대로 정리한다.

---

## 1. 게임 개요

### 기본 정보

| 항목 | 내용 |
|------|------|
| 정식 명칭 | 《Mario + Rabbids Sparks of Hope》 |
| 개발사 | Ubisoft Milan, Ubisoft Paris (지원: Ubisoft Pune, Chengdu, Montpellier) |
| 퍼블리셔 | Ubisoft (닌텐도 IP 라이선스 협업) |
| 디렉터 | Davide Soliani (크리에이티브 디렉터), Damiano Moro |
| 리드 디자이너 | Xavier Manzanares (브랜드 프로듀서 겸 공동 기획자) |
| 작곡 | Grant Kirkhope, Yoko Shimomura, Gareth Coker, Christophe Héral |
| 작가 | Andrea Babich, Edward Kuehnel |
| 출시일 | 2022년 10월 20일 |
| 플랫폼 | Nintendo Switch 독점 |
| 엔진 | Snowdrop (Ubisoft 자체 엔진) |
| 장르 | 턴제 전술 / 액션 어드벤처 RPG |

### 출신 — "닌텐도가 라이선스를 넘긴 IP"라는 사건

이 시리즈의 핵심은 **닌텐도가 자사 최고 가치 IP인 《Super Mario》를 외부 서드파티 스튜디오에 맡겼다**는 사실이다. 이는 닌텐도 역사상 극히 드문 일이며, 그 신뢰의 출발점이 1편 《Kingdom Battle》(2017)이다.

《Wikipedia》와 《GameSpot》 자료에 따르면, 마리오와 Rabbids의 크로스오버 발상은 2010년 Ubisoft Paris가 Wii용 어드벤처 게임으로 닌텐도에 제안했다가 거절당한 데서 시작했다. 이후 2013~2014년 Ubisoft Milan의 크리에이티브 디렉터 Davide Soliani와 브랜드 프로듀서 Xavier Manzanares가 "Rabbids 시리즈의 미래"를 고민하며 다시 닌텐도와 협의했고, 단순 파티 게임을 넘어 **XCOM 스타일 턴제 전술 게임**이라는 파격적 방향으로 발전시켰다. 닌텐도는 이를 승인하면서 "Davide, 무엇이든 요청해라. 최악의 경우 우리가 '아니오'라고 할 뿐이다"라는 태도로 협업했다고 Soliani는 회고한다.

1편은 2017년 E3 Ubisoft 컨퍼런스에서 공개되었고, 무대에 마리오의 창조자 **Shigeru Miyamoto**가 직접 올라 Soliani의 발표를 도왔다. 발표 도중 Soliani가 관객의 호응을 보고 무대에서 눈물을 흘린 장면은 인터넷 밈이 되었다. 1편은 닌텐도가 개발하지 않은 게임 중 Switch 최고 판매작 반열에 올랐고, 그 성공이 《Sparks of Hope》의 제작을 가능케 했다.

### 개발 규모와 기간

Soliani에 따르면 《Sparks of Hope》는 약 **3년 반(three and a half years)**에 걸쳐 제작되었으며, 그는 이 작품이 1편 《Kingdom Battle》보다 "만들기 더 어려웠다(harder to make)"고 밝혔다. 그리드를 버린 새 전투, 더 자유로운 오픈 구조의 행성 탐사, Sparks 시스템 등 거의 모든 시스템을 재설계했기 때문이다. Ubisoft Milan과 Paris를 중심 축으로, Pune·Chengdu·Montpellier 등 글로벌 스튜디오가 지원하는 전형적 Ubisoft 대형 협업 체제로 진행됐다. 캐릭터 시네마틱 애니메이션 외주는 이탈리아의 Maga Animation Studio가 일부 담당했다.

### 기술 스택

엔진은 Ubisoft 자체 **Snowdrop**으로, 《The Division》·《Avatar: Frontiers of Pandora》 등 고사양 작품에 쓰이던 엔진을 Switch라는 저전력 하드웨어에 맞춰 운용했다. 개발팀은 1편에서 Snowdrop과 Switch를 다뤄 본 경험 덕에 속편에서 **더 큰 스코프(bigger scope)**, 즉 그리드 없는 자유 이동·넓은 행성 탐사·더 화려한 비주얼을 구현할 수 있었다고 밝혔다(《Nintendo Everything》). 다만 이 야심은 후술할 로딩 시간·프레임 안정성 문제라는 비용을 동반했다.

---

## 2. 게임 설명

### 컨셉과 톤

《Sparks of Hope》는 한 문장으로 요약하면 "**마리오 캐릭터들과 Rabbids가 한 팀이 되어, 그리드 없이 자유롭게 움직이며 벌이는 우주 규모의 턴제 전술 어드벤처**"다. 1편이 버섯 왕국 한정의 다소 좁은 세계였다면, 속편은 다섯 개의 행성을 넘나드는 우주 모험으로 스케일을 키웠다. 톤은 여전히 명랑하고 슬랩스틱하지만, 《Super Mario Galaxy》와 《Super Mario Odyssey》를 떠올리게 하는 모험심·경이감을 더했다.

### 세계관과 줄거리 [스포일러 포함]

1편의 사건 이후 마리오의 세계와 Rabbids는 평화롭게 공존하고 있다. 그러나 **Sparks**라 불리는 존재들(Rabbids와 《Super Mario Galaxy》의 별 종족 Luma가 융합한 하이브리드)이 나타나면서 평화가 깨진다. 이들은 우주를 부식시키는 어둠의 힘 **Darkmess(다크메스)**에 쫓기고, 그 배후에는 빌런 **Cursa(커사)**가 있다.

[스포일러] Cursa는 1편의 거대 변칙 존재 'Megabug'에서 떨어져 나온 의식을 가진 파편으로 밝혀진다. 마리오 팀은 다섯 행성 — Beacon Beach, Pristine Peaks, Palette Prime, Terra Flora, Barrendale Mesa — 을 여행하며 Sparks를 구하고 새 동료를 모은다. 종반부 Cursa는 **Rosalina(로젤리나)**를 빙의·장악하지만, 팀은 Cursa를 물리치고 Rosalina를 구해 무사히 귀환한다.

### 주요 캐릭터 / 영웅 로스터

플레이어는 세 명으로 팀을 구성해 전투에 나선다. 주요 영웅은 다음과 같다.

- **Mario** — 균형형 사격수. 시리즈의 얼굴.
- **Luigi** — 장거리 저격형. 시야 내 대기 사격(overwatch) 특화.
- **Princess Peach** — 회복·생존 지원형.
- **Rabbid Peach** — 자가 회복과 탱킹.
- **Rabbid Luigi** — 상태 이상·디버프 특화.
- **Rabbid Mario** — 근접 산탄형.
- **Edge** — 속편 신규 Rabbid 영웅. 검을 든 시크한 전사로, Cursa에게 원한이 있어 합류한다. 회전 베기로 다수의 적을 동시 타격.
- **Rabbid Rosalina** — 속편 신규 영웅. 적의 행동을 방해(스킬 사용 봉인 등)하는 컨트롤형.
- **Bowser** — 적이었던 쿠파가 동료가 되어 합류. 미니언 소환과 광역 화력 담당.

조연으로는 안내자 역할의 로봇 비스킷(Beep-0), 그리고 위기의 Rosalina가 핵심 NPC로 등장한다. 이 작품은 마리오/루이지의 성우 **Charles Martinet**의 목소리가 (보이스 클립 형태로) 담긴 마지막 정규 마리오 타이틀 중 하나로, 그는 2023년 브랜드 앰배서더로 역할을 전환했다.

### 무드 / 아트 디렉션

전반적 비주얼은 화사한 색채와 코미디 연출이 중심이다. 다섯 행성 각각이 해변·설산·물감 세계·식물 정원·황무지 등 뚜렷한 비주얼 테마를 가져, 1편의 단조로운 버섯 왕국 톤에서 크게 벗어났다. Rabbids 특유의 과장된 슬랩스틱 개그(소리 지르고 넘어지고 카메오 패러디)와 마리오 세계관의 동화적 분위기가 충돌하면서 만들어내는 특유의 부조화가 시리즈의 정체성이다.

### 사운드 / 음악 — "게임 음악계의 드림팀"

《Sparks of Hope》의 사운드트랙은 영어권 매체가 일제히 "**게임 음악계 최고 작곡가들의 집결**"이라 표현한 호화 라인업으로 화제가 됐다(《NME》).

- **Grant Kirkhope** — 1편 작곡가. 《Banjo-Kazooie》·《GoldenEye 007》의 거장. 이번엔 내러티브·캐릭터 테마를 맡아 특유의 "친근하면서도 장엄한(friendly-epic)" 사운드를 유지.
- **Yoko Shimomura** — 《Kingdom Hearts》·《Street Fighter II》·《Final Fantasy XV》의 전설. 주로 **전투 큐(battle cues)**를 작곡하고, 전체 레코딩을 일본에서 총괄 조율했다.
- **Gareth Coker** — 《Ori and the Blind Forest》·《Halo Infinite》의 작곡가. 특정 무대와 보스전에 프랑스 인상주의 등 새로운 색채와 감정을 입혔다.

특기할 점은, 모든 곡을 일본의 두 스튜디오에서 동일한 연주자·동일한 장비·동일한 믹싱 엔지니어로 녹음해 음향적 통일성을 확보했다는 것이다. 닌텐도의 전설 **Koji Kondo(코지 콘도)**와 《Super Mario Galaxy》 공동 작곡가 **Mahito Yokota(요코타 마히토)**가 사운드트랙을 감수했다. 사운드트랙은 52개 트랙으로 게임 출시일과 같은 날 발매됐고, 이 음악은 후술하듯 2023년 Ivor Novello Awards에서 최우수 오리지널 게임 스코어를 수상했다.

---

## 3. 핵심 시스템 / 메카닉

《Sparks of Hope》의 정체성이자 가장 논쟁적인 변화가 바로 **전투 시스템의 전면 재설계**다. 1편이 《XCOM》식 그리드 전술이었다면, 속편은 그리드를 완전히 버렸다.

### 코어 게임플레이 루프

플레이는 크게 두 층위로 나뉜다.

1. **행성 탐사(오버월드)** — 각 행성을 비교적 자유롭게 돌아다니며 NPC와 대화하고, 퍼즐을 풀고, 숨은 Sparks와 보상을 찾고, 전투 트리거를 만난다.
2. **전투** — 트리거되면 별도의 전투 아레나로 전환되어 3인 팀으로 턴제 전술 전투를 치른다.

핵심 루프는 "탐사 → 전투 → 보상·성장 → 더 깊은 탐사"의 순환이며, 1편 대비 탐사 비중이 크게 늘었다. 마리오를 다른 캐릭터로 자유롭게 교체해 모험할 수도 있다.

### 그리드를 버린 자유 이동 — 가장 큰 변화

이 작품의 가장 결정적 혁신이다. 《IGN》은 "전작의 최고 아이디어는 유지하되, 즉시 매우 다르게 느껴질 만큼 스스로를 재발명했다"고 평했다. 구체적으로:

- **이동**: 전작의 칸(grid) 기반 이동을 폐기하고, 캐릭터를 일정 **이동 반경(movement radius)** 안에서 표준 3인칭 게임처럼 **자유롭게 조작**한다. 《Nintendo Life》는 "마리오 플랫포머에서처럼 자연스럽게 환경을 뛰어다닐 수 있다"고 표현했다.
- **행동 경제(turn/action economy)**: 각 캐릭터는 턴당 두 번의 행동을 쓸 수 있다. 무기를 발사하기(공격) 전까지는 반경 내에서 얼마든지 움직이며 위치를 잡을 수 있지만, **무기를 한 번 쏘면 그 캐릭터는 그 턴에 더 이상 이동할 수 없다.** 이 "공격 후 이동 불가" 규칙이 위치 선정의 긴장감을 만든다.
- **무료 행동(free actions)**: 무기 발사와 별개로, 이동 중 **Bob-omb(폭탄병)을 적에게 던지거나 대시로 적을 들이받는** 등의 무료 행동을 위치 이동 도중에 끼워 넣을 수 있다. 즉 "달려가며 폭탄을 던지고, 다시 자리를 잡아 사격"하는 식의 동선 설계가 핵심이다.
- **팀 점프(Team Jump)**: 아군을 발판 삼아 도약해 사거리·고도를 확보하는 시스템. 대부분의 캐릭터는 턴당 한 번만 점프할 수 있어, 세 명을 어떻게 연쇄 배치하느냐가 전술의 묘미가 된다.

《GameSpot》은 이 변화에 대해 "재설계된 전술 덕에 이 장르에서 본 것 중 손꼽히게 뛰어난 턴 경제(some of the best turn economy I've seen in the genre)를 만들어냈다"며 9/10을 부여했다.

### Sparks 시스템 — 속편의 새 진척 축

전투 깊이를 더하는 새 레이어가 **Sparks**다. 플레이어는 우주 전역에 흩어진 Sparks를 구출하며, 각 Spark는 전투에서 쓸 수 있는 고유 능력을 부여한다. 예를 들어 특정 Spark는 공격에 화염·냉기·전기 속성을 입히고, 어떤 것은 광역 폭발이나 보호막, 데미지 증폭을 제공한다.

- **각 영웅은 Spark를 두 개까지 장착**할 수 있다(1편의 능력 트리보다 훨씬 모듈러한 구성).
- 이로써 같은 캐릭터라도 장착 Spark 조합에 따라 전혀 다른 역할을 수행하게 되어, 팀 구성의 자유도와 변주가 크게 넓어졌다.
- Sparks 자체도 경험치로 성장시켜 능력 수치를 강화할 수 있다.

이 모듈식 빌드 시스템이 캐릭터를 "더 다재다능한 개인(more versatile individuals)"으로 만들고, 결과적으로 더 균형 잡힌 팀 빌딩을 가능케 했다는 것이 다수 매체의 평가다.

### 진행 구조와 성장

- **진행**: 다섯 행성 + DLC 추가 구역을 순회. 메인 퀘스트 외에 사이드 퀘스트, 숨은 보물, 환경 퍼즐이 곳곳에 배치된다.
- **성장**: 각 캐릭터는 스킬 트리(스킬 포인트로 능력 강화)와 Spark 장착, 무기 외형 변경 등으로 커스터마이즈된다. 1편보다 빌드 다양화와 실험 여지가 넓다.
- **경제**: 전투·탐사 보상으로 코인과 자원을 모아 강화에 투자한다.

### 난이도와 접근성

전투 시작 전 **상황에 따라 난이도를 자유롭게 조정**할 수 있는 것이 큰 접근성 장점이다. 세 가지 기본 모드 — **Relaxed(여유), Average(보통), Demanding(도전)** — 가 제공되며(《Game Rant》), 그 외에도 적의 체력·플레이어 데미지 등을 세부 슬라이더로 조절할 수 있어, 전투를 즐기는 코어 유저부터 스토리·탐사만 보고 싶은 라이트 유저까지 폭넓게 수용한다. 이 유연한 난이도 설계가 "가족 게임"으로서의 정체성을 뒷받침했고, 후술할 D.I.C.E. '올해의 가족 게임' 수상으로 이어진다. 다만 이 관대함이 도전 욕구가 강한 유저에게는 긴장감 부족이라는 양날의 검이 됐다(6장 참조).

### UI/UX 철학

자유 이동으로 전환되면서 UI도 "칸 단위 계획"에서 "공간 단위 직관"으로 바뀌었다. 이동 반경, 사거리, 시야선(라인 오브 사이트), 엄폐물의 보호 정도(반엄폐/완전엄폐)를 시각적으로 즉시 보여주어, 복잡한 전술을 직관적으로 계획하게 한다. 닌텐도 스타일의 친절한 온보딩과 슬랩스틱 연출로 진입 장벽을 낮춘 것이 일관된 디자인 철학이다.

---

## 4. 평가

### 평론 점수

《Sparks of Hope》는 비평적으로 매우 호평받았다.

| 지표 | 점수 |
|------|------|
| Metacritic (Switch) | 85/100 (약 122개 리뷰) |
| OpenCritic | 96% 추천 (약 127개 리뷰) |
| 주요 매체 다수 | 9/10, 4.5/5 등 |

### 주요 평론 인용

- **IGN (9/10)**: "후속작은 최고의 아이디어를 유지하면서도 즉시 매우 다르게 느껴질 만큼 스스로를 재발명했다. 거의 모든 면에서 더 크고 더 좋아졌으며, 더 자유롭고 커스터마이즈 가능한 전투와 거의 완전히 재구상된, 훨씬 덜 선형적이고 퍼즐로 가득 찬 오버월드를 갖췄다."
- **GameSpot (9/10) — "This Sparks Joy"**: "재설계된 전술 덕에 이 장르에서 손꼽히는 최고의 턴 경제를 보여준다. 전작의 모든 문제를 고치진 못했지만, Nintendo Switch 최고의 독점작 반열에 드는 가치 있는 속편이다."
- **Game Informer (9/10)**: 공식을 정련한 작품으로, 그래픽·사운드트랙·게임플레이 개선을 칭찬.
- **Polygon (Recommended)**: "이런 기묘한 조합이 이런 기쁨을 자아낼 줄 누가 예상했을까. 《Sparks of Hope》로 Ubisoft Milan과 Paris는 게임 역사상 가장 기묘한 엘리베이터 피치 중 하나를 마리오 최고의 스핀오프 중 하나로 바꿔놓았다."
- **Eurogamer (Recommended)**: "원작을 특별하게 만든 모든 것을 포착하면서, 더 복잡하고 완성도 높은 경험을 제공한다. 새로운 차원의 전략적 깊이를 갖췄고, 기대 이상으로 진짜 《Super Mario》 게임처럼 느껴지는 월드빌딩을 보여준다."
- **Nintendo Life (8/10)**: 칭찬과 함께 균형 문제를 지적 — "전투는 방대한 선택지와 난이도 사이의 불균형을 겪는다. 《Kingdom Battle》의 도전적이고 정교하게 짜인 전투와 뚜렷이 대비된다... 전투는 이전의 진화라기보다, 때로 Cursa의 위협을 사소하게 만들어버릴 만큼 자유와 창의성 쪽으로 이동했다."

### 수상 이력

| 시상식 (연도) | 결과 |
|------------------|------|
| The Game Awards 2022 — Best Sim/Strategy Game | 수상 |
| D.I.C.E. Awards 2023 — Family Game of the Year | 수상 |
| Ivor Novello Awards 2023 — Best Original Video Game Score | 수상 |
| Golden Joystick Awards 2022 | 후보 |
| BAFTA Games Awards 2023 | 후보 |
| Hollywood Music in Media Awards | 후보 |
| Kids' Choice Awards | 후보 |

전술 장르 최고작이자(TGA Best Sim/Strategy), 가족 친화적 게임(DICE Family Game of the Year), 그리고 사운드트랙(Ivor Novello)이라는 세 축에서 동시에 인정받았다는 점이 이 작품의 정체성을 잘 요약한다.

### 상업 지표 — "비평 성공, 상업 실망"의 괴리

여기서 이 게임의 가장 큰 역설이 드러난다. 평론·유저 반응은 좋았지만, **Ubisoft가 직접 "기대에 못 미쳤다(underperformed)"고 공식 발표**했다.

- Ubisoft는 2022년 말 실적 발표에서 "뛰어난 평점과 플레이어 반응, 야심 찬 마케팅 계획에도 불구하고, 《Mario + Rabbids: Sparks of Hope》가 2022년 마지막 몇 주와 2023년 1월 초에 부진한 데 놀랐다(surprised by the underperformance)"고 밝혔다(《GameSpot》, 《NME》).
- 일본 출시 첫 주 실물 판매는 17,647장으로 해당 주 소매 판매 3위에 그쳤다.
- 그러나 **2024년 1월 기준 약 300만 장(nearly 3 million copies)**을 판매했으며, VGC는 이 수치가 출시 후 동일 기간 기준으로 전작 《Kingdom Battle》과 대체로 비슷한 페이스라고 분석했다(《Nintendo Life》, 《ComicBook.com》). 즉 초반 부진은 시간이 지나며 상당 부분 회복됐다.

### 유저 평가

OpenCritic 96% 추천이 보여주듯 전문가 평가는 압도적으로 긍정적이었고, ResetEra·Famiboards 등 커뮤니티 리뷰 스레드에서도 전투 자유도와 사운드트랙은 호평이 주를 이뤘다. 반면 일부 유저는 "1편보다 너무 쉬워졌다", "오버월드 탐사·퍼즐이 늘어지고 산만하다"는 불만을 제기했다(6장 참조).

---

## 5. 성공 요인 분석

상업적으로는 "실망"으로 분류됐지만, **작품성·디자인 측면에서는 명백한 성공**이며 시리즈를 비평적으로 정점에 올린 작품이다. 그 요인을 분석한다.

### (1) "재발명할 용기" — 안전한 반복을 거부한 전투 설계

가장 큰 성공 요인은 역설적이게도 **위험을 감수한 재설계**다. Soliani는 인터뷰에서 "전작에서 사람들이 가장 좋아한 것이 전투 시스템이었지만, 우리는 진화하고 혁신해야 했고, 앞으로 나아갈 용기를 갖고 플레이어가 새로 시도할 진짜 이유를 제시하는 것이 중요했다"고 밝혔다. 그리드를 버린 자유 이동은 시리즈 정체성을 위협할 수도 있는 도박이었지만, 결과적으로 IGN·GameSpot이 "장르 최고의 턴 경제"라 부르는 차별점을 만들어냈다. 속편이 단순한 콘텐츠 추가가 아니라 **시스템 차원의 진화**를 택했다는 점이 평단의 높은 점수를 끌어냈다.

### (2) 닌텐도-Ubisoft 협업이라는 희소 자산

닌텐도가 외부에 마리오 IP를 맡긴 사례 자체가 마케팅·화제성의 핵심이었다. Soliani가 닌텐도에 "많은 것을 요청했고(특히 속편에서)" 수용·거절을 거치며 만든 작품은, 마리오 세계관의 정통성과 Ubisoft의 시스템 디자인 역량이 결합된 독특한 결과물이다. 이 협업의 신뢰는 1편의 성공으로 쌓였고, 속편은 그 신뢰를 더 큰 스코프로 갚았다.

### (3) 《Super Mario Odyssey》식 자유로 확장한 월드 디자인

Soliani는 탐사 중심 환경의 영감으로 "**자유(freedom)**"를 꼽았고, 《Super Mario Odyssey》 같은 비선형 모험 구조를 지향했다. 1편의 좁고 선형적인 복도형 진행에서 벗어나 다섯 행성을 자유롭게 누비는 구조로 확장함으로써, Eurogamer의 표현대로 "기대 이상으로 진짜 마리오 게임처럼 느껴지는" 경험을 만들었다.

### (4) 작곡가 드림팀이라는 차별화 마케팅 포인트

Grant Kirkhope·Yoko Shimomura·Gareth Coker라는 세 거장의 협업은 그 자체로 게임 음악 팬들에게 강력한 소구점이었다. 일본에서의 통일된 레코딩, Koji Kondo·Mahito Yokota의 감수는 "닌텐도 품질"을 보증하는 신호였고, Ivor Novello 수상으로 그 가치가 공인됐다. 음악은 비평·홍보 양면에서 작품의 격을 높였다.

### (5) 폭넓은 난이도 설계 = 시장 외연 확장

전투 전 자유로운 난이도 조정과 Relaxed/Average/Demanding 모드는 코어 전술 팬과 가족 단위 라이트 유저를 동시에 끌어안는 장치였다. DICE '올해의 가족 게임' 수상이 보여주듯, 닌텐도 플랫폼의 핵심 고객층(가족·전 연령)에 맞춘 접근성 설계가 작품의 시장 적합성을 높였다.

### (6) 전작 대비 차별점

| 항목 | 《Kingdom Battle》(2017) | 《Sparks of Hope》(2022) |
|------|--------------------------|---------------------------|
| 이동 | 그리드(칸) 기반 | 그리드 폐지, 자유 이동 |
| 진행 구조 | 선형 복도형 | 다섯 행성 비선형 탐사 |
| 능력 시스템 | 캐릭터 고정 스킬 트리 | Sparks 모듈 장착(인당 2개) |
| 난이도 | 도전적·정교한 큐레이션 | 유연 조정, 더 관대함 |
| 스케일 | 버섯 왕국 한정 | 우주 규모 |

---

## 6. 비평적 시각 / 한계 / 논란

호평작이지만 명백한 약점과 논쟁점도 존재한다.

### (1) 난이도 균형의 붕괴 — "너무 쉬워졌다"

가장 자주 지적된 약점이다. Nintendo Life는 "방대한 선택지와 난이도 사이의 불균형"을 정면으로 비판하며, 자유 이동·Sparks·팀 점프가 제공하는 막강한 옵션이 **적의 위협을 사소하게 만들어버린다(trivialise)**고 지적했다. 1편의 "도전적이고 정교하게 큐레이션된 전투"의 긴장감이 사라졌다는 평가다. 즉 접근성을 위한 관대한 설계가, 전술 게임 본연의 머리싸움을 즐기던 코어 팬에게는 손맛 손실로 다가왔다.

### (2) 오버월드 탐사·퍼즐의 늘어짐

비선형 행성 구조는 자유를 줬지만, 동시에 산만함을 낳았다. 일부 매체와 유저는 "혼란스러운 맵에서 전투를 찾아 헤매게 만들고, 지루하고 번거로운 퍼즐로 가득하다"고 비판했다. 전투의 질이 높은 만큼, 전투 사이를 잇는 탐사 구간이 오히려 페이스를 떨어뜨린다는 지적이다.

### (3) 산만한 스토리

여러 리뷰가 내러티브를 약점으로 꼽았다. GameSpot 리뷰 라운드업에서도 "스토리가 사방으로 흩어진다(all over the place)"는 평가가 있었으며, 전반적으로 스토리는 전투 메카닉만큼의 집중 투자를 받지 못했다는 것이 중론이다.

### (4) 기술적 한계 — 로딩과 프레임

Snowdrop 엔진으로 더 큰 스코프를 추구한 대가로 **로딩 시간**과 Switch의 성능 한계에서 오는 안정성 문제가 다수 리뷰에서 지적됐다. "Switch가 모든 것을 항상 부드럽게 처리하진 못한다"는 평가가 대표적이다.

### (5) 상업 부진과 그 후폭풍 — 개발팀이 입은 상처

작품 외적 논란으로, **Ubisoft의 "기대 미달" 공식 발표가 개발팀에 남긴 상처**가 있다. Soliani는 "우리는 3년 반 동안 일했고 정말 좋은 게임을 만드는 데 전력을 다했다. 게임 성과에 대해 받은 메시지는 팀 사기에 다소 상처가 됐다(a bit hurtful for the morale of the team)"고 토로했다. 출시 타이밍이 《Call of Duty: Modern Warfare II》, 《Pokémon Scarlet/Violet》, 《God of War Ragnarök》 같은 초대형 작품들과 겹친 점, 메가 브랜드·라이브 서비스가 소비자 지출을 흡수하던 시장 환경(《TheGamer》 분석)이 부진의 외부 요인으로 꼽힌다. 즉 작품 자체의 질이 아니라 **타이밍과 시장 구조**가 초반 판매 부진의 핵심이었다는 분석이다.

---

## 7. 영향과 유산

### 장르적 의미 — "친근한 전술 게임"의 완성형

《Sparks of Hope》는 1편이 개척한 "콘솔에서 즐기는 친근하고 접근성 높은 턴제 전술" 노선을 정점으로 끌어올렸다. 《XCOM》·《Fire Emblem》처럼 진입 장벽이 높던 전술 장르를, 마리오의 친화력과 자유 이동·유연 난이도로 전 연령 대중에게 열었다는 점에서 의미가 크다. TGA Best Sim/Strategy 수상은 이를 공인한다. 특히 그리드를 버린 자유 이동 전투는 "턴제 전술이 반드시 격자에 갇혀야 하는가"라는 질문을 던진 디자인 실험으로 기록된다.

### IP·산업적 의미 — 닌텐도 외부 협업 모델의 성공 사례

이 시리즈는 닌텐도가 핵심 IP를 외부 스튜디오에 맡겼을 때 양질의 결과가 나올 수 있음을 보여준 드문 성공 사례다. 1편과 속편 합산으로 시리즈는 상업·비평 모두에서 안정적 성과를 냈고, 닌텐도-서드파티 라이선스 협업의 청사진이 됐다.

### DLC와 사후 지원

2023년 세 개의 유료 DLC로 콘텐츠를 확장했다.

- **The Tower of Doooom** (2023년 3월 2일) — Spawny를 구하는 던전형 도전 콘텐츠.
- **The Last Spark Hunter** (2023년 6월 21일) — Melodic Gardens를 배경으로 네 번째 Spark Hunter인 신규 캐릭터 Kanya 등장.
- **Rayman in the Phantom Show** (2023년 8월 30일) — Ubisoft의 간판 캐릭터 **Rayman**이 Rabbid Mario·Rabbid Peach와 함께 영화 스튜디오를 무대로 활약. Rayman의 정식 게임 복귀를 알린 화제의 DLC로, Ubisoft IP끼리의 크로스오버라는 점에서도 의미가 컸다.

### 개발진의 그 이후 — Soliani의 독립

상업 부진을 둘러싼 갈등 이후, 디렉터 Davide Soliani는 Ubisoft를 떠나 독립 스튜디오 **Day 4 Night**를 설립했다. 이 스튜디오에는 《Red Dead Redemption》의 Christian Cantamessa, 그리고 본작의 작곡가이자 《Banjo-Kazooie》의 Grant Kirkhope가 합류했다. Soliani는 "닌텐도와 함께한 시간은 환상적이었다"며 향후 닌텐도와의 재협업에도 열려 있다는 의사를 밝혔다(《Nintendo Life》, 2025). 즉 이 프로젝트는 한 시대 협업의 마침표인 동시에, 핵심 인재들의 새로운 출발점이 됐다.

### 문화적 의미

마리오 시리즈 정규 라인에서 성우 Charles Martinet의 목소리가 담긴 사실상 마지막 작품 중 하나라는 상징성, 그리고 "농담 같은 발상도 진정성과 디자인 역량으로 명작이 될 수 있다"는 1편의 교훈을 한 번 더 입증한 점에서, 이 작품은 게임 업계의 "의외성의 성공" 신화의 한 챕터로 남았다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 수치 / 내용 |
|------|-------------|
| Metacritic (Switch) | 85/100 (약 122개 리뷰) |
| OpenCritic 추천율 | 96% (약 127개 리뷰) |
| 출시일 | 2022년 10월 20일 (Switch 독점) |
| 개발 기간 | 약 3년 반 |
| 누적 판매 | 약 300만 장 (2024년 1월 기준) |
| 일본 출시 첫 주 실물 | 17,647장 (해당 주 소매 3위) |
| 사운드트랙 트랙 수 | 52곡 |
| DLC | 3종 (2023년) |
| 주요 수상 | TGA Best Sim/Strategy 2022, DICE Family Game of the Year 2023, Ivor Novello Best Original Video Game Score 2023 |

### 주요 인물

- **Davide Soliani** — 크리에이티브 디렉터. 시리즈의 얼굴. 현재 독립 스튜디오 Day 4 Night 설립.
- **Damiano Moro** — 공동 디렉터.
- **Xavier Manzanares** — 브랜드 프로듀서 / 리드 디자이너, 시리즈 공동 기획자.
- **Grant Kirkhope / Yoko Shimomura / Gareth Coker** — 작곡 3인방.
- **Shigeru Miyamoto** — 닌텐도 측 협업 파트너, 1편 E3 발표 동반.

### 주요 인터뷰 / 자료

- Davide Soliani 인터뷰 (ComicBook.com): 영감·닌텐도와의 협업·제약. https://comicbook.com/gaming/news/mario-rabbids-sparks-of-hope-david-soliani-interview-nintendo-switch/
- Davide Soliani 인터뷰 (GamesHub): 전투·월드 설계 의도. https://www.gameshub.com/news/features/mario-rabbids-sparks-of-hope-interview-davide-soliani-combat-worlds-22770/
- "Ubisoft 측 '실망' 발언과 개발팀 반응" (Nintendo Everything): https://nintendoeverything.com/mario-rabbids-sparks-of-hope-director-harder-to-make-than-kingdom-battle-ubisofts-comments-were-a-bit-hurtful/
- Snowdrop·Switch 경험과 스코프 확장 (Nintendo Everything): https://nintendoeverything.com/mario-rabbids-sparks-of-hope-teams-experience-with-switch-and-snowdrop-engine-allowed-for-bigger-scope/

### 참고 자료 목록 (영어권 매체 중심)

- 《Wikipedia》 — Mario + Rabbids Sparks of Hope: https://en.wikipedia.org/wiki/Mario_+_Rabbids_Sparks_of_Hope
- 《Wikipedia》 — Mario + Rabbids Kingdom Battle (시리즈 기원): https://en.wikipedia.org/wiki/Mario_+_Rabbids_Kingdom_Battle
- 《Metacritic》 — 평론/유저 점수: https://www.metacritic.com/game/mario-plus-rabbids-sparks-of-hope/
- 《GameSpot》 — 리뷰("This Sparks Joy") 및 리뷰 라운드업, 상업 실적 기사: https://www.gamespot.com/reviews/mario-rabbids-sparks-of-hope-review-this-sparks-joy/1900-6417985/
- 《GameSpot》 — Ubisoft "Surprised" By Lackluster Sales: https://www.gamespot.com/articles/ubisoft-surprised-by-lackluster-sales-of-mario-rabbids-sparks-of-hope/1100-6510517/
- 《Game Informer》 — Refining The Formula: https://gameinformer.com/review/mario-rabbids-sparks-of-hope/refining-the-formula
- 《Nintendo Life》 — 리뷰(8/10) 및 판매 회복 기사: https://www.nintendolife.com/reviews/nintendo-switch/mario-plus-rabbids-sparks-of-hope
- 《Polygon》·《Eurogamer》·《IGN》 리뷰 (ResetEra/Famiboards 리뷰 스레드 종합): https://www.resetera.com/threads/mario-rabbids-sparks-of-hope-review-thread.644358/
- 《NME》 — 작곡가 라인업 및 판매 부진 보도: https://www.nme.com/news/gaming-news/ubisoft-surprised-by-mario-rabbids-sparks-of-hope-low-sales-3379523
- 《TheGamer》 — "How Could Mario + Rabbids 2 Fail?" (부진 원인 분석): https://www.thegamer.com/mario-rabbids-sparks-of-hope-underperformed-reason-ubisoft/
- 《Super Mario Wiki》 — 사운드트랙: https://www.mariowiki.com/Mario_+_Rabbids_Sparks_of_Hope_(Original_Game_Soundtrack)
- 《Game8》 — Battle System and Combat Guide: https://game8.co/games/Mario-Rabbids-Sparks-of-Hope/archives/393366
- 《Game Rant》 — Difficulty Levels Explained: https://gamerant.com/mario-rabbids-sparks-of-hope-difficulty-levels-relaxed-average-demanding/

---

*본 분석서는 영어권 매체·개발자 인터뷰·공식 자료를 토대로 작성되었으며, 판매·점수 등 수치는 각 출처 기준이다. 일부 수치는 보고 시점에 따라 갱신될 수 있다.*
