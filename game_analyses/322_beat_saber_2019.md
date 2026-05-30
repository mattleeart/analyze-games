# 《Beat Saber》 (2019) — VR 시대를 연 리듬 액션의 결정판

## 1. 게임 개요

《Beat Saber》는 체코 프라하의 소규모 스튜디오 **Beat Games**(구 Hyperbolic Magnetism)가 개발한 VR 전용 리듬 액션 게임이다. 2018년 5월 1일 Steam 얼리 액세스로 첫선을 보인 뒤, **2019년 5월 21일** PlayStation VR과 PC 정식판이 동시에 출시되었으며, 같은 날 Facebook(현 Meta)의 신형 스탠드얼론 헤드셋 **Oculus Quest** 런칭 라인업의 핵심 타이틀로 데뷔했다. 이 2019년의 "트리플 런칭"은 《Beat Saber》를 VR 산업의 단순한 인기작에서 시대를 정의하는 킬러앱으로 격상시킨 결정적 전환점이었다.

**개발사 / 퍼블리셔**
- 개발 / 퍼블리싱: Beat Games (체코 프라하 소재)
- 2019년 11월 26일 Facebook(Oculus Studios)에 인수. 인수 후에도 프라하 본거지에서 독립 스튜디오로 운영.

**주요 크레딧**
- **Ján Ilavský** — 공동 창립자, 게임 디자이너 / 리드 프로그래머. 이전부터 인디 모바일 게임을 만들던 두 명의 체코 개발자 콤비 중 한 명.
- **Vladimír Hrinčár** — 공동 창립자, 아트 / 디자인. Ilavský와 함께 Hyperbolic Magnetism 시절부터 함께한 동업자.
- **Jaroslav Beck** — 공동 창립자 겸 작곡가 / CEO 역할. Blizzard의 《Overwatch》 단편 영상과 StarCraft, Battlefield 트레일러 음악으로 이름을 알린 체코 출신 작곡가로, 2016년 Epic Music Productions를 세웠고 2018년 Beat Games 공동 창립에 합류해 비즈니스 측면을 이끌었다.

**개발 기간 / 규모**
- 2016년경 Ilavský와 Hrinčár가 "VR에서 라이트세이버 비슷한 무기로 음악에 맞춰 무언가를 잘라보면 어떨까"라는 초기 프로토타입을 시작. 약 2년에 걸친 사이드 프로젝트 형태의 개발 끝에 2018년 5월 얼리 액세스에 도달.
- 얼리 액세스 시점 팀 규모는 **한 자릿수**에 가까운 극소수 인원. Facebook 인수 시점에도 30명 미만으로 알려졌고, 그 이후 빠르게 100명대까지 확장.
- 자체 자금으로 시작된 부트스트랩 인디 프로젝트로, 초기 외부 투자 거의 없음.

**엔진 / 기술 스택**
- **Unity 엔진** 기반.
- 초기에는 SteamVR / Oculus PC SDK / PSVR SDK 대응. 2019년 5월 Oculus Quest 출시와 함께 **Snapdragon 835** 기반의 모바일 GPU에 맞춘 최적화 빌드를 별도 유지. 이후 Quest 2 / Quest 3로 옮겨가며 그래픽 옵션과 라이팅을 단계적으로 강화.
- 핵심 인풋은 양손 6DoF 모션 컨트롤러, 헤드 트래킹(벽 회피용), 그리고 좌우 햅틱.

## 2. 게임 설명

### 컨셉

《Beat Saber》는 "리듬 게임 + 라이트세이버 전투 + 운동"을 VR이라는 매체에서 자연스럽게 융합한 결과물이다. 플레이어는 양손에 한 자루씩 색이 다른 광선검(기본값: 왼손 빨강, 오른손 파랑)을 쥐고, 음악의 비트에 맞춰 정면에서 날아오는 색깔 블록을 **정확한 방향**으로 베어낸다. 동시에 폭탄을 피하고, 머리 위·아래·옆으로 다가오는 벽을 몸을 움직여 회피한다. 게임의 본질은 단순하지만, 그 단순함이 음악과 신체 움직임을 가장 직접적으로 묶어내는 장치가 된다.

이 게임은 서사 중심이 아니다. 전통적 의미의 줄거리도, 캐릭터도, 세계관 백스토리도 거의 없다. 대신 게임은 **순간순간의 카타르시스**와 **자기 신체에 대한 인식**을 핵심 경험으로 삼는다. Road to VR의 초기 프리뷰가 묘사했듯, 이 게임은 "DDR(Dance Dance Revolution)과 라이트세이버 전투의 우리가 미처 원하는 줄 몰랐던 융합"이다.

### 무드 / 톤 / 아트 디렉션

비주얼은 **네온 사이버펑크 + 미니멀**의 결합이다. 칠흑같이 어두운 무대 안에서 광선검의 빨강과 파랑이 명료하게 떠오르고, 블록이 부서질 때 작은 파티클이 튀며, 비트에 맞춰 무대 양옆의 라이트가 점멸한다. UI 역시 극도로 간결하다. 점수, 콤보, 노트 시각 외에는 모든 시각적 노이즈를 제거했다. 이런 미니멀리즘은 두 가지 효과를 낳는다. 첫째, 저사양 모바일 칩셋 위에서도 일정한 프레임을 보장한다(특히 Quest 1의 Snapdragon 835 시절). 둘째, VR 멀미를 유발할 수 있는 시각적 과부하를 제거해 장시간 플레이를 가능케 한다.

