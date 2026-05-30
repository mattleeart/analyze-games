# Mortal Kombat 1 (2023) 심층 분석

> 30년 넘은 격투 IP가 자기 역사를 두 번째로 리셋하다. 《Mortal Kombat 1》은 시리즈가 가장 야심 차게 다시 시작한 작품이면서, 동시에 격투게임 장르의 구조적 딜레마—"신선한 메카닉" vs "콘텐츠 깊이와 모네타이제이션의 무게"—를 가장 적나라하게 드러낸 사례다. 본 분석은 영어권 매체·개발자 발언·판매 데이터·커뮤니티 반응을 토대로, 이 게임이 왜 비평적으로 호평받으면서도 유저 사이에서는 의견이 갈렸는지, 그리고 시리즈와 장르에 무엇을 남겼는지를 자세히 다룬다.

---

## 1. 게임 개요

《Mortal Kombat 1》은 **NetherRealm Studios**가 개발하고 **Warner Bros. Games**(WB Interactive Entertainment)가 퍼블리싱한 2D 평면 기반 3D 격투게임이다. 2023년 9월 19일 PlayStation 5, Xbox Series X|S, Nintendo Switch, PC(Steam·Epic Games Store)로 정식 출시되었으며, 프리미엄·디럭스 에디션 구매자에게는 9월 14일 얼리 액세스가 제공되었다. 한국·일본을 포함한 글로벌 동시 발매였다.

이 작품의 가장 큰 출시 전략적 특징은 **PlayStation 4와 Xbox One을 완전히 건너뛴 첫 메이저 격투게임**이라는 점이다. 즉 처음부터 PS5·Xbox Series 세대만을 타깃으로 설계되어, 구세대 콘솔의 하드웨어 한계에 발목 잡히지 않고 비주얼과 렌더링을 끌어올릴 수 있었다(다만 Switch는 별개의 문제를 안았는데, 후술한다). 가격은 전 플랫폼 공통 **$70**로 책정되었다.

### 개발 주체와 크레딧

- **디렉터/총괄**: **Ed Boon**. 1992년 원작 《Mortal Kombat》의 공동 창작자이자 NetherRealm Studios의 수장으로, 시리즈의 정체성을 30년 넘게 지켜온 인물이다.
- **개발사**: NetherRealm Studios(시카고 소재). 《Mortal Kombat》 리부트(2011)·《MKX》·《MK11》, 그리고 《Injustice》 시리즈를 만든 스튜디오.
- **퍼블리셔**: Warner Bros. Games. 모회사 Warner Bros. Discovery(WBD).
- **성우**: Liu Kang은 Matthew Yang King, Johnny Cage는 Andrew Bowen 등이 맡았으며, 시리즈 전통대로 풀 모션 캡처와 페이셜 캡처가 적용되었다.

### 개발 기간·엔진

가장 주목할 기술적 사실은 **엔진 교체**다. 시리즈는 오랜 기간 *heavily modified* 버전의 **Unreal Engine 3**를 사용해 왔는데, 《Mortal Kombat 1》에서 NetherRealm은 마침내 **Unreal Engine 4**로 베이스를 옮겼다. Ed Boon은 인터뷰에서 "엔진 업그레이드 때문에 《Injustice 3》보다 《Mortal Kombat 1》을 먼저 만들게 됐다"고 밝혔다. 즉 새 엔진을 길들이고 그 위에서 비주얼·메카닉을 새로 설계하는 작업이 이번 작품의 핵심 동력이었던 셈이다. (Ed Boon은 본작이 Unreal Engine 5가 아닌 UE4 기반임을 명시했다.)

개발은 2020년경 시작되었다. 원래는 2022년 출시를 목표로 했으나, COVID-19 팬데믹을 비롯한 여러 요인으로 2023년으로 연기되었다. NetherRealm은 자사의 대략 2년 주기 출시 리듬(MK ↔ Injustice 교대)을 유지해 왔는데, 본작은 그 리듬 안에서 "엔진 세대 교체"라는 무거운 과제를 짊어진 타이틀이었다.

본작은 《Mortal Kombat 11》(2019)의 직접적 후속이자, 2011년 리부트에 이은 **시리즈 두 번째 리부트**다. 다만 완전한 백지화가 아니라, 전작 스토리에서 자연스럽게 이어지는 "**소프트 리부트**"라는 점이 중요하다(상세는 2장).

