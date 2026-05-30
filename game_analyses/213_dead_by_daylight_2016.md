# Dead by Daylight (2016) 심층 분석

> 한 명의 살인마와 네 명의 생존자가 안개 낀 시험장에서 마주하는 비대칭 멀티플레이어 호러. 출시 당시 "콘텐츠가 부족한 실험작"이라는 미지근한 평가를 받았지만, 거의 10년에 걸친 집요한 라이브 운영과 호러 영화 IP 총집합 전략으로 누적 6,000만 명 이상이 플레이한 장르의 표준이 된 게임. 이 문서는 영어권 매체·개발자 인터뷰·상업 데이터를 토대로 Dead by Daylight가 무엇이고, 왜 성공했으며, 어떤 한계를 안고 어떤 유산을 남겼는지 정밀하게 분석한다.

---

## 1. 게임 개요

### 기본 정보
- **개발/퍼블리셔**: Behaviour Interactive (캐나다 몬트리올). 캐나다 최대 규모의 독립 게임 스튜디오로, 원래는 수탁(work-for-hire) 개발이 주력이던 회사였다. Dead by Daylight는 이 회사가 처음으로 크게 성공시킨 자체 IP다.
- **초기 퍼블리셔**: Starbreeze Studios. 《PAYDAY》 시리즈로 알려진 스웨덴 퍼블리셔로, 2015년 자사의 두 번째 퍼블리싱 딜로 Behaviour의 신작에 USD 2,000,000을 투자했다.
- **장르**: 비대칭(asymmetric) 4 대 1 멀티플레이어 서바이벌 호러
- **엔진**: Unreal Engine 4 (2016~2024). 2024년 4월 Unreal Engine 5로 대규모 업그레이드.
- **첫 공개**: 2016년 3월 2일 첫 트레일러 → 5월 29일 클로즈드 베타 → **2016년 6월 14일 PC(Steam) 정식 출시**

### 주요 크레딧
- **Creative Directors**: Ashley Pannell, Dave Richard, Mathieu Coté, Matthew Spriggens
- **게임 디렉터/리드 디자이너**: Mathieu Coté — 출시 초기부터 수년간 이 게임의 얼굴 역할을 맡으며 수많은 인터뷰와 커뮤니티 소통을 담당했다.
- **프로듀서**: Stéfan Beauchamp-Daniel
- **프로그래밍**: Fadi Beyrouti(테크니컬 디렉터), Jean-Philip Desjardins, Rémi Veilleux
- **라이터**: Farah Daoud-Brixi
- **작곡**: Michel F. April

### 개발 규모와 배경
Dead by Daylight는 거대 예산 프로젝트가 아니었다. Starbreeze의 초기 투자가 USD 2M 수준이었다는 점에서, 이 게임은 비교적 작은 팀이 비교적 낮은 예산으로 시작한 "아이디어 승부형" 프로젝트였다. Behaviour는 수탁 개발로 쌓은 Unreal Engine 기술력을 자체 IP에 투입했고, Unreal Engine 4를 선택한 핵심 이유 중 하나가 검증된 네트워킹·멀티플레이어 지원이었다. 비대칭 멀티플레이어라는 까다로운 동기화 문제를 다뤄야 하는 게임에서 이는 합리적 선택이었다.

### 출시 플랫폼 연표
| 플랫폼 | 출시일 |
|---|---|
| Windows (Steam) | 2016년 6월 14일 |
| PlayStation 4 / Xbox One | 2017년 6월 20~23일 |
| Nintendo Switch | 2019년 9월 24일 |
| Mobile (iOS/Android) | 2020년 4월 17일 (2025년 3월 20일 서비스 종료) |
| Google Stadia | 2020년 10월 1일 (2023년 1월 18일 종료) |
| Xbox Series X/S | 2020년 11월 10일 |
| PlayStation 5 | 2020년 11월 |
| Nintendo Switch 2 | 2025년 |

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 컨셉
Dead by Daylight의 한 판(Trial, 시험)은 단순하다. 네 명의 **생존자(Survivor)**가 어두운 맵에 떨어지고, 한 명의 **살인마(Killer)**가 그들을 사냥한다. 생존자는 발전기를 고쳐 탈출하려 하고, 살인마는 그들을 붙잡아 갈고리에 매달아 정체 모를 존재에게 제물로 바치려 한다. 이 단순한 비대칭 구도가 이 게임의 전부이자 핵심이다.