### 사운드 / 음악

음악 디렉션은 Beat Games의 공동 창립자이자 작곡가인 **Jaroslav Beck**이 직접 담당했다. 출시 시점의 **Original Soundtrack Vol. 1**은 Beck의 자체 레이블 Epic Music Productions를 통해 발매된 10트랙짜리(약 22분) EP로, EDM·드럼앤베이스·일렉트로니카·복합 비트가 혼합된 자체 제작곡이다. 대표곡 《Beat Saber》, 《Escape》(feat. Summer Haze), 《$100 Bills》, 《Legend》(feat. BackchatBrass) 등은 게임을 처음 접한 사용자들이 가장 많이 듣게 되는 입문 트랙이다.

이후 Beck은 Vol.2, Vol.3, Vol.4, Vol.5(2021)까지 OST 시리즈를 확장하며 Boom Kitty, Camellia, Tokyo Machine, Pegboard Nerds 같은 EDM 씬 인기 아티스트들을 합류시켰다. OST 외에 라이선스 DLC 음악 팩(섹션 3 참고)이 본격적으로 시작된 것도 정식 출시 시점인 2019년 5월의 Imagine Dragons 팩부터다.

## 3. 핵심 시스템 / 메카닉

《Beat Saber》의 디자인은 한 줄로 요약될 만큼 단순해 보이지만, 실제로는 매우 정교하게 조율된 입력 시스템·물리·심리적 보상 루프의 합이다. 이 섹션은 본 분석서에서 가장 비중 있게 다룰 부분이다.

### 코어 게임플레이 루프 (모먼트-투-모먼트)

플레이어는 가상의 무대 위에 서서 정면을 바라본다. 곡이 시작되면 어둠 속에서 빨강·파랑 블록이 일정한 속도로 다가온다. 각 블록에는 **화살표**(상·하·좌·우·대각선 4방향, 총 8방향) 또는 **점**(임의 방향)이 표시되며, 화살표 방향과 **블록 색깔에 일치하는 손**으로 정확하게 베어야 점수가 주어진다.

베어내는 동작은 다음 세 가지 변수에 의해 채점된다.

1. **스윙 시작 각도** (Pre-swing): 블록에 닿기 *전* 광선검이 얼마나 큰 호를 그렸는가. 최대 70도까지 측정해 최대 70점.
2. **스윙 종료 각도** (Post-swing): 블록을 *지난 후* 광선검이 얼마나 큰 호를 그리며 따라갔는가. 최대 30점.
3. **베기 정확도**(Cut accuracy): 블록의 정중앙에서 얼마나 가까운 위치를 베었는가. 최대 15점.

이 셋의 합 115점이 한 블록의 기본 점수이며, 콤보 배수(1x → 2x → 4x → 8x)가 곱해진다. 즉 단순히 "맞춘다"가 아니라 **"몸 전체로 큰 호를 그리며 정중앙을 베어야 만점"** 인 구조다. 이 채점 공식이야말로 《Beat Saber》가 단순한 액션 리듬에서 **신체를 적극적으로 동원하게 만드는 운동**으로 자연스럽게 변모하는 이유다. 점수를 추구할수록 팔은 더 크게 휘둘러지고, 어깨와 코어가 자동으로 동원된다.

블록 외에 두 가지 위험 요소가 있다.

- **폭탄(Bomb)** — 검은 가시 공. 광선검이 닿으면 점수 차감 및 콤보 리셋. 폭탄은 종종 두 개가 가까이 배치되어 광선검의 자세를 강제 회전시키는 트릭 패턴을 만든다.
- **벽(Obstacle / Wall)** — 좌우 또는 정면에서 다가오는 빨간 직사각형 벽. 머리(헤드셋)가 닿으면 점수 감소와 콤보 리셋. 회피하려면 실제로 몸을 옆으로 기울이거나 숙여야 한다.

이후 업데이트에서 추가된 두 가지 신규 노트 타입은 메카닉의 깊이를 더했다.

- **Chain (체인)** — 한 번 베기 시작하면 그 궤적을 따라 작은 조각들이 연속으로 분리되는 노트. 큰 호를 빠르게 그리는 동작을 보상한다.
- **Arc (아크)** — 두 블록을 잇는 곡선. 권장 광선검 경로를 시각화하며, 그 궤적을 따라가면 보너스 점수를 얻는다.

### 진행 구조

게임은 **로비 중심의 메타 구조**다. 메뉴에서 곡을 고르고, 난이도를 정하고, 모드를 선택해 플레이한다. 진행을 강제하는 캠페인 챕터, 오픈월드, 챕터 기반 구조는 없다(예외: PSVR 정식판에 포함된 캠페인 모드 — 후술하듯 평가가 갈렸다).

곡 선택 화면에서 플레이어가 만나는 선택지는 다음과 같다.

- **공식 OST 트랙** (Vol.1~5+)
- **유료 DLC 뮤직 팩** (Imagine Dragons, BTS, Linkin Park, Billie Eilish, Lady Gaga, Skrillex, Green Day, Timbaland, Fall Out Boy, Lizzo, Panic! at the Disco 등)
- **모드 설치 시 커스텀 곡** (PC 한정)

곡당 5단계 난이도(**Easy / Normal / Hard / Expert / Expert+**)가 거의 모든 트랙에 존재하며, 일부 곡은 추가로 **Lawless**(맵 디자이너 자유 패턴)나 360도 회전 전용 패턴을 제공한다.