---

## 2. 게임 설명 — 무엇을 다시 시작했는가

### 컨셉과 세계관: "New Era"

《Mortal Kombat 1》의 세계관은 **"New Era"(새 시대)**라는 이름의 완전히 재창조된 타임라인 위에 서 있다. 이는 전작 《MK11》과 그 확장 《MK11: Aftermath》의 직접적 결과다.

[스포일러] 전작에서 시간의 신 Kronika와 Shang Tsung을 물리친 **Fire God Liu Kang(불의 신 류 캉)**은, Kronika의 신물 **Hourglass(모래시계)**를 손에 넣어 우주를 통째로 재창조한다. 그러나 Liu Kang은 자신이 Kronika처럼 권력에 미쳐버릴까 두려워, 시간의 타이탄 권좌를 내려놓고 새로 태어난 **Geras**에게 Hourglass의 수호를 맡긴다. 그리고 자신은 한 발 물러나 **Earthrealm(지구계)의 수호신**이 된다.

이 New Era에서 Liu Kang은 Outworld(외계)의 故 **King Jerrod**와 협력해, 과거에는 외계가 지구를 침략하기 위한 수단이었던 **Mortal Kombat 토너먼트**를 두 세계의 평화로운 교류 행사로 재정립한다. 즉 시리즈 30년의 기본 전제—"지구를 지키기 위한 사활을 건 무술 대회"—자체가 근본부터 다시 쓰인 것이다. 이것이 본작의 서사적 야심의 핵심이다.

### 캐릭터의 재해석

Liu Kang이 운명을 다시 짠 결과, 익숙한 캐릭터들이 전혀 다른 배경을 갖게 되었다. 이 "익숙한 얼굴, 낯선 사연"이 본작 스토리 모드의 가장 큰 재미 요소다.

- **Raiden(라이덴)**: 더 이상 천둥의 신이 아니다. New Era의 Raiden은 무술에 뛰어난 **평범한 농부**로, Liu Kang의 가르침을 받아 Earthrealm의 챔피언으로 선발된다. 시리즈 최강의 신격 캐릭터가 인간 주인공으로 강등된 것은 상징적이다.
- **Lin Kuei(린 쿠에이)**: 과거의 암살자 집단이 아니라 Earthrealm의 고대 수호 가문이다. 가장 큰 변화는 **Scorpion, Sub-Zero, Smoke가 형제**가 되었다는 점. 이번 Scorpion은 Kuai Liang으로, Sub-Zero인 형 Bi-Han의 동생이며, Smoke(Tomas Vrbada)는 그랜드마스터가 입양한 또 다른 형제다. 시리즈 역사상 처음으로 이 세 명이 한 팀으로 함께 싸운다—수십 년간 숙적이던 Scorpion과 Sub-Zero의 관계를 통째로 뒤집은 것이다.
- **Shang Tsung(샹 쑹)**: 한때 영혼을 빨아먹던 강력한 마법사가, New Era에서는 가짜 약을 파는 **돌팔이 약장수(snake oil salesman)**로 전락했다. Liu Kang이 가한 가장 잔인하고 모욕적인 운명 개변이라 할 만하다.
- **그 외**: Kung Lao는 농부, **Johnny Cage**는 한물간 헐리우드 배우, **Kenshi Takahashi**는 전직 야쿠자 조직원으로 등장한다.

### 줄거리

[스포일러] 메인 플롯은 Liu Kang이 Kung Lao·Raiden(농장 일꾼들), 재정난에 시달리는 배우 Johnny Cage, 전직 야쿠자 Kenshi를 토너먼트 참가자로 모으는 데서 출발한다. 한편 무력해진 약장수 Shang Tsung은 **"Damashi"**라는 의문의 인물의 접근을 받는다. Damashi는 그에게 사실은 위대한 마법사가 될 잠재력이 있으며, 보이지 않는 힘이 그를 방해해 왔다고 속삭인다.

이야기가 진행되며 Raiden이 토너먼트에서 우승해 Earthrealm 챔피언이 되지만, 진짜 위협은 따로 있었다. **Damashi의 정체는 다른 타임라인의 Shang Tsung—이른바 "Titan Shang Tsung"**이었다. Fire God Liu Kang이 New Era를 만든 것처럼, 또 다른 타임라인에서는 Shang Tsung이 시간의 타이탄이 되어 자기만의 우주를 창조했고, 그 Titan Shang Tsung이 Liu Kang의 타임라인을 침략하려 한 것이다.