게임 디렉터 Mathieu Coté는 인터뷰에서 개발 의도를 "무한한 순간 생성기(an infinite moment generator)"라고 표현했다. 계속 플레이하고 또 플레이해도 재미있고, 매번 자신이 정확히 무엇을 상대하는지 확신하지 못하는 게임 — 그것이 목표였다. 정해진 스토리를 클리어하는 게임이 아니라, 매 판마다 추격과 도주의 긴장이 새롭게 빚어지는 게임을 만들고자 했다.

### 세계관 — The Entity와 The Fog
게임의 모든 캐릭터는 **The Entity(개체)**라 불리는 거미 같은 형상의 우주적 공포 존재에게 붙잡혀 끝없는 시험에 갇혀 있다. The Fog(안개)는 이 존재가 지배하는 영역이며, 살인마가 생존자를 갈고리에 걸면 The Entity가 위에서 촉수를 뻗어 제물을 거둬간다. 죽어도 죽음은 끝이 아니다 — 캐릭터는 다시 캠프파이어 옆에서 깨어나 또다시 시험에 던져진다. 이 순환적·무한 루프적 세계관은 "왜 같은 캐릭터로 무한히 매칭이 반복되는가"라는 멀티플레이어 게임의 구조적 특성을 서사적으로 합리화하는 영리한 장치다.

Coté에 따르면 개발 초기부터 Stephen King, 특히 《The Dark Tower》 연작이 팀의 머릿속에 있었다. 서로 다른 세계와 아이디어를 과도하게 설명하지 않으면서 하나로 엮는 방식에 매료됐다는 것이다. 그는 "코즈믹 호러를 다룰 때 초반의 모호함은 약점이 아니라 강점"이라고 말했는데, 이 철학은 훗날 Halloween의 Michael Myers, 《A Nightmare on Elm Street》의 Freddy Krueger 같은 서로 무관한 IP들을 한 세계에 끌어모으는 데 결정적 토대가 됐다. The Entity는 모든 호러를 빨아들일 수 있는 "만능 빨대"였다.

### 무드와 아트 디렉션
톤은 끈적하고 불안한 슬래셔 호러다. 안개에 잠긴 농장, 정신병원, 공장, 자동차 정비소 같은 맵은 어둡고 좁은 시야와 음향으로 공포를 빚는다. 핵심 음향 장치는 **심장박동음(heartbeat)** — 살인마가 가까워질수록 점점 거세지는 이 소리가 생존자의 긴장을 끌어올린다. 작곡가 Michel F. April의 사운드는 멜로디보다는 분위기·긴장·타격감 중심으로, 추격이 시작될 때의 음악적 고조가 "들켰다"는 공포를 즉각적으로 전달한다.

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

### 코어 게임플레이 루프
Dead by Daylight의 한 판은 양측에서 전혀 다른 경험으로 진행된다.

**생존자 입장**: 4명이 흩어져 맵을 탐색하며 7개의 발전기 중 **5개를 수리**한다. 발전기 앞에서 상호작용 버튼을 누르면 수리가 진행되는데, 이 도중 무작위로 **스킬체크(Skill Check)**가 발생한다. 화면에 원형 게이지와 회전 바늘이 나타나고, 바늘이 좁은 영역(great zone)에 들어올 때 버튼을 누르면 "great"로 진척이 가속되고, 넓은 영역(good zone)이면 무효과, 완전히 놓치면 "fail"로 진척이 후퇴하고 **큰 소음이 터져 살인마에게 위치가 노출**된다. 5개 발전기를 다 고치면 맵 양쪽의 **출구 게이트** 두 곳이 점등되고, 레버를 당겨 문을 열어 탈출한다. 마지막 생존자 한 명만 남으면 맵 어딘가의 **해치(hatch)**로 단독 탈출하는 길도 열린다.