### 게임 모드

- **Solo / Standard** — 가장 기본. 두 손, 정면 화살표, 점수 추구.
- **Party** — 친구 교대 모드. 점수 입력 및 닉네임 입력.
- **Campaign** — PSVR 정식판부터 도입된 미션형 모드. 특정 점수 조건, 특정 모디파이어 조건(예: "Disappearing Arrows로 90% 정확도 달성") 등을 하나씩 해결해 트로피를 모으는 구조. 후술하듯 평론에서 가장 호불호가 갈렸다.
- **Multiplayer** — 2021년 후속 업데이트로 추가. 최대 5명이 같은 곡을 동시에 플레이하며 점수 경쟁. 출시 시점에는 부재했고, 이는 초기 리뷰의 단골 비판 지점이었다.
- **Practice** — 곡의 특정 구간을 반복 연습. 시작 지점, 속도를 조절 가능.
- **360°/90° 모드** — 무대를 둘러싼 노트가 사방에서 등장. 플레이어가 실제로 몸을 돌리며 플레이.
- **One Saber / No Arrows / Lawless** — 패턴 변형 모드.

플레이어가 선택할 수 있는 모디파이어(채점 가산 / 감산)는 다음과 같다.

- **No Fail** — 죽지 않음(50% 점수 페널티)
- **One Life** — 한 번 실패하면 즉시 종료
- **Faster Song / Slower Song / Super Fast Song**
- **Ghost Notes** — 노트가 마지막 순간에 사라짐
- **Disappearing Arrows** — 화살표 방향만 사라짐
- **Small Notes / Pro Mode / Strict Angles** — 정확도 요구치 강화
- **Battery Energy / Insta Fail** — 실수 허용치 감소

이 모디파이어 체계는 단순한 게임에 길고 깊은 숙련 곡선을 부여한다. 같은 곡, 같은 난이도여도 Disappearing Arrows를 켠 Expert+ 플레이는 사실상 별개의 도전이다.

### 자원 / 진척도 시스템

전통적 의미의 진척도 시스템은 거의 없다. 레벨업도, 장비도, 통화도 없다. 진척도는 **점수와 등급(S, A, B, C, D, E)**, 그리고 **퍼펙트 콤보**(FC, Full Combo) 달성 여부만으로 표현된다. 게임은 의도적으로 **장식을 모두 배제하고 음악과 신체에만 집중**시키는 디자인 철학을 고수했다. 후속 업데이트에서 아바타(머리 위 모자, 광선검 스킨)가 추가되었지만 게임 플레이의 본체에는 거의 영향이 없다.

### 멀티 / 라이브 운영 / MTX

- **멀티** — 2021년 무료 업데이트로 추가. 최대 5인 동시 플레이.
- **라이브 운영** — 시즌 패스나 배틀패스 형태의 라이브 서비스는 없다. 대신 **유료 뮤직 팩**이 비정기적으로 출시되는 단순한 모델.
- **DLC 가격** — 곡당 약 $1.99, 팩(보통 8~12곡) $12.99 전후. 이 균일하고 직관적인 가격 정책이 누적 4,000만 곡 판매(2021년 2월 기준)로 이어진 핵심 매출원이 되었다.

### 라이선스 뮤직 팩 라인업 (2019~2024 주요)

- **Imagine Dragons Music Pack** (2019-05): 정식 출시와 동시에 공개된 첫 빅네임 라이선스. 《Believer》, 《Thunder》, 《Radioactive》 등 12트랙.
- **Monstercat Music Pack** (2019-08): EDM 레이블 패키지.
- **Panic! at the Disco Music Pack** (2019-09)
- **Rocket League x Monstercat Music Pack** (2020-04)
- **Green Day Music Pack** (2020-09)
- **Timbaland Music Pack** (2020-12)
- **BTS Music Pack** (2021-04): 12트랙. K-팝 팬덤이 VR로 대규모 유입된 분기점.
- **Linkin Park Music Pack** (2021): 8트랙.
- **Skrillex Music Pack** (2021)
- **Billie Eilish Music Pack** (2021-08): 《Bad Guy》, 《Therefore I Am》, 《NDA》 등 10트랙, $12.99. *Variety*가 별도 기사로 다뤄 일반 음악 매체의 주목까지 이끌어낸 사례.
- **Lady Gaga, Fall Out Boy, Lizzo, The Rolling Stones, Daft Punk** 등 (2022~2024)

이 라이선스 협상은 Facebook 인수 이후 가속화됐다. Beat Games 단독으로는 메이저 레이블(Universal, Sony Music, Warner)과 동등 협상력으로 마주하기 어려웠지만, 모기업의 인수 이후 Interscope를 비롯한 메이저 레이블과 장기 계약이 차례로 체결되었다.

### 난이도 / 접근성 옵션

- **5단계 난이도** + **No Fail** / **Slower Song** 모디파이어로 진입 장벽을 사실상 0에 가깝게 낮춤.
- **한 손 모드(One Saber)** — 한 손만 사용. 일부 신체 조건의 플레이어에게 중요한 옵션.
- **앉아서 플레이** 옵션 (벽 회피 조정).
- **컬러 커스터마이즈** — 색약 대응. 좌우 광선검 색을 자유롭게 변경 가능.
- **광선검 길이, 트레일 효과 조정**
- **자동 회전(360 모드 보조)**, **격투기 모드용 크기 조정** 등.