엔딩에서 Fire God Liu Kang과 Titan Shang Tsung은 각자 **여러 타임라인(멀티버스)에서 군대를 소집**한다. 두 군대가 충돌하고, 결국 Liu Kang 진영의 한 멤버가 Titan Shang Tsung을 쓰러뜨린다. Liu Kang은 Titan Shang Tsung과 그 동맹 Quan Chi를 먼지로 만들어 그 타임라인을 붕괴시킨다. 이 멀티버스적 클라이맥스는 후속 콘텐츠(Khaos Reigns)로 이어지는 떡밥을 남긴다.

### 무드·톤·아트 디렉션

《Mortal Kombat》 특유의 **고어와 블랙코미디의 공존**은 그대로다. UE4로의 전환 덕에 캐릭터 모델·피부 질감·근육 디테일·X-Ray 연출(Fatal Blow/Fatality 시 뼈와 장기가 부서지는 슬로모션)이 한층 사실적으로 표현되었다. 한편 Johnny Cage의 헐리우드 메타 개그, Shang Tsung의 약장수 코미디 등으로 시리즈 특유의 자조적 유머도 강화되었다. 스토리 모드는 영화적 컷신과 인터랙티브 전투를 매끄럽게 엮는 NetherRealm 특유의 시네마틱 연출을 다시금 보여 준다.

---

## 3. 핵심 시스템 / 메카닉 — Kameo Fighters

### 코어 루프와 가장 큰 변화: Kameo 시스템

《Mortal Kombat 1》의 게임플레이를 한 단어로 요약하면 **"Kameo"**다. 본작 전투의 근본 구조는 **변형된 2v2** 방식이다. 플레이어는 직접 조작하는 **메인 파이터** 한 명을 고르고, 그와 별개로 **Kameo Fighter(어시스트 파트너)** 한 명을 고른다. Kameo는 직접 조작하는 캐릭터가 아니라, **Kameo 전용 버튼**을 눌러 호출하는 보조 캐릭터다.

핵심 작동 방식은 다음과 같다.

- **방향 입력 + Kameo 버튼**의 조합에 따라 Kameo가 서로 다른 기술을 사용한다. 예컨대 Kameo 버튼만 누르면 A 기술, 아래 방향과 함께 누르면 B 기술이 나가는 식이다.
- Kameo의 기술은 단순 추가 공격에 그치지 않는다. **추가 special move, throw(잡기), breaker(콤보 탈출)** 등 공격과 방어 양쪽 모두에 쓰인다. 즉 Kameo는 메인 캐릭터의 콤보를 연장하거나, 압박을 강화하거나, 위기에서 빠져나오는 다용도 도구다.
- **Fatal Blow와 Fatality에도 Kameo가 관여**한다. 본작의 화려한 Fatal Blow 연출 절반을 Kameo가 담당하며, Kameo는 **자신만의 고유 Fatality**도 갖는다.

이 시스템의 디자인 의도는 명확하다. 같은 메인 캐릭터라도 어떤 Kameo와 조합하느냐에 따라 콤보 루트·압박·방어 옵션이 완전히 달라진다. 메인 로스터 × Kameo 로스터의 곱으로 **조합의 가짓수가 폭발적으로 늘어나며**, 시리즈 역사상 가장 큰 메카닉 변화이자 메타게임의 깊이를 한 단계 끌어올린 변수다. 런칭 시점 Kameo는 총 **15명**으로, 그중 10명은 부팅 직후 바로 사용 가능하고 나머지 5명은 플레이를 통해 언락한다.

GameSpot은 리뷰에서 "훌륭한 메카닉과 거친 스토리가 견고한 첫인상을 만든다(Great mechanics and a wild story make a solid first impression)"고 평하며 Kameo 시스템을 본작 게임플레이의 핵심 강점으로 꼽았다.

### 진행 구조와 모드

본작은 격투게임의 표준 구성(스토리·아케이드·온라인·튜토리얼)에 더해 두 가지 굵직한 싱글플레이어 축을 갖는다.