**살인마 입장**: 1인칭(생존자는 3인칭) 시점으로 맵을 순찰하며 생존자를 찾는다. 살인마 주변에는 **공포 반경(Terror Radius)**이 있어, 그 안에 들어온 생존자는 심장박동음을 듣는다 — 즉 살인마가 다가오는 것을 거리감 있게 감지할 수 있다(반대로 살인마는 생존자의 정확한 위치를 모를 때가 많다). 생존자를 발견하면 추격이 시작되고, 기본 공격 두 방을 맞히면(첫 방=부상, 둘째 방=다운) 생존자가 쓰러진다. 살인마는 쓰러진 생존자를 들어 맵 곳곳의 **희생용 갈고리(hook)**로 옮겨 매단다.

### Hook — 3단계 처형 시스템
갈고리는 이 게임의 심장이다.
- **1단계(첫 걸림)**: 매달린 생존자는 자력 탈출을 시도하거나(낮은 확률), 동료가 다가와 구조할 수 있다. 시간이 지나면 2단계로 넘어간다.
- **2단계(투쟁 단계, struggle)**: The Entity의 촉수가 다가오며, 생존자는 스킬체크를 연속으로 성공시켜 버텨야 한다. 실패하면 사망.
- **3단계(희생)**: 세 번째로 갈고리에 걸리면 즉시 The Entity에게 제물로 바쳐져 사망한다.

이 구조는 "추격 → 다운 → 후킹 → 구조"라는 끝없는 줄다리기를 만든다. 살인마는 한 명을 집요하게 노려 빨리 제거할지(이른바 터널링), 압박을 분산할지 선택해야 하고, 생존자 팀은 누군가가 후킹될 때마다 "구조하러 갈 것인가, 발전기를 계속 돌릴 것인가"라는 자원 배분 결정을 반복한다.

### Mori와 기타 처형
특정 오퍼링이나 조건이 충족되면 살인마는 **Mori(처형 연출)**로 생존자를 직접 처치할 수 있다. 각 살인마 고유의 잔혹한 처형 애니메이션이 재생되며, 호러 IP 캐릭터의 경우 원작 분위기를 살린 연출이 큰 매력 포인트다.

### Bloodweb과 진행 구조
모든 캐릭터(생존자·살인마 각각)는 **Bloodweb(블러드웹)**이라는 거미줄 모양 스킬트리를 가진다. 한 판이 끝나면 행동에 따라 **블러드포인트(Bloodpoints)**를 얻고, 이를 Bloodweb에 투입해 퍽·아이템·애드온·오퍼링을 해금한다. 레벨 5/10/15에 추가 퍽 슬롯이 열리며, 레벨 50까지 키운 뒤에는 **프레스티지(Prestige)**로 단계를 올려 최대 prestige 100까지 갈 수 있다. 이 시스템은 "게임을 하면 할수록 빌드 선택지가 넓어지는" 장기 진행 동기를 제공하지만, 동시에 후술할 "그라인드(grind)" 비판의 원천이기도 하다.

### Perks — 게임의 전략적 깊이
**퍽(Perk)**은 이 게임의 전략적 핵심이다. 캐릭터당 최대 **4개**를 장착하며, 각 퍽은 3티어로 강화된다. 생존자 퍽은 130개 이상의 풀에서 추격 생존, 팀 정보 공유, 발전기 수리 속도, 반-터널(anti-tunnel) 보호 등에 특화돼 있고, 살인마 퍽은 120개 이상의 풀에서 발전기 후퇴, 오라 추적, 추격 우위, 후킹 압박, 엔드게임 봉쇄 등에 특화돼 있다. 핵심은 퍽이 특정 캐릭터에 묶여 있지 않고 **교차 해금(teachable)**된다는 점이다 — 한 캐릭터의 퍽을 다른 캐릭터에게 가르칠 수 있어, 수백 개 퍽의 조합으로 사실상 무한에 가까운 빌드가 만들어진다. PC Gamer가 "엄청나게 복잡한 다재다능한 빌드와 전략의 그물망"이라 표현한 깊이가 바로 여기서 나온다.

### 살인마별 비대칭 능력
각 살인마는 고유한 **특수 능력(Power)**을 가진다. 순간이동, 함정 설치(Trapper), 원거리 사슬·도구, 텔레포트, 은신, 추격 가속 등 능력이 제각각이라, 같은 게임이라도 어떤 살인마를 상대하느냐에 따라 생존자의 대응 전략이 완전히 달라진다. 이 "상대가 누구인지 모르고 매번 다른 위협을 마주하는" 가변성이 Coté가 말한 "무한한 순간 생성기"의 실체다.