VR 게임 중에서도 접근성 옵션의 폭은 상당히 넓은 편이며, 특히 한 손 모드는 장애인 게이머 커뮤니티에서 자주 호평된다.

### UI / UX 디자인 철학

UI는 "**보이는 것이 적을수록 좋다**"는 원칙으로 구성됐다. 게임 중에는 점수, 콤보 배수, 에너지 바, 곡 진행 바 외에 어떤 시각 요소도 없다. 메뉴는 곡 → 난이도 → 모디파이어 → 시작 순서로 3~4번의 클릭만으로 곡에 진입할 수 있다. 이는 **"VR 안에서는 메뉴 시간이 짧을수록 멀미와 피로가 줄어든다"**는 경험칙을 충실히 반영한 결과로, 후속 VR 리듬 게임 대다수가 이 인터페이스 패턴을 모방했다.

## 4. 평가

### 평론 점수

**Metacritic**
- PC: 약 87 (호평 일색)
- PlayStation 4 / PSVR: 81
- 유저 스코어는 모든 플랫폼에서 8점대 후반.

**OpenCritic**: 86 / 100, 비평가 91% 추천. 34개 매체 평균.

**주요 매체 점수**
- **IGN — 9.5 / 10** — "Beat Saber은 VR에서 가능한 가장 만족스러운 리듬 게임 중 하나다. 휘두를 때마다 작동하는 단순한 메카닉이 시간이 지나도 매혹적으로 남는다."
- **GameSpot — 8 / 10** — 핵심 게임플레이를 극찬하면서도 곡 수의 한정성과 캠페인 모드의 약점을 지적.
- **Eurogamer** — Essential 등급 권고. "VR이 무엇을 할 수 있는지의 가장 깔끔한 증명."
- **PC Gamer** — 정식판 리뷰에서 "VR이 단순한 신기함을 넘어 진짜 게임으로 향하는 다리"라고 표현.
- **Polygon** — 출시 직후의 "VR을 위한 첫 번째 진짜 킬러앱" 평가.

### 주요 수상

- **The Game Awards 2019 — Best VR/AR Game** 수상
- **DICE Awards 2019 — Immersive Reality Game of the Year** 수상 (D.I.C.E. Summit)
- **Steam Awards 2019 — VR Game of the Year** (유저 투표 부문)
- **BAFTA Games Awards 2019 — Best Debut Game** 노미네이트
- **Game Developers Choice Awards 2019 — Best VR/AR Game** 노미네이트
- Develop:Star Awards, Webby Awards, 다수의 매체 GOTY 후보.

VR 카테고리에서 사실상 그해를 휩쓴 수상 실적으로, "VR 게임의 표준 후보 = Beat Saber"라는 인상을 산업 차원에서 굳혔다.

### 상업 지표 (시간 순)

판매·매출 데이터는 Beat Games / Oculus / Road to VR의 공식 발표 및 추정치를 기준으로 한다.

| 시점 | 누적 판매 | 누적 DLC 곡 | 추정 매출 |
|------|-----------|------------|-----------|
| 2018-05 (얼리 액세스) | 출시 한 달 만에 10만+ | — | — |
| 2019-03 | **100만 장** (출시 9개월) | — | — |
| 2020-03 | **200만 장** | 1,000만+ | **약 $67M** (Road to VR 추정) |
| 2021-02 | **400만 장** | **4,000만+** | **약 $180M** (Road to VR 추정) |
| 2022 | Quest 단독 매출 1억 달러 돌파 (UploadVR) | — | — |
| 2023~ | 누적 매출 **2억 5,500만 달러+** 추정 (UploadVR) | — | — |

특히 주목할 것은 매출의 **가속도**다. 200만 장 → 400만 장은 약 11개월 만이며, 그 사이 DLC 매출이 본격적으로 비중을 키웠다. Quest 2가 2020년 10월 출시되면서 사용자 기반이 폭발적으로 늘었고, Beat Saber는 Quest 2를 산 사람의 **첫 게임**, 혹은 **유일한 게임**으로 자리 잡았다.

### 유저 평가

- **Steam**: 정식판 리뷰 9만+ 건 중 "압도적으로 긍정적" (97% 안팎). VR 게임 중 최고 수준.
- **Reddit r/beatsaber**: 활성 구독자 20만+ 명, 일일 수십 건의 클립이 업로드되는 매우 능동적인 커뮤니티. 모딩, 맵 추천, FC 자랑이 주류.
- **YouTube**: "Expert+ Full Combo" 클립, "BSWC(Beat Saber World Championship)" 토너먼트 영상, 트릭샷 영상이 누적 수십억 뷰 단위의 거대한 생태계를 형성.

### 평론-유저 괴리

평론과 유저 평가가 거의 동일하게 호평 일색이라는 점이 오히려 특이하다. 일반적으로 유저는 평론보다 더 가혹한데, 이 게임은 양쪽 모두에서 90점대를 받는다. 단 한 가지 미묘한 차이는, **하드코어 유저층**일수록 "공식 콘텐츠는 부족하지만 커스텀이 있으니 만점"이라는 식의 평가를 한다는 점이다. 즉 **유저 평가의 절반은 모딩 커뮤니티가 만들어준 것**이라 해도 과언이 아니다.

## 5. 성공 요인 분석

《Beat Saber》의 성공은 우연이 아니며, 다음 여섯 가지 요인의 정밀한 정렬에서 비롯됐다.