**Story Mode**는 약 5~6시간 분량의 영화적 캠페인으로, 위 2장에서 설명한 New Era 서사를 따라간다. NetherRealm은 시리즈 전통대로 컷신과 전투를 매끄럽게 엮어, 격투게임 중 가장 잘 만든 시네마틱 캠페인이라는 평가를 다시 한 번 받았다. IGN의 Mitchell Saltzman은 특히 복귀 캐릭터들이 새 백스토리를 얻은 점을 호평했다.

**Invasions**는 본작의 신규 싱글플레이어 모드로, 과거의 **Krypt(보상 탐험)와 Towers(연승전)를 대체·진화**시킨 형태다. 컨셉은 **보드게임**이다. 플레이어는 보드의 칸들을 이동하며 적과 싸우고, 아이템과 탈리스만을 줍고, 상징적인 MK 로케일의 미니 버전을 탐험한다. 내레이션은 Johnny Cage가 맡아 특유의 유머를 더한다. Ed Boon은 이 모드를 두고 "도시 몇 블록을 덮을 만큼 큰 보드게임 같다"고 표현했다. Invasions는 **시즌제**로 운영되어, 시즌마다 새로운 보드·적·보상이 추가되도록 설계되었다.

### 난이도·접근성·UI

본작은 캐주얼 진입을 돕는 장치를 다수 갖췄다. 대표적으로 **Easy Fatality** 기능이 있는데, 입력이 까다로운 Fatality를 간소화된 커맨드로 발동할 수 있게 해 준다(이 기능이 유료 토큰과 결합되어 논란이 된 점은 6장에서 다룬다). 또한 시리즈 전통의 친절한 튜토리얼, 콤보 트라이얼, 프레임 데이터 표시 등 학습 도구를 제공한다.

### 라이브 운영·시즌 패스·모네타이제이션

본작은 출시 후 장기 운영을 전제로 한 다중 화폐 구조를 갖는다.

- **Koins**: 기본 인게임 화폐(플레이로 획득, 상점 구매에 사용).
- **Seasonal Kredits**: Invasions 시즌 진행으로 얻는 시즌 한정 화폐.
- **Krowns**: 추가 보상 화폐.
- **Dragon Krystals**: **실제 돈으로 구매하는 유일한 프리미엄 화폐**. 가격은 500개 $5, 1,150개 $10, 2,500개 $20, 5,600개 $40. 코스메틱(스킨·장신구 등)과 **Easy Fatality Token** 등 소비성 자원을 산다.

중요한 점은, Dragon Krystals로 **게임플레이를 직접 강화하는 아이템은 살 수 없다**는 것이다. 즉 페이투윈 요소는 아니다. 그럼에도 여러 통화의 복잡성과 Easy Fatality의 유료화는 비판의 빌미가 되었다.

---

## 4. 평가

### 비평 점수

《Mortal Kombat 1》은 출시 시점 **강력한 비평적 호평**을 받았다. Metacritic 기준 **PS5 버전 86점**, OpenCritic에서는 평론가의 **94%가 추천**했다.

| 매체 | 점수 | 핵심 평 |
| --- | --- | --- |
| Game Informer | 9/10 | 시리즈 복귀작이자 새 방향 제시 |
| GamesRadar+ | 5/5 | "An exceptional, confident fighting game"(뛰어나고 자신감 있는 격투게임) |
| IGN (Mitchell Saltzman) | 8/10 | 스토리 모드와 복귀 캐릭터의 새 백스토리 호평 |
| GameSpot | 8/10 | "New Era, Familiar Kombat" — 좋은 메카닉·거친 스토리, 그러나 모드 다양성 부족 |
| Push Square | 7/10 | "2011 이후 가장 신선한 작품, 그러나 같은 함정에 빠진다" |

대표 평을 인용하면 다음과 같다.

- GameSpot: "Great mechanics and a wild story make a solid first impression, but a shallow selection of modes keeps MK1 from a flawless victory."(훌륭한 메카닉과 거친 스토리가 견고한 첫인상을 만들지만, 빈약한 모드 선택이 MK1을 완벽한 승리에서 멀어지게 한다.)
- Push Square: "Mortal Kombat 1 is the best and most refreshing entry in the series since Mortal Kombat (2011), but it falls directly into the same traps as those prior entries."(2011년 이후 시리즈에서 가장 좋고 신선한 작품이지만, 이전작들과 똑같은 함정에 그대로 빠진다.)
- 일부 매체: "It's the perfect entry point for newcomers and long time fans of the series."(신규 유저와 오랜 팬 모두에게 완벽한 진입점이다.)