### 라이브 운영 / 시즌 / MTX
- **2018년 6월**: 인게임 스토어 도입(코스메틱 판매)
- **2019년 10월**: 배틀패스(Rift) 시스템 도입
- **2020년**: 크로스플레이 / **2024년**: 크로스프로그레션
- DLC 챕터는 대개 신규 살인마 1 + 신규 생존자 1로 구성되며, 2026년 3월 기준 **총 47개 DLC**가 출시됐다. 그중 27개는 모든 플레이어가 쓰는 신규 맵을 동반했고, 3개(《The Last Breath》, 《Left Behind》, 《A Lullaby for the Dark》)는 무료 배포됐다.
- 정식 패치 전 Steam에서 **PTB(Public Test Build)**로 사전 테스트를 거친다.

### 대안 모드와 접근성
2024년부터 코어 4v1 외에 **Lights Out(시야 제한)**, **My Little Oni**, **Chaos Shuffle(무작위 퍽)**, **2v8(2 살인마 대 8 생존자)** 같은 한정 모드를 도입해 변주를 제공했다. 또한 2020년부터 시작된 멀티이어 그래픽 리워크로 출시 초기의 투박한 비주얼을 현세대 수준으로 끌어올렸다.

---

## 4. 평가

### 평론 — "엇갈리거나 평균적" 출발
| 매체 | 점수 |
|---|---|
| Metacritic (PC) | 71 / 100 ("mixed or average") |
| Metacritic (PS4) | 64 / 100 |
| Metacritic (Xbox One) | 58 / 100 |
| Metacritic (Switch) | 61 / 100 |
| GameSpot | 9 / 10 |
| IGN | 9 / 10 |
| PC Gamer UK | 88 / 100 |

주목할 점은 **평론이 크게 갈렸다**는 것이다. GameSpot은 9/10을 주며 "플레이어 커뮤니티 덕분에 Dead by Daylight는 비대칭 경쟁 멀티플레이어 영역에서 적수가 없다(without peer in the asymmetrical competitive multiplayer arena)"고 극찬했고, PC Gamer UK는 88점을 주며 "면도날처럼 날카로운 기계적 흥미, 엄청나게 복잡한 다재다능한 빌드와 전략의 그물망, 다양한 캐릭터 군"을 칭찬했다. 그러나 종합 메타스코어는 PC 71점에 머물렀다. 출시 당시 콘텐츠·맵·살인마 가짓수가 적어 "반복감이 빠르게 온다"는 지적이 점수를 끌어내린 것이다. 콘솔판은 초기 최적화 문제로 점수가 더 낮았다(Xbox One 58점).

이 "런칭 71점"은 Dead by Daylight 평가의 핵심 아이러니다 — 게임은 출시 시점이 아니라 **출시 이후 거의 10년간의 운영으로 평가받아야 하는 게임**이었다.

### 상업 지표 — 천천히, 그러나 끝없이
판매·플레이어 수는 시간이 지날수록 누적적으로 폭발했다.
- 첫 주 270,000+ 카피 → 2개월 내 100만 → 2017년 11월 300만 → 2019년 5월 500만 카피
- 플레이어 수: 2020년 8월 2,500만 → 2021년 5월 3,600만 → 2022년 5월 5,000만 → **2023년 11월 6,000만 명 이상**
- Steam 동시 접속 역대 최고 약 **120,700명**, 평시에도 5만 명 이상 동접 유지
- 전 플랫폼 월간 액티브 유저 약 800만~1,000만 명

Starbreeze 퍼블리싱 시절 데이터도 성장세를 뒷받침한다. 2017년 한 해 매출이 SEK 202,000,000(50/50 분배 대상), 누적 SEK 345,000,000에 달했고 당시까지 300만 카피가 팔렸다. 모바일판은 2020년 출시 48시간 만에 100만 다운로드, 2020년 10월 1,000만, 2022년 5월 2,500만 다운로드를 기록했다(NetEase 협업, 2023년 인도 차단, 2025년 3월 서비스 종료).