### 5-1. "VR을 위한 첫 번째 진짜 게임"이라는 포지셔닝

2016~2018년 VR 시장은 "기술 시연(tech demo) 천국, 진짜 게임 사막"이었다. Vive와 Rift 초기에는 《Job Simulator》, 《Superhot VR》 등 인디 히트작은 있었지만, **반복 플레이 시간을 보장하는 코어 루프**를 가진 게임은 드물었다. Beat Saber는 출시 첫 주부터 "VR을 처음 사면 보여주는 게임"으로 자리매김했고, 이 단순한 사실은 어떤 마케팅 캠페인보다 강력했다. 헤드셋을 손님 머리에 씌우면 30초 안에 환호성이 나오는 게임은 그 자체로 영업 사원이다.

### 5-2. 단순함의 천재성 — "30초 안에 이해, 1,000시간 안에 마스터"

게임플레이는 그래픽 스타일과 인터페이스 모두 신규 사용자가 시연 30초 만에 이해 가능하게 디자인됐다. 동시에 Expert+ 난이도, Disappearing Arrows, Ghost Notes 같은 모디파이어, 그리고 커뮤니티 매핑 트렌드(예: 익스트림 BPM 350+ 패턴)는 천 시간 단위의 숙련 곡선을 제공한다. **진입은 0, 천장은 무한**이라는 이 비대칭이 게임의 수명을 결정적으로 늘렸다.

### 5-3. Oculus Quest 런칭 동시 출시 — 플랫폼-게임 공진화

2019년 5월 21일 Oculus Quest 출시는 VR 역사상 가장 중요한 분기점이다. PC와 케이블을 더 이상 필요로 하지 않는 첫 메이저 스탠드얼론 헤드셋이었고, 그 런칭 라인업의 얼굴이 바로 Beat Saber였다. Quest는 Beat Saber를 팔았고, Beat Saber는 Quest를 팔았다. 무선이 된 게임은 360도 회전이 자유로워졌고, 거실의 한가운데에서 가족이 돌아가며 플레이하는 **"리빙룸 VR"**의 표준 시나리오를 만들어냈다. VentureBeat의 당시 보도는 "Beat Saber가 Quest의 와이어리스 VR을 의미 있게 만들어준 게임"이라고 평했다.

### 5-4. Facebook 인수와 라이선스 메가딜

2019년 11월 Facebook의 Beat Games 인수는 게임의 두 번째 도약 엔진이었다. Beat Games 단독으로는 거의 불가능했던 메이저 레이블 라이선스 협상이 모기업의 자원과 함께 가능해졌다. **Imagine Dragons → BTS → Linkin Park → Billie Eilish → Lady Gaga**로 이어지는 라인업은 단순한 음악 팩이 아니라 **타깃 인구 통계의 확장**을 의미했다. BTS 팩은 K-팝 팬덤을, Billie Eilish 팩은 10대 후반 여성을, Lady Gaga 팩은 LGBTQ+ 커뮤니티를 새로 유입시켰다. 이 다양화가 곧 매출 곡선의 가속을 설명한다.

### 5-5. 모딩 커뮤니티 — 무료의 "DLC 군대"

PC 버전에서는 BSMG(Beat Saber Modding Group)가 결성되어 **BeatSaver**(맵 저장소)와 **BeastSaber**(메타데이터·랭킹·리뷰), **ModAssistant / BSManager**(설치 도구)라는 견고한 생태계를 구축했다. 5,000명 이상의 등록 매퍼가 월 약 **2,500곡**을 새로 추가하며, 누적 5만+ 커스텀 곡이 존재한다. 활성 유저의 약 65%가 커스텀 곡을 즐긴다는 추정치는 이 게임 수명의 절반을 커뮤니티가 책임지고 있다는 의미다. Beat Games는 모딩을 공식 지원하지는 않았지만, 사실상 묵인하며 이 생태계를 자산화했다. 모딩의 존재는 PC 버전을 "끝없는 콘텐츠 머신"으로 만들었고, Quest 버전(모딩이 더 까다로움)은 공식 라이선스 곡을 사주는 사용자 풀로 분화시켰다. 이 이중 구조가 영리하게 작동했다.

### 5-6. 운동 — "재미있는 운동"이라는 카테고리의 발명

코로나19 락다운(2020) 시기 헬스장이 닫히면서 Beat Saber는 예상치 못한 "홈 카디오" 카테고리의 대표 주자가 됐다. **Virtual Reality Institute of Health and Exercise**의 측정에 따르면 Beat Saber는 **싱글 테니스와 유사한 칼로리 소비**(시간당 약 200~400 kcal, 체중 240파운드 기준 45분 세션에서 680~900 kcal)를 보였다. 이는 단순한 게임이 아니라 **유산소 운동 기구**로 게임이 재포지셔닝되는 계기였다. 2024년 JMIR Serious Games 저널의 후속 연구(87명, 20분 표준화 세션) 역시 이를 학술적으로 확인했다.

이 "운동" 포지셔닝은 두 가지 부작용을 낳았다. 첫째, "다이어트용으로 산다"는 새로운 구매 동기 군. 둘째, **VR fitness** 자체가 하나의 게임 카테고리로 부상해 《Supernatural》, 《FitXR》 같은 후속작의 시장을 열었다.

### 동시기 작품 대비 차별점

같은 시기 VR 시장의 경쟁자들과 비교하면 차별점이 더 선명해진다.