요약하면 비평가들은 **Kameo 시스템·재해석된 세계관·시네마틱 스토리·전투의 손맛**을 높이 샀고, 동시에 **모드 다양성·콘텐츠 깊이·시리즈가 반복하는 모네타이제이션 습관**을 한계로 지적했다.

### 유저 평가와 비평-유저 괴리

비평과 달리 **유저 평가는 뚜렷이 갈렸다**. Metacritic 유저 스코어는 약 **6.5**, Steam은 초기 21,751개 리뷰 기준 **Mixed 69% 긍정**, 이후 누적 36,020개 리뷰 기준 **70/100 Mixed** 수준에 머물렀다. 비평가 평균(83~86점대)과 유저 점수(65~70점대) 사이에 **명확한 괴리**가 존재한다.

유저 불만의 핵심은 다음과 같다.

- **로스터 깊이와 모드 다양성** 부족.
- **모네타이제이션**(다중 화폐, 유료 코스메틱, Easy Fatality 토큰)에 대한 거부감.
- 전작 **MK11 대비 체감 다운그레이드**(특히 Switch 버전과 일부 시스템).
- WB가 후일 **레거시 DLC를 별도 판매**한 것에 대한 "탐욕(greed)" 비판.

반대로 긍정 측은 PC·콘솔에서의 최적화, 시각적 완성도, 신규 유저에게 친절한 진입성, Kameo의 신선함을 들었다.

### 상업 지표

- 출시 직후 WBD CEO David Zaslav는 2023년 11월 "MK1이 9월 중순 출시 이후 거의 **300만 장**을 팔았다"고 언급했다. PS4/Xbox One을 건너뛴 격투게임으로서는 강한 수치였다.
- 2023년 9월 **미국 월간 판매 2위**.
- 이후 판매는 꾸준히 증가해 **2024년 8월 400만+**, **2025년 1월 500만**, **2025년 8월 620만**을 기록했고, 최근에는 **800만 장 이상**을 돌파한 것으로 보고되었다.
- 다만 전작 **《Mortal Kombat 11》은 1,500만 장**을 팔았는데, MK1은 그에 한참 못 미쳤다. 이 격차가 후술할 DLC 지원 조기 종료의 직접적 배경이 된다.

---

## 5. 성공 요인 분석

### (1) 디자인: "리부트의 명분"을 메카닉과 서사로 동시에 제공

NetherRealm은 본작에서 두 가지를 동시에 새로 했다. 하나는 **Kameo라는 신규 코어 메카닉**, 다른 하나는 **New Era라는 세계관 리셋**이다. 이 둘이 맞물리면서 "왜 또 새 MK를 사야 하는가?"라는 질문에 대한 명분이 분명해졌다. Kameo는 오랜 팬에게도 새 메타게임을 학습할 동기를 주었고, New Era는 익숙한 캐릭터를 낯선 사연으로 다시 만나게 해 서사적 신선함을 제공했다. 비평가들이 "시리즈 복귀작(return to form)이자 의미 있는 새 방향"이라고 평한 것은 이 이중 혁신 덕분이다.

### (2) 출시 전략: 차세대 전용 + IP 게스트 마케팅

PS4/Xbox One을 버리고 **차세대 전용**으로 간 결정은 비주얼 상한을 끌어올렸고, "최신 하드웨어에서 가장 화려한 격투게임"이라는 포지셔닝을 가능케 했다. 또한 NetherRealm은 시리즈 전매특허인 **대중문화 게스트 캐릭터** 마케팅을 적극 활용했다. 출시 후 Kombat Pack 1에 《The Boys》의 Homelander, 《Invincible》의 Omni-Man, DC/존 시나의 Peacemaker를 투입해, 격투게임 팬뿐 아니라 해당 IP 팬덤의 화제를 끌어모았다. 이 게스트 라인업은 커뮤니티에서 폭넓은 호응을 얻었다.

### (3) 타이밍과 시장 환경