### 수상과 인정
Dead by Daylight는 "꾸준함"으로 인정받는 게임의 전형이다. Steam Awards의 **"Labor of Love(애정의 결실)"** 부문에 거의 매년 후보로 오르며, 9주년을 맞은 시점까지도 후보 캠페인을 진행했다. 단발성 GOTY보다는 "오래도록 살아 있는 게임"이라는 정체성으로 명성을 쌓았다.

### 유저 평가와 평론-유저 괴리
Steam 유저 평가는 대체로 긍정적이지만, 운영 이슈가 터질 때마다 출렁였다. 2021년 10월 Pinhead NFT 논란 당시에는 리뷰 폭격으로 "Mostly Negative"까지 떨어진 적도 있다(후술). 평론은 출시 시점 71점으로 미지근했지만, 유저들은 라이브 운영이 누적되며 점점 더 호의적으로 돌아섰다 — 이 게임에서 "평론-유저 괴리"는 점수 자체보다 **시점의 차이**에서 발생한다.

---

## 5. 성공 요인 분석 (핵심)

### 5-1. 비대칭 호러라는 "선점된 공백"
2016년 당시 "4 대 1 비대칭 멀티플레이어 호러"는 사실상 비어 있는 시장이었다. Dead by Daylight는 경쟁작 《Friday the 13th: The Game》보다 **약 1년 먼저** 출시되며 이 스타일을 메인스트림으로 끌어올렸다. 슬래셔 영화 관객이라면 누구나 직관적으로 이해하는 "한 명의 살인마, 여러 명의 희생자"라는 구도를 게임화한 것은, 마케팅을 따로 설명할 필요가 없는 강력한 컨셉이었다.

### 5-2. 호러 IP 총집합 전략 — 가장 결정적인 차별점
Dead by Daylight의 장수를 설명하는 단 하나의 요인을 꼽으라면 **라이선스 IP의 끝없는 흡수**다. The Entity라는 "무엇이든 빨아들이는" 세계관 장치 덕분에, 서로 무관한 호러 프랜차이즈를 무리 없이 한 게임에 모을 수 있었다.

출시 1주년인 2017년 10월, 첫 유료 라이선스 챕터로 《Halloween》의 **Michael Myers(The Shape)**와 생존자 Laurie Strode, 그리고 Haddonfield 맵을 추가했다. 이것이 첫 유료 DLC이자 첫 라이선스 캐릭터였고, 이후 Dead by Daylight는 호러 영화의 살아 있는 박물관이 되어 갔다 — 《A Nightmare on Elm Street》의 Freddy Krueger, 《Saw》, 《Silent Hill》, 《Resident Evil》, 《Alien》, 《Scream》의 Ghost Face, 《Texas Chainsaw Massacre》의 Leatherface, Chucky, 《Stranger Things》의 Demogorgon, 《Hellraiser》의 Pinhead, 그리고 Nicolas Cage까지. 23개 DLC가 라이선스 캐릭터를 담았다.

이 전략의 위력은 경쟁작과 비교하면 선명하다. 《Friday the 13th》, 《Evil Dead: The Game》, 《The Texas Chain Saw Massacre》는 각각 강력한 단일 IP에 의존했지만, 그 하나의 라이선스가 고갈되면 콘텐츠가 멈췄다. GamesRadar는 이 경쟁작들이 "썩어가는(rot)" 동안 Dead by Daylight는 "스스로를 먹여 살리는(self-feeding)" 호러 거인으로 Steam Top 50에 남아 있다고 평했다. DBD는 라이선스가 하나 빠지면 다른 라이선스를 끼워 넣으면 되는 **모듈식 콘텐츠 파이프라인**을 가진 유일한 게임이었다.

### 5-3. "무한한 순간 생성기"라는 설계 깊이
Coté가 의도한 무한 재플레이성은 단순한 표어가 아니라 시스템으로 구현됐다. 살인마마다 전혀 다른 능력, 수백 개의 교차 해금 퍽, 무작위 스킬체크, 가변적 맵 — 이 모든 요소가 결합해 매 판이 다른 긴장을 만든다. "내가 누구를 상대하는지 확신할 수 없다"는 정보 비대칭은 공포의 원천이자 학습 곡선의 원천이며, 플레이어를 수백 시간 붙잡아두는 깊이의 원천이다.