- **《Job Simulator》(2016) / 《Vacation Simulator》(2019)** — 코미디 시뮬레이션. 재미는 강력하지만 반복 플레이 동기가 약함.
- **《Superhot VR》(2016)** — 액션 퍼즐. 명작이지만 짧은 캠페인(3~4시간) 후 반복성이 한정적.
- **《Audica》(2019, Harmonix)** — VR 리듬 슈팅. 정통 리듬게임 명가의 작품이지만 동작이 정적(총 조준).
- **《Pistol Whip》(2019, Cloudhead)** — 리듬 + 슈팅 + 액션 영화. 강력한 컨셉이지만 후발주자.

이들과 비교한 Beat Saber의 차별점은 **신체 전체를 휘두르는 큰 호의 동작**이 곧 점수와 직결된다는 점, 그리고 **음악과 시각의 카타르시스가 동기화**되는 첫 30초의 압도성이다.

## 6. 비평적 시각 / 한계 / 논란

만점에 가까운 평가 속에서도, 시간이 흐르며 누적된 비판은 분명히 존재한다.

### 6-1. 공식 곡 수의 빈약함

출시 시점 공식 곡은 단 **10곡**(OST Vol.1)이었다. 이 한계는 거의 모든 평론에서 공통적으로 지적됐다. 《GameSpot》은 "스타일적 다양성이 부족하고, 공식 곡 컬렉션의 한정성이 게임이 도달할 수 있었던 만큼 좋아지지 못하게 한다"고 명시했다. 메인 OST 대부분이 EDM/일렉트로니카 한 계열이라는 점도 음악적 다양성을 떨어뜨렸다. 이 한계는 부분적으로 DLC 팩으로, 부분적으로는 모딩으로 메워졌지만, 추가 비용 없이 즐길 수 있는 베이스 게임의 콘텐츠가 부족하다는 인상은 끝내 완전히 해소되지 못했다.

### 6-2. 캠페인 모드의 미적지근한 평가

PSVR 정식판과 함께 추가된 캠페인 모드는 "트로피를 모으는 미션 형식"이었지만, 대부분의 평론가는 이를 "성공적이지 못한 추가"로 평가했다. 동일한 곡을 다른 모디파이어 조합으로 다시 플레이하는 구조는 새로운 콘텐츠라기보다 도전과제 시스템의 확장에 가까웠고, 사실상 게임의 핵심 매력에 기여하지 못했다.

### 6-3. 멀티플레이어 부재의 장기화

출시 시점에 온라인 멀티플레이어가 없었던 점은 가장 자주 거론된 미비점이다. 마침내 멀티가 추가된 것은 **2021년**이었고, 그것도 5인 동시 점수 경쟁 형태에 머물렀다. 본격적인 1대1 대전, 협동 모드, 리그 시스템 같은 e스포츠 인프라는 여전히 공식적으로는 미흡하다는 평이 많다(BSWC 같은 비공식 토너먼트가 그 빈자리를 채웠다).

### 6-4. 커스텀 곡 접근성 — "당신은 하드코어가 되거나, 떨어지거나"

PC 모딩 씬은 강력하지만, 진입 장벽이 일반 사용자에게는 만만치 않다. ModAssistant 설치, 게임 버전 다운그레이드, 모드 충돌 관리 등은 비기술적 사용자에게 분명한 장벽이다. Quest 버전의 사이드로딩 모딩은 한층 더 까다롭다. 이 결과 "공식 콘텐츠는 부족한데 커뮤니티 콘텐츠는 진입이 어려운" 중간층 사용자가 생긴다. 일부 리뷰는 모딩 커뮤니티의 "당신이 충분히 노력하지 않은 거다"는 문화에 대해 부정적으로 언급한다.

### 6-5. Facebook / Meta 인수 이후의 운영 논란

2019년 11월 인수 이후, 몇 가지 작은 불만이 누적됐다.

- **Quest 전용 계정 정책** — Meta 계정 강제, PSVR과의 크로스 진척도 부재.
- **DLC 가격 정책** — 다른 라이선스 음악 게임 대비 곡당 단가가 다소 높다는 지적.
- **모딩에 대한 미묘한 적대** — Quest 버전 업데이트 시 모드 호환성을 깨는 변경이 잦았던 점. 모딩 커뮤니티는 "공식 무시 + 잦은 호환성 파괴"의 패턴이 의도된 것이냐를 두고 추측을 이어갔다.
- **저작권/모딩 갈등** — Jaroslav Beck은 2021년 Beat Games에서 떠난 후, 본인이 공동 창립자였음에도 모기업 정책의 변화를 두고 모호한 입장을 보였고, 이는 커뮤니티 정서에 작은 균열을 남겼다.

### 6-6. 안전 / 부상 이슈

운동 강도가 강한 게임이라는 점이 부상으로 이어지는 사례도 보고됐다. 어깨 회전근개 통증, 손목 부상, 가구 충돌 등 가벼운 부상부터 헤드셋이 벽이나 천장 등에 부딪혀 파손되는 사례까지. Reddit r/beatsaber에서 "Quest broken from Beat Saber" 클립은 농담거리가 된 지 오래다.

## 7. 영향과 유산

### 7-1. 장르의 정의 — "VR 리듬 액션"이라는 카테고리 창설

Beat Saber 이전에는 "VR 리듬 게임"이라는 카테고리가 사실상 존재하지 않았다. 이후 등장한 작품 거의 전부가 Beat Saber의 그림자 안에서 정의된다.