2023년은 차세대 콘솔 보급이 충분히 진행된 시점이었고, 격투게임 장르 자체가 《Street Fighter 6》(2023) 등으로 다시 주목받던 해였다. MK1은 이 격투게임 부흥기의 한 축을 담당하며, 미국에서 9월 월간 2위에 오르는 강한 초동을 기록했다.

### (4) 운영 방법론: 시네마틱 스토리 + 시즌제 싱글플레이

NetherRealm의 차별화된 강점은 **격투게임 중 압도적으로 잘 만든 싱글플레이어 콘텐츠**다. 영화적 스토리 모드는 격투게임에 관심 없던 라이트 유저까지 끌어들이는 입구 역할을 했고, Invasions의 시즌제는 출시 후에도 유저를 붙잡아 두는 장치로 설계되었다. 격투게임이 "온라인 대전만의 장르"라는 통념을 NetherRealm은 꾸준히 깨 왔고, 본작도 그 전략을 계승했다.

### (5) 동시기 작품 대비 차별점

같은 해 출시된 《Street Fighter 6》가 모던/클래식 조작과 월드 투어 모드로 진입성과 콘텐츠를 강화했다면, MK1은 **Kameo의 조합 깊이 + 고어 연출 + 시네마틱 스토리 + 멀티버스 서사**라는 자기만의 색으로 차별화했다. 즉 두 작품은 "격투게임의 대중화"라는 같은 목표를 서로 다른 방법으로 추구하며 장르 전체의 파이를 키웠다.

---

## 6. 비평적 시각 / 한계 / 논란

### (1) Nintendo Switch 포트 참사

본작에서 가장 큰 논란은 단연 **Switch 버전의 처참한 품질**이었다. 출시 직후 다수 매체와 유저가 Switch 포트를 "거의 플레이 불가(nearly unplayable)", 심지어 "쓰레기(garbage)"라고 혹평했다(TechRadar, Dexerto, VGC, GamesRadar 등).

구체적 문제는 다음과 같다.

- **성능**: 60fps를 목표로 했으나 특정 기술 발동 시 심각한 프레임 드랍.
- **그래픽**: "PS2 시대 수준"이라는 비교가 나올 만큼 큰 해상도 저하와 비주얼 글리치(직물·스트레칭 오류 등).
- **로딩**: 전투 사이 로딩이 길고, 메뉴 반응이 둔함.
- **버그**: Invasion 모드의 게임브레이킹 버그.
- **콘텐츠 누락**: 런칭 시 Switch판은 Invasions 본편 콘텐츠가 빠진 채 **"도입부만"** 제공되었고, 정식 시즌 콘텐츠는 출시 몇 주 뒤에야 들어왔다. WB는 "최상의 경험을 위해 출시 시점엔 도입부만 제공한다"고 해명했다.

문제를 키운 결정타는 **가격**이었다. Switch판도 다른 플랫폼과 **동일한 $70**였기 때문에, 압도적으로 낮은 품질을 프리미엄 가격에 사야 한다는 점에서 강한 반발을 샀다.

### (2) 모네타이제이션과 "WB의 탐욕"

비록 페이투윈은 아니었지만, **다중 화폐 구조의 복잡성**과 **Easy Fatality의 유료 토큰화**는 거듭 비판받았다. 입력이 어려운 Fatality를 돈으로 손쉽게 발동하게 만든 설계는 "연출을 인질로 삼은 과금"이라는 인상을 주었다. 또한 후일 WB가 레거시 DLC를 별도로 판매하는 방식이 커뮤니티에서 "탐욕"이라는 강한 단어로 비판받았다.

### (3) 모드 다양성·콘텐츠 깊이 부족

여러 비평가가 공통적으로 지적한 한계다. GameSpot은 "빈약한 모드 선택이 완벽한 승리를 막는다"고 했고, Push Square는 "신선하지만 이전작과 같은 함정에 빠진다"고 평했다. 특히 **Invasions 모드**는 비평·유저 양쪽에서 **호불호가 갈렸다**. 보드게임 컨셉의 신선함은 인정받았으나, 실제로는 약한 적과의 반복 전투를 끝없이 치르며 느리게 떨어지는 보상을 모으는 **지루한 그라인드**라는 비판이 많았다. 일부는 싱글플레이 요소가 온라인 연결을 요구해 오프라인에서 자유롭게 즐길 수 없다는 점도 문제 삼았다.