### 5-4. "처음부터 라이브 게임으로 만들지 않는다"는 운영 철학
2026년 GDC에서 Behaviour 측은 라이브서비스 성공 비결을 역설적으로 표현했다: **"You have to start by not making a live game(라이브 게임을 만들지 않는 것부터 시작해야 한다)."** 즉, 먼저 그 자체로 재미있고 완결된 코어 게임플레이 루프를 만든 뒤, 그 위에 콘텐츠를 쌓아 올렸다는 뜻이다. 많은 라이브서비스 게임이 수익 구조부터 설계하고 게임성을 뒤로 미루다 실패한 것과 대조적이다. 견고한 4v1 루프가 먼저 있었기에, 그 위에 47개 DLC를 얹어도 게임이 무너지지 않았다.

### 5-5. 퍼블리싱 권리 회수와 장기 투자
2018년 3월, Starbreeze는 Dead by Daylight의 퍼블리싱 권리를 개발사 Behaviour에 USD 16,000,000(초기 USD 4M + 게임 매출의 65% 로열티로 단계 지급되는 USD 12M)에 매각했다. 이로써 Behaviour는 자사 최대 흥행작의 운영·수익을 직접 통제하게 됐고, 장기 라이브 운영에 전권을 쥐고 투자할 수 있는 구조를 확보했다. 이 권리 회수는 게임의 10년 운영을 가능케 한 사업적 분기점이었다.