- **《Synth Riders》(Kluge Interactive, 2018~)** — "신스웨이브 미학 + 두 손으로 비트 따라가기". 곡 흐름을 화살표 대신 부드러운 궤적으로 풀어낸 변주.
- **《Audica》(Harmonix, 2019)** — Rock Band 명가의 답안. 손잡이가 라이트세이버가 아니라 권총이라는 점에서 차이.
- **《Pistol Whip》(Cloudhead, 2019)** — 액션 영화 리듬 슈팅. Beat Saber의 핵심을 슈팅과 통합.
- **《Ragnarock》(2021)** — 바이킹 드럼 리듬. "북을 친다"는 동작 자체를 음악으로 묶음.
- **《Smash Drums》, 《Beat Sage》(AI 자동 매핑 툴)** 등 파생 생태계.

이들 모두는 Beat Saber가 정의한 "**팔의 큰 호 + 정확한 타이밍 = 카타르시스**"라는 기본 등식을 변주한다.

### 7-2. VR fitness 카테고리의 산업화

《Supernatural》(2020), 《FitXR》, 《Les Mills Bodycombat》(2022) 등 본격적 VR 피트니스 앱은 Beat Saber가 "재미있는 운동"이라는 시장을 검증해준 덕분에 가능했다. Meta는 이 카테고리를 **Quest의 핵심 마케팅 축**으로 격상시켜 "운동으로서의 VR"이라는 새로운 구매 동기를 만들었다.

### 7-3. e스포츠와 커뮤니티 토너먼트

**BSWC (Beat Saber World Championship)** 같은 커뮤니티 주도 토너먼트가 매년 개최되며, 상위권 플레이어들의 Expert+ 퍼펙트 콤보 클립은 트위치·유튜브에서 수백만 뷰 단위의 콘텐츠가 된다. 공식 e스포츠 인프라 없이도, 시청 콘텐츠로서의 정체성을 확립한 드문 사례다.

### 7-4. 산업적 의미 — VR 소프트웨어의 수익성 증명

VR 산업에서 가장 자주 던져진 질문은 "이 시장에서 게임을 만들어서 진짜 돈이 되는가"였다. Beat Saber의 누적 매출 2억 5,500만 달러+, 그중 Quest 단독 1억 달러+는 그 질문에 대한 가장 강력한 긍정 답안이다. 이 데이터 한 줄이 후속 VR 게임 개발사의 투자 유치 슬라이드에서 거의 빠짐없이 인용된다. Population: One, Onward, Resident Evil 4 VR 같은 후속 VR 히트작들이 다른 양상이긴 해도 시장 자체의 검증된 규모를 전제로 가능했다.

### 7-5. 문화적 의미 — VR의 이미지를 바꾼 게임

대중 매체에서 "VR"이라는 단어가 등장하면 떠올리는 이미지가 바뀌었다. **Ready Player One** 식의 거대한 가상세계가 아니라, **거실에서 양손에 광선검을 들고 빨강·파랑 블록을 베는 사람**이 VR의 새로운 아이콘이 됐다. 광고, 영화, 시트콤, 라스베이거스 VR 어케이드의 사인 — 모두에서 Beat Saber가 시각적 메타포 역할을 한다. 이는 단순한 인기를 넘어 한 매체의 대중적 표상을 결정했다는 점에서 거의 게임 단독으로 달성한 흔치 않은 성취다.

### 7-6. 후속작? — "후속작 없음"이라는 전략

흥미롭게도 Beat Games는 2026년 현재까지 **공식 후속작을 내지 않았다**. 대신 OST Vol.5, 새로운 라이선스 팩, 멀티플레이어, 새로운 노트 타입(Chain, Arc) 같은 형태로 **본편을 라이브 운영**하는 전략을 택했다. 이는 라이선스 자산(이미 출시된 모든 음악 팩)을 한 게임 안에서 누적시키는 비즈니스 모델 결정인 동시에, "코어 디자인이 완성되어 있으므로 후속작이 필요하지 않다"는 자신감의 표현이기도 하다.

## 8. 부록

### 핵심 통계 표

| 항목 | 값 | 출처 / 시점 |
|------|------|------------|
| 첫 출시 (얼리 액세스) | 2018-05-01 (PC, Steam) | Beat Games / Steam |
| 정식 출시 | 2019-05-21 (PC / PSVR / Oculus Quest) | Beat Games |
| Facebook 인수 | 2019-11-26 | GameDeveloper.com |
| 100만 장 달성 | 2019-03 (출시 9개월) | Beat Games 공식 |
| 200만 장 달성 | 2020-03 | Road to VR |
| 400만 장 달성 | 2021-02 | Road to VR, PC Gamer |
| 누적 DLC 곡 판매 | 4,000만+ (2021-02) | Road to VR |
| 추정 매출 (2021-02) | 약 $180M | Road to VR |
| Quest 단독 매출 1억 달러 | 2022 | UploadVR |
| 누적 매출 추정 | $255M+ (2023) | UploadVR |
| Metacritic (PC) | 약 87 | Metacritic |
| OpenCritic | 86 / 100, 91% 추천 | OpenCritic |
| IGN | 9.5 / 10 | IGN |
| GameSpot | 8 / 10 | GameSpot |
| 칼로리 소비 | 약 200~400 kcal/시간 (테니스 단식 수준) | VR Health Institute |
| 커스텀 곡 누적 | 5만+ | BSMG / BeatSaver |
| 월간 신규 커스텀 곡 | 약 2,500곡 | BeatSaver |
| 등록 매퍼 수 | 5,000명+ | BeatSaver |
| 주요 수상 (2019) | TGA Best VR, DICE Immersive Reality GOTY, Steam Awards VR GOTY | 각 시상식 공식 |