### (4) 비평-유저 괴리의 본질

86점의 비평 점수와 6.5~7.0의 유저 점수 사이의 간극은, 본작이 "**전투와 첫인상은 훌륭하지만, 장기적으로 붙들어 둘 콘텐츠 깊이와 운영 신뢰가 부족하다**"는 격투게임 장르의 고질적 딜레마를 그대로 보여 준다. 비평가는 출시 시점의 완성도를 보고, 유저는 수십~수백 시간을 플레이하며 그라인드·과금·로스터 한계를 체감하기 때문이다.

---

## 7. 영향과 유산

### 시리즈 안에서의 의미

《Mortal Kombat 1》은 시리즈에 두 가지를 남겼다. 첫째, **엔진 세대 교체**(UE3 → UE4)를 완수해 NetherRealm의 기술 기반을 다음 10년 분량으로 갱신했다. 둘째, **타임라인을 다시 한 번 리셋**해 향후 서사 확장의 멀티버스적 토대를 마련했다. Titan Shang Tsung·멀티버스 군대 같은 장치는 게스트 캐릭터의 등장과 후속 스토리를 정당화하는 서사적 그릇이 되었다.

### 장르에 미친 영향: Kameo 어시스트의 재해석

태그·어시스트 메카닉 자체는 격투게임 역사에서 새롭지 않다(《Marvel vs. Capcom》 등). 그러나 MK1은 이를 **메인 1 + 호출형 어시스트 1**이라는 형태로 다듬어, 메인 캐릭터를 완전히 교체하지 않으면서도 조합 다양성을 폭발시키는 방식을 대중적으로 제시했다. 같은 해 《Street Fighter 6》의 모던 조작과 함께, 2023년은 메이저 격투게임이 **진입성과 표현 다양성을 동시에 넓힌 해**로 기록된다.

### 후속 콘텐츠와 운영의 궤적

- **Kombat Pack 1**: Ermac·Quan Chi·Takeda(복귀) + Homelander·Omni-Man·Peacemaker(게스트). 게스트 라인업이 특히 화제가 되었다.
- **《Khaos Reigns》 확장팩 (2024)**: 신규 스토리 챕터 + **Kombat Pack 2**(Cyrax·Sektor·Noob Saibot + 게스트 Ghostface《Scream》·T-1000《Terminator 2》·Conan the Barbarian). 멀티버스 떡밥을 본편 후일담으로 회수했다.
- **DLC 지원 조기 종료**: 판매가 전작 MK11(1,500만)에 크게 못 미친다는 것이 분명해지자, WB는 추가 DLC 지원을 비교적 이른 시점에 중단했다. 이는 본작의 운영사에서 가장 아쉬운 대목이다.
- **Definitive Edition (2025년 5월 14일)**: NetherRealm은 출시 후 전 콘텐츠를 묶은 디피니티브 에디션을 내놓으며, 게임 지원은 계속하되 **추가 캐릭터·스토리 챕터는 더 이상 계획에 없다**고 확정했다.

### 산업적·문화적 의미

MK1은 "**차세대 전용 출시가 격투게임에서도 가능하다**"는 것을 상업적으로 입증한 사례다. 동시에, 강한 비평 점수와 800만 장 이상의 누적 판매에도 불구하고 전작에 못 미친 성과는, **격투게임에서 콘텐츠 깊이·운영 신뢰·합리적 가격 정책이 초동 화제 못지않게 장기 매출을 좌우한다**는 교훈을 남겼다. Switch 포트 논란은 멀티플랫폼 동시 발매 시 "약한 하드웨어에 대한 품질 책임"이라는 업계 화두를 다시 환기시켰다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
| --- | --- |
| 개발사 / 퍼블리셔 | NetherRealm Studios / Warner Bros. Games |
| 디렉터 | Ed Boon |
| 엔진 | Unreal Engine 4 (전작들은 modified UE3) |
| 출시일 | 2023년 9월 19일 (프리미엄 얼리액세스 9월 14일) |
| 플랫폼 | PS5, Xbox Series X\|S, Switch, PC(Steam·Epic) — PS4/Xbox One 미지원 |
| 가격 | $70 (전 플랫폼 공통) |
| 장르 | 2D 평면 3D 격투게임 |
| Metacritic | PS5 86 / OpenCritic 94% 추천 |
| 대표 평점 | Game Informer 9, GamesRadar+ 5/5, IGN 8, GameSpot 8, Push Square 7 |
| 유저 점수 | Metacritic 약 6.5 / Steam Mixed 69~70% |
| 누적 판매 | 출시 직후 ~300만 → 2024.8 400만+ → 2025.1 500만 → 2025.8 620만 → 최근 800만+ |
| 전작 비교 | MK11 1,500만 장 (MK1 미달) |
| 런칭 Kameo 수 | 15명 (10명 즉시, 5명 언락) |
| 핵심 신규 시스템 | Kameo Fighters (메인 1 + 호출형 어시스트 1) |
| 신규 싱글 모드 | Invasions (보드게임형, 시즌제, Johnny Cage 내레이션) |