### 5-6. 커뮤니티와 크리에이터 생태계
Dead by Daylight는 스트리머·유튜버 친화적이다. 추격의 긴박함, 후킹·구조의 드라마, 살인마/생존자 양측 시청 모두 콘텐츠로서 매력적이라 트위치·유튜브에서 꾸준히 소비됐다. 또한 게임 크로스오버(Payday 2, For Honor, PUBG, Rainbow Six Siege, Balatro, Assassin's Creed Shadows 등)와 미디어 확장으로 IP 자체를 키워, 호러 팬덤 바깥으로도 인지도를 넓혔다.

---

## 6. 비평적 시각 / 한계 / 논란

### 6-1. 매치메이킹과 역할 불균형
가장 고질적인 문제는 **역할 인구 불균형**이다. 추격하는 살인마 역할은 1인분의 압박을 홀로 감당해야 해 스트레스가 크고, 보다 많은 플레이어가 생존자를 선호한다. 그 결과 살인마 큐 대기시간은 평균 약 422초에 달하는 반면 생존자는 약 21초에 불과하다는 분석이 있을 정도로 격차가 크다. 매치메이킹이 "균형 잡힌 매치"보다 "큐 시간 단축"을 우선하다 보니, 실력 차가 큰 매치가 빈번하다는 비판이 따른다.

### 6-2. 밸런스 논쟁 — 영원히 끝나지 않는 줄다리기
비대칭 게임의 숙명적 난제다. 최상위 조직 플레이(보이스 채팅으로 협력하는 4인 생존자)에서는 생존자가 더 강하고, 무작위로 매칭되는 퍼블릭 게임에서는 살인마가 더 강한 경향이 있다. 솔로큐 생존자는 팀 협력이 없어 특히 불리하다. 어느 한쪽을 버프하면 반대쪽이 불만을 터뜨리는 구조라, 패치마다 밸런스 논쟁이 재점화된다.

### 6-3. 비매너 플레이와 커뮤니티 독성
**터널링(tunneling)** — 한 생존자만 집요하게 노려 빨리 제거하는 전술 — 과 **슬러깅(slugging)** — 다운된 생존자를 후킹하지 않고 방치해 압박을 거는 전술 — 은 효율적이지만 당하는 입장에서는 극도로 불쾌해, 끝없는 논쟁의 대상이다. 또한 매치 후 채팅·제스처를 통한 도발 등 커뮤니티 독성(toxicity) 문제가 신규 유저 정착을 방해한다는 지적이 꾸준하다. 생존자 게임플레이가 살인마 추가에 비해 정체돼 있다는 불만도 있다.

### 6-4. 그라인드와 수익 모델
Bloodweb·프레스티지 시스템은 장기 동기를 주지만, 모든 퍽을 모으는 데 막대한 블러드포인트와 시간이 든다. 신규 유저가 경쟁력 있는 빌드를 갖추기까지의 그라인드가 진입 장벽이라는 비판이 있다. 또한 라이선스 DLC·코스메틱·배틀패스로 구성된 수익 구조는 "전부 사려면 비싸다"는 누적 비용 문제를 안는다.

### 6-5. NFT 논란 (2021)
2021년 10월, Pinhead(Hellraiser) 관련 NFT가 출시되자 커뮤니티가 강하게 반발해 Steam 평가가 한때 "Mostly Negative"까지 떨어지는 리뷰 폭격이 벌어졌다. Behaviour는 자사가 직접 관여한 것이 아니라고 해명했지만, 라이선스 파트너의 부수 사업이 게임 평판에 직격탄을 날린 사례로 남았다.

### 6-6. 라이선스 만료라는 구조적 리스크
호러 IP 총집합 전략은 양날의 검이다. 라이선스 계약이 만료되면 콘텐츠가 게임에서 제거된다. 《Stranger Things》는 2021년 라이선스 만료로 삭제됐다가 2023년 11월 재계약으로 복귀했고, 《Hellraiser》 콘텐츠는 2025년 4월 라이선스 문제로 제거됐으며(기구매자는 계속 플레이 가능), 상징적이게도 **Michael Myers의 《Halloween》 라이선스마저 2026년 1월 19일 제거**됐다(별도의 새 《Halloween》 게임 출시 예정 때문). 거의 10년간 게임의 얼굴이던 캐릭터가 떠나는 것은, 빌려온 IP에 의존하는 모델의 근본적 취약성을 보여준다.

---

## 7. 영향과 유산

### 7-1. 비대칭 호러 장르의 정의자
Dead by Daylight는 비대칭 멀티플레이어 호러를 하나의 독립 장르로 확립했다. 이후 《Friday the 13th: The Game》(2017), 《Evil Dead: The Game》(2022), 《The Texas Chain Saw Massacre》(2023), 《Propnight》, 《Video Horror Society》 등 수많은 후속·경쟁작이 등장했다. 이들 다수가 "DBD 공식"을 변주했지만, 단일 라이선스 의존이라는 약점 탓에 대부분 수명이 짧았다(《Evil Dead: The Game》은 2025년 스토어에서 내려갔다). Dead by Daylight만이 멀티 라이선스 + 오리지널 스토리 + 검증된 코어 루프의 결합으로 장르의 왕좌를 지켰다. GamesRadar의 표현대로, 경쟁작들이 "썩는" 동안 DBD는 Steam Top 50에 남았다.

### 7-2. 라이브서비스 운영의 교과서
거의 10년간 47개 DLC, 정기 패치, 그래픽 리워크(2020~), 2024년 Unreal Engine 5 마이그레이션, 대안 모드(2v8 등) 도입을 이어온 운영 모델은 "어떻게 게임을 장수시키는가"의 사례 연구가 됐다. "먼저 완결된 게임을 만들고, 그 위에 쌓아 올린다"는 철학, 그리고 PTB로 커뮤니티 테스트를 거치는 운영 방식은 후발 라이브서비스 개발자들이 참고하는 모델이다.

### 7-3. IP 컬래버레이션의 허브
Dead by Daylight는 단순한 게임을 넘어 **호러 IP의 교차로**가 됐다. 서로 다른 영화사·게임사·장르의 캐릭터가 한 무대에 서는 곳으로, 호러 팬에게는 "꿈의 대진표"를 실현하는 공간이다. 이는 IP 라이선싱이 게임의 핵심 사업 모델이 될 수 있음을 입증했다.

### 7-4. 미디어 프랜차이즈로의 확장
Dead by Daylight IP는 게임 바깥으로 뻗어 나갔다.
- **스핀오프 게임**: 《Hooked on You: A Dead by Daylight Dating Sim》(2022, 데이팅 시뮬레이션), 《What the Fog》(2024, 협동 로그라이크), 《The Casting of Frank Stone》(2024, Supermassive Games 제작 인터랙티브 드라마), 《Dead by Daylight Pinball》(2023)
- **보드게임**: Level 99 Games / Asmodee (2023년 4월)
- **만화**: Titan Comics 미니시리즈(Legion, Hillbilly 등)
- **영상화**: Blumhouse Productions와 Atomic Monster의 영화화 개발 진행(2026년 각본가 합류), 애니메이션 시리즈 개발 발표(2026)

### 7-5. 문화적·지역적 의미
일본은 일본 테마 챕터와 확장된 로어 덕에 최대 시장 중 하나가 됐고, 2021년 8월 도쿄 스카이트리에 Dead by Daylight 테마 카페 "The Entity Café"가 문을 열기도 했다. 게임이 단순 소비 콘텐츠를 넘어 오프라인 문화 현상으로 확장된 사례다.

---

## 8. 부록

### 핵심 통계 표
| 항목 | 수치 / 사실 | 출처 |
|---|---|---|
| PC 출시일 | 2016년 6월 14일 | Wikipedia |
| 엔진 | Unreal Engine 4 → UE5(2024.4) | Wikipedia / Unreal |
| Metacritic (PC) | 71/100 | Metacritic |
| GameSpot | 9/10 | GameSpot |
| PC Gamer UK | 88/100 | Wikipedia/PC Gamer |
| 첫 주 판매 | 270,000+ 카피 | Wikipedia |
| 누적 카피 | 2017.11 300만 / 2019.5 500만 | Wikipedia |
| 누적 플레이어 | 2023.11 기준 6,000만+ | Wikipedia |
| Steam 동접 최고 | 약 120,700명 | SteamCharts/IconEra |
| 총 DLC | 47개 (2026.3 기준, 라이선스 23개) | Wikipedia |
| Starbreeze→Behaviour 권리 매각 | USD 16,000,000 (2018.3) | Starbreeze IR |
| 2017년 매출 | SEK 202,000,000 (50/50 분배) | Starbreeze IR |

### 주요 인터뷰 / 강연
- Mathieu Coté & Dave Richard, GDC 2026 인터뷰 — Stephen King 영감, 라이브서비스 철학("start by not making a live game"), 2v8, 커뮤니티 (Newsweek)
- Mathieu Coté 인터뷰 — "infinite moment generator" 설계 철학 (TheGamer)
- "Living Through Dead by Daylight" — Unreal Engine 개발자 인터뷰 (engine 선택 이유)

### 참고 자료 목록
- Dead by Daylight — Wikipedia: https://en.wikipedia.org/wiki/Dead_by_Daylight
- "Living Through Dead by Daylight" — Unreal Engine: https://www.unrealengine.com/developer-interviews/living-through-dead-by-daylight
- Starbreeze sells rights to Dead by Daylight to Behaviour for USD 16 million — Starbreeze: https://www.starbreeze.com/2018/03/starbreeze-sells-rights-to-dead-by-daylight-to-behaviour-for-usd-16-million/
- Dead by Daylight developer to acquire publishing rights from Starbreeze — Game Developer: https://www.gamedeveloper.com/business/-i-dead-by-daylight-i-developer-to-acquire-publishing-rights-from-starbreeze
- Dead by Daylight Reviews — Metacritic: https://www.metacritic.com/game/dead-by-daylight/
- Dead by Daylight Reviews — GameSpot: https://www.gamespot.com/games/dead-by-daylight/reviews/
- GDC Interview: Dead by Daylight's Creators on Stephen King, 2v8, Community — Newsweek: https://www.newsweek.com/entertainment/gdc-interview-dead-by-daylights-creators-on-stephen-king-2v8-community-11669297
- Dead By Daylight Interview With Mathieu Côté — TheGamer: https://www.thegamer.com/dead-by-daylight-interview-mathieu-cote-jean-escalante/
- "the self-feeding horror giant still in the Steam Top 50" — GamesRadar+: https://www.gamesradar.com/games/survival-horror/
- 10 Licensed Horror Killers You Can Play in Dead By Daylight — Sideshow: https://www.sideshow.com/blog/10-licensed-horror-killers-dead-by-daylight
- Dead by Daylight Player Count and Statistics — IconEra: https://icon-era.com/blog/dead-by-daylight-player-count-and-statistics.548/

---

*본 분석서는 2026년 5월 기준 영어권 매체·개발자 인터뷰·상업 데이터를 토대로 작성됐다. 일부 운영·라이선스 현황(예: Halloween 라이선스 제거)은 시점에 따라 변동될 수 있다.*