### 주요 라이선스 뮤직 팩 목록 (출시 순)

| 출시 | 팩 |
|------|-----|
| 2019-05 | Imagine Dragons Music Pack |
| 2019-08 | Monstercat Music Pack |
| 2019-09 | Panic! at the Disco Music Pack |
| 2020-04 | Rocket League x Monstercat Music Pack |
| 2020-09 | Green Day Music Pack |
| 2020-12 | Timbaland Music Pack |
| 2021-04 | BTS Music Pack |
| 2021 | Linkin Park / Mike Shinoda Music Pack |
| 2021 | Skrillex Music Pack |
| 2021-08 | Billie Eilish Music Pack |
| 2022~ | Lady Gaga, Fall Out Boy, Lizzo, The Rolling Stones, Daft Punk 등 |

### 주요 인터뷰 / 매체 자료

- **Road to VR — Ben Lang의 시리즈 기사들** (판매 마일스톤, 매출 추정, 칼로리 측정 기사 다수). "Beat Saber Has Sold 4M Copies & 40M Songs", "Playing Beat Saber Could Burn the Same Number of Calories as Tennis" 등.
- **UploadVR** — "Beat Saber Passes $100 Million In Revenue On Quest Platform Alone", "Beat Saber Reportedly Reached $255 Million Revenue".
- **PC Gamer** — "Beat Saber slashes VR sales records after shipping 4 million copies", "Beat Saber is a VR rhythm game that's basically Lightsaber Hero".
- **Variety** — Billie Eilish Music Pack 발매 기사 (2021-08).
- **VentureBeat** — Beat Saber Quest 데뷔 기사.
- **GameDeveloper.com (구 Gamasutra)** — Facebook의 Beat Games 인수 발표 기사 (2019-11).
- **Mixed-news.com** — "Beat Saber: How it began and how it's going" (개발사 역사 종합).
- **Shacknews** — Beat Saber Oculus Quest 런칭 라인업 기사.

### 커뮤니티 / 모딩 자료

- **BSMG (Beat Saber Modding Group) Wiki** — https://bsmg.wiki
- **BeatSaver** — 커스텀 맵 마스터 저장소.
- **BeastSaber (bsaber.com)** — 큐레이션, Map of the Week, Beasties Awards.
- **r/beatsaber** — Reddit 커뮤니티(20만+ 구독자).

### 참고 자료 목록 (영어권 매체 중심)

1. Wikipedia — "Beat Saber" (게임 일반 정보, 출시 일자, 판매 데이터의 1차 집계).
2. Wikipedia — "The Game Awards 2019" (수상 데이터).
3. Metacritic — Beat Saber PC / PS4 critic & user reviews.
4. OpenCritic — Beat Saber 평론 집계.
5. IGN — Beat Saber 9.5/10 리뷰.
6. GameSpot — Beat Saber 8/10 리뷰.
7. Road to VR — "Beat Saber Has Sold 4M Copies & 40M Songs, an Estimated $180M Revenue".
8. Road to VR — "Beat Saber Sold 2M Copies & 10M Songs for an Estimated $67M Revenue".
9. Road to VR — "Playing Beat Saber Could Burn the Same Number of Calories as Tennis".
10. Road to VR — "Beat Saber is a VR Fusion of DDR and Lightsaber Combat That We Never Knew We Wanted".
11. UploadVR — "Beat Saber Passes $100 Million In Revenue On Quest Platform Alone".
12. UploadVR — "Beat Saber Reportedly Reached $255 Million Revenue".
13. UploadVR — "Beat Saber Wins 2019 VR Game Of The Year At The Game Awards".
14. PC Gamer — "Beat Saber slashes VR sales records after shipping 4 million copies".
15. PC Gamer — "Beat Saber is a VR rhythm game that's basically Lightsaber Hero".
16. Variety — "Billie Eilish Beat Saber Music Pack Launches on Oculus Quest 2, Rift Platforms" (2021).
17. VentureBeat — "Beat Saber will debut on the Oculus Quest wireless VR headset".
18. GameDeveloper.com — "Beat Saber dev Beat Games acquired by Facebook" (2019-11).
19. Music Ally — "Facebook buys the developer of VR-music game Beat Saber".
20. Mixed-news.com — "Beat Saber: How it began and how it's going".
21. Shacknews — "Beat Saber joins Oculus Quest launch game lineup".
22. Virtual Reality Institute of Health and Exercise — Beat Saber 평가 보고서.
23. JMIR Serious Games (2024) — Beat Saber 에너지 소비 측정 연구 (87명, 20분 표준화 세션).
24. BSMG Wiki — 모딩 가이드, FAQ.
25. BeastSaber (bsaber.com) — 커뮤니티 큐레이션 사이트.

---

*분석서 작성: 2026년 5월. 자료 기준은 최대한 영어권 1차 자료를 우선하며, 판매·매출은 모두 공식 발표 혹은 신뢰 가능한 추정치(Road to VR, UploadVR 등)에 근거함. 본문 내 매출 추정 수치는 출처 시점 추정이며 실제 결산 수치와 차이가 있을 수 있다.*