### 주요 콘텐츠 연표

| 시점 | 사건 |
| --- | --- |
| 2020년경 | 개발 시작 (원래 2022 목표) |
| 2023.06 | Kameo 시스템·로스터 공개 |
| 2023.07 | Kombat Pack 1 발표 (Homelander·Omni-Man·Peacemaker 등) |
| 2023.09.19 | 정식 출시 |
| 2024 | 《Khaos Reigns》 확장팩 + Kombat Pack 2 (Ghostface·T-1000·Conan) |
| 2025.05.14 | Definitive Edition 출시, 추가 캐릭터/스토리 종료 확정 |

### 참고 자료 (영어권 매체 중심)

- Wikipedia, "Mortal Kombat 1" — https://en.wikipedia.org/wiki/Mortal_Kombat_1
- Metacritic, "Mortal Kombat 1" — https://www.metacritic.com/game/mortal-kombat-1/
- OpenCritic, "Mortal Kombat 1" — https://opencritic.com/game/15004/mortal-kombat-1/reviews
- GameSpot 리뷰, "New Era, Familiar Kombat" — https://www.gamespot.com/reviews/mortal-kombat-1-review-new-era-familiar-kombat/1900-6418115/
- GameSpot, "Review Roundup" — https://www.gamespot.com/articles/mortal-kombat-1-review-roundup/1100-6517760/
- Push Square 리뷰 (PS5) — https://www.pushsquare.com/reviews/ps5/mortal-kombat-1
- Xbox Wire, "Kameo Fighters Explained" — https://news.xbox.com/en-us/2023/06/08/mortal-kombat-1-kameo-fighters/
- Den of Geek, "Story Changes Explained" — https://www.denofgeek.com/games/mortal-kombat-1-changes-explained-reboot-alters-timeline/
- Kotaku, "Invasions Mode / Reviews" — https://kotaku.com/mortal-kombat-1-release-mk1-reviews-invasion-mode-ps5-1850843881
- VGChartz, "Sales Top 6.2 Million" — https://www.vgchartz.com/article/465439/mortal-kombat-1-sales-top-62-million-units/
- EventHubs (판매·DLC 다수) — https://www.eventhubs.com/
- Dexerto, "Switch Port nearly unplayable" — https://www.dexerto.com/mortal-kombat/mortal-kombat-1-players-claim-switch-port-is-nearly-unplayable-despite-premium-price-2299091/
- TechRadar, "Switch port slammed as garbage" — https://www.techradar.com/gaming/nintendo-switch/mortal-kombat-1-nintendo-switch-port-slammed-as-garbage-by-gamers
- Dexerto, "All Currencies Explained" — https://www.dexerto.com/mortal-kombat/all-mortal-kombat-1-currencies-explained-2297750/
- Mortal Kombat Wiki (Fandom), 캐릭터·타임라인 — https://mortalkombat.fandom.com/wiki/Mortal_Kombat_1

---

> 《Mortal Kombat 1》은 자기 역사를 다시 쓴 야심작이자, 격투게임이 직면한 구조적 긴장—신선한 메카닉과 화려한 첫인상 vs 콘텐츠 깊이·운영 신뢰·가격 정책—을 가장 선명하게 보여 준 작품이다. 86점의 비평과 6.5의 유저 점수, 800만 장의 판매와 전작 절반에 그친 성과가 한 게임 안에 공존한다. 그 모순이야말로 본작이 게임 기획·운영 레퍼런스로서 가장 흥미로운 지점이다.
