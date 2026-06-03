# 《Telling Lies》 (2019) 심층 분석

## 1. 게임 개요

《Telling Lies》는 2019년 8월 23일 출시된 내러티브 추리 게임이자 FMV(Full-Motion Video, 실사 동영상) 게임이다. 영국 출신의 게임 디렉터 **Sam Barlow**가 자신이 설립한 스튜디오 **Furious Bee**(이후 Half Mermaid Productions로 정비됨)와 함께 개발했고, 게임·영화·음악을 가로지르는 아트하우스 퍼블리셔 **Annapurna Interactive**가 배급했다. Barlow는 2015년 데뷔작 《Her Story》로 인디 게임계에 충격을 던졌고, 그 전에는 《Silent Hill: Origins》와 《Silent Hill: Shattered Memories》의 리드 디자이너·작가로 일했던 인물이다. 《Telling Lies》는 그 《Her Story》의 정신적 후속작(spiritual sequel)으로 기획됐다.

**출시일(플랫폼별)**

- iOS / macOS / Windows(PC): 2019년 8월 23일
- Nintendo Switch / PlayStation 4 / Xbox One: 2020년 4월 28일

흥미로운 점은 이 게임이 PC와 모바일(iOS)을 **동시 출시**했다는 사실이다. 검색·텍스트 입력을 핵심 메카닉으로 삼는 게임이라 태블릿·스마트폰 같은 터치 환경과 궁합이 좋았고, 실제 Metacritic 기준 iOS 버전(87점)이 PC 버전(84점)보다 높은 평점을 받았다.

**장르**: 인터랙티브 드라마 / 내러티브 미스터리 / FMV 추리

**주요 크레딧**

- 디렉터·각본: Sam Barlow
- 공동 각본: Amelia Gray(소설가, 《Maniac》《Mr. Robot》등 TV 작가 출신)
- 작곡: **Nainita Desai**(런던 출신 작곡가, 이후 《Immortality》도 담당)
- 음악 연주: London Contemporary Orchestra
- 출연(주연 4인):
  - **Logan Marshall-Green** — David Smith 역(영화 《Prometheus》《Upgrade》)
  - **Alexandra Shipp** — Ava 역(《X-Men: Apocalypse》의 스톰 역)
  - **Kerry Bishé** — Emma 역(《Halt and Catch Fire》)
  - **Angela Sarafyan** — Maxine Williams 역(《Westworld》)

**개발 기간·규모**: 개발은 **2016년 1월**에 시작되어 약 2년 반에 걸쳐 진행됐다. 로스앤젤레스 Mid-City 지역에서 약 6주에 걸쳐 촬영이 이뤄졌고, 주택 3채·아파트 4채·소규모 상점 1곳을 로케이션으로 활용했다. 촬영된 원본 푸티지는 **100시간 이상**이었으며, 이를 편집해 최종 게임에는 약 **10시간 분량**의 영상이 들어갔다. 이는 전작 《Her Story》(약 2시간 분량, 단일 취조실 세트)의 거의 5배에 달하는 규모다. Barlow는 게임 개발보다 영화 제작에 가까운 워크플로를 택했다 — 촬영에 들어가기 한참 전에 각본과 캐릭터, 주제를 확정해두고 프로덕션에 임했다.

**엔진/기술 스택**: 클라이언트는 Unity 엔진 기반으로 제작됐다. 그러나 이 게임의 본질은 그래픽 엔진이 아니라 **실사 영상 데이터베이스 + 검색 인터페이스**라는 소프트웨어 구조에 있다. 핵심은 "RETINA"라는 가공의 NSA 영상 아카이브를 시뮬레이션하는 검색 시스템이며, 플레이어가 입력한 키워드로 수백 개의 영상 클립을 검색해내는 메타데이터 매칭 엔진이 게임플레이의 골격이다.

---

## 2. 게임 설명

### 컨셉과 프레이밍

《Telling Lies》는 플레이어를 한 대의 노트북 앞에 앉힌다. 게임이 시작되면 우리는 어두운 방에서 노트북 화면을 마주한 **Karen**이라는 여성을 위에서 내려다본다(카메라가 노트북 웹캠 시점이다). Karen은 전직 NSA/FBI 관계자로, 미국 시민을 대규모 감시한 비밀 데이터베이스 RETINA의 하드드라이브 사본을 불법으로 빼낸 인물이다. 우리는 그녀의 어깨 너머로, 또는 정확히는 그녀의 노트북 화면을 통해 이 방대한 도청·영상 기록을 뒤지며 한 남자의 진실을 파헤친다.

게임 화면은 철저히 "데스크톱 메타포"로 구성된다. 화면 중앙엔 검색창과 영상 플레이어가 있고, 한쪽엔 메모장, 다른 쪽엔 사진·파일이 놓인 가상의 바탕화면이 있다. 플레이어는 이 데스크톱 위에서만 모든 것을 한다. 게임은 단 한 발자국도 "걷지" 않는다. 우리가 하는 일은 오직 검색하고, 보고, 듣고, 적는 것이다.

### 줄거리 [스포일러 포함]

[스포일러] 데이터베이스의 중심에는 **David Smith**라는 남자가 있다. 그는 FBI 요원으로, "Green Dagger"라는 코드명의 잠입 작전에 투입된 언더커버 에이전트다. 작전 목표는 환경 급진주의 단체 "Green Storm"(혹은 그 모체인 "Organizing Group")에 잠입해, 이들이 테러로 발전할지를 감시·적발하는 것이다. David는 "David Jones"라는 가명으로 활동가들 사이에 스며든다.

David의 사생활은 이미 곪아 있다. 그는 아내 **Emma**, 어린 딸 **Alba**와 가정을 꾸리고 있지만, 그 가정은 어두운 기원을 갖고 있다 — David는 Emma의 폭력적인 전 남자친구 Paul을 냉혹하게 살해한 뒤 Emma와 결혼했다. Emma는 시간이 흐를수록 David를 두려워하게 된다. 잠입 임무로 집을 비우는 일이 잦아지고, 부부 사이는 멀어진다.

잠입 현장에서 David는 젊은 활동가 **Ava**를 만나 사랑에 빠진다. 처음엔 임무의 일부였으나, David는 점차 환경 운동의 대의를 진심으로 믿게 되고, 결국 단체 내에서 가장 급진적인 인물로 변모한다. 감시자였던 그가 신봉자가 되어버리는 것이다. 작전 핸들러 Mike(혹은 상부)는 통제력을 잃어간다.

이중·삼중의 압박 속에서 David는 스트레스를 풀기 위해 **Maxine Williams**라는 여성이 운영하는 웹캠 채팅방을 드나든다. Maxine은 여러 개의 가명으로 캠 방송을 하는 성 노동자다. David는 돈을 내고 그녀와 대화하며, 점차 자신의 진짜 정체·임무·죄책감까지 털어놓는다. 외로운 David는 이것이 진짜 교감이라 믿기 시작한다. 그러나 Maxine에게 그는 손님 한 명일 뿐이다. 그녀는 David를 차단하지만 David는 집요하게 돌아오고, 마침내 Maxine은 그가 아는 자신의 모든 것이 거짓이며, 자신이 둘의 대화를 전부 녹화해뒀고 그가 계속 따라붙으면 이를 공개하겠다고 경고한다.

[스포일러] 절정에서 David는 자신의 보트에 폭탄을 싣고 파이프라인 다리를 폭파한다 — 그가 잠입했던 급진 단체의 이념을 그 스스로 실행에 옮긴 셈이다. 그는 보트 위에서 폭발과 함께 사실상 자살한다. 그를 둘러싼 두 여성, Emma와 Ava는 각자의 삶을 추슬러 David 없이 딸들을 키우며 살아간다. Maxine은 클리블랜드(오하이오)의 거처를 떠나 뉴욕에서 캠 에이전시를 차리고, 훗날 "강인한 여성 주인공"이 등장하는 범죄 소설을 쓰는 소설가가 된다. 그리고 모든 영상을 검토한 Karen은 결국 이 기록 전체를 세상에 유출한다.

이 게임의 진짜 주제는 잠입 작전이나 환경 테러가 아니다. **거짓말**이다. 모든 등장인물이 거짓을 산다 — David는 위장 신분으로, Maxine은 직업적 페르소나로, 사람들은 화면 앞에서 자기 자신을 연기한다. 그리고 마지막에는 플레이어 자신, 즉 Karen조차 무언가를 숨기고 있음이 드러난다. 게임은 "당신은 어떤 거짓말을 보고 있고, 어떤 진실을 골라 믿을 것인가"를 묻는다.

### 캐릭터

- **David Smith / David Jones** (Logan Marshall-Green): 게임의 중심축. FBI 언더커버 요원이지만 잠입한 이념에 동화되고, 가정·임무·캠 채팅이라는 세 거짓 사이에서 붕괴해간다. 매력적이지만 위험하고, 동정과 혐오를 동시에 자아내는 인물.
- **Ava** (Alexandra Shipp): 환경 활동가. David가 사랑에 빠지는 상대이자, 그의 변절을 촉발하는 인물. 순수한 신념의 화신처럼 그려진다.
- **Emma** (Kerry Bishé): David의 아내. 그가 살해한 남자의 옛 연인이었고, David를 점점 두려워하게 된다. 가정의 붕괴를 가장 가까이서 견디는 인물.
- **Maxine Williams** (Angela Sarafyan): 여러 가명으로 활동하는 캠 성 노동자. David에게 거짓 친밀함을 팔지만, 결국 자신의 기록으로 David를 무너뜨리는 능동적 행위자다. 게임에서 가장 자기 운명을 스스로 결정짓는 캐릭터.
- **Karen** (플레이어 아바타): 우리가 조종하는 시점 인물. 화면 밖에 있는 듯하지만 게임은 그녀의 정체와 동기를 조금씩 흘린다.

### 무드/톤/아트 디렉션

전체적인 톤은 차갑고 관음적이며 불안하다. Barlow는 영감의 원천으로 Francis Ford Coppola의 1974년작 《The Conversation》(감청·도청에 대한 편집증적 영화)과 Steve McQueen의 2011년작 《Shame》(성 중독과 고립)을 직접 언급했다. 비선형 편집의 거장 Nicolas Roeg 감독의 스타일도 참조점이었다. 화면은 한밤의 노트북 불빛처럼 어둡고, 영상 클립들은 흔들리는 손, 거친 노이즈, 비대칭 구도로 일상의 도청 영상 같은 날것의 질감을 갖는다. Barlow는 "아무도 그렇게 촬영하지 않는다. 모두가 자기 안전지대 밖에 있었다(Nobody shoots like that. Everyone was out of their comfort zone)"고 촬영 과정을 회고했다 — 영화 문법을 일부러 깨뜨려, 감시 카메라가 우연히 잡아낸 사적 순간 같은 불편한 진정성을 노린 것이다.

### 사운드/음악

작곡은 **Nainita Desai**가 맡았다. 그녀는 프로젝트 초기, Barlow가 트위터로 직접 연락해 합류했다. 특이하게도 Desai는 **촬영이 시작되기도 전에 각본만 받고 먼저 스코어를 작곡**했다 — 영화 음악에서도 드문 역순 작업이었다. 스코어는 **London Contemporary Orchestra**가 연주했고, 친밀한 현악·목관·피아노·하프를 중심으로 한다. Hitchcock의 미스터리, Fincher의 음울함, Lynch적 초현실주의를 동시에 환기한다는 평을 받았다. 'Spectral Scrubbing'이라는 독특한 확장 연주 기법을 도입해, 플레이어가 영상 타임라인을 앞뒤로 긁을(scrub) 때의 공기감·부유감을 음악으로 형상화했다. 이 사운드트랙은 Hollywood Music in Media Awards, Music + Sound Awards 등에서 후보·수상 대상이 됐다.

---

## 3. 핵심 시스템 / 메카닉

《Telling Lies》의 게임플레이는 거의 전부가 **검색**이라는 단일 행위 위에 세워져 있다. 그러나 그 단순한 행위 위에 정교한 제약과 리듬이 얹혀, 한 편의 추리극을 능동적으로 재구성하게 만든다.

### 코어 게임플레이 루프

1. **키워드 검색**: 플레이어는 화면의 검색창에 단어나 짧은 구절을 입력한다. RETINA 데이터베이스는 영상 속 인물이 **그 단어를 실제로 발화한** 클립들을 찾아 반환한다.
2. **상위 5개만 반환**: 검색 결과는 최대 **5개의 클립**만 표시된다. 같은 단어가 100개의 영상에서 나왔어도, 우리는 그중 (대체로 시간순 또는 관련도순) 다섯 개만 볼 수 있다. 따라서 더 희귀하고 구체적인 단어를 찾아낼수록 더 깊은 영상에 도달한다.
3. **발화 지점부터 재생**: 클립은 처음부터가 아니라 **검색한 단어가 발화된 그 순간부터** 재생된다. 만약 5분짜리 대화의 4분 30초 지점에서 그 단어가 나왔다면, 우리는 일단 마지막 30초만 볼 수 있다.
4. **수동 스크럽**: 그 앞부분(처음 4분 30초)을 보려면 플레이어가 직접 타임라인 슬라이더를 **거꾸로 긁어서** 되감아야 한다. 이 "스크럽" 동작 자체가 게임의 촉각적 핵심이다. Barlow는 《The Conversation》에서 도청 테이프를 앞뒤로 돌리는 행위에 대한 "페티시"를 의도적으로 차용했다고 밝혔다.
5. **반쪽짜리 대화**: 결정적 제약이 여기 있다. 영상은 **대화 당사자 한쪽만** 보여준다. 화상 통화 장면이라도 우리는 화면에 잡힌 한 사람의 피드만 보고, 상대방의 영상과 목소리는 **들리지 않는다**(상대의 마이크는 녹음되지 않았다는 설정). 따라서 한 대화의 "반대쪽"을 보려면, 그 상대방이 한 말 속의 키워드를 따로 추론해 **다시 검색**해 별개의 클립으로 찾아내야 한다.
6. **트랜스크립트 누적과 단서 확장**: 영상을 볼수록 대사가 메모/트랜스크립트에 쌓이고, 거기서 새로운 검색어가 떠오른다. 이름·장소·은어·구체적 표현 하나가 다음 검색의 열쇠가 된다. 이렇게 **하나의 단서가 다음 단서를 낳는** 연쇄가 진행 구조 전체를 형성한다.

### 진행 구조: "수직으로 파고드는" 비선형 서사

Barlow의 핵심 디자인 철학은 서사가 **옆으로(시간순으로) 흐르지 않고 아래로(주제·맥락으로) 파고든다**는 것이다. 플레이어는 이야기를 시간 순서대로 받지 않는다. 어떤 단서에 끌리느냐에 따라 1년 차의 한 장면을 보다가 갑자기 작전 막바지의 장면으로 점프한다. 같은 사건을 여러 시점·여러 시기에 걸쳐 거듭 마주치며, 매 조우마다 의미와 서브텍스트가 한 겹씩 깊어진다. Barlow는 이를 두고 "관객에게 항복하고 스스로 길을 찾게 두는 것이므로, 산산조각 내어 부품으로 만들어도 작동하는 이야기를 지어야 한다"고 설명했다.

이는 학계에서 "게이티드 스토리 구조(Gated Story Structure)"로 분석되기도 했다(Springer 논문 《Gated Story Structure and Dramatic Agency in Sam Barlow's Telling Lies》). 모든 클립이 처음부터 열려 있지만, 실질적으로는 플레이어가 올바른 키워드를 떠올려야만 다음 영상에 "도달"할 수 있어, 자유 탐색처럼 보이는 구조 안에 자연스러운 진행의 문턱(gate)이 박혀 있다는 것이다.

전작 《Her Story》가 단일 취조실·단일 배우라는 극도로 제한된 무대에서 작은 단서의 어긋남까지 집착하게 만들었다면, 《Telling Lies》는 4명의 인물·수십 개의 로케이션·2년의 시간이라는 광대한 공간을 펼쳐놓는다. Barlow는 이 확장의 모델로 의외의 작품을 들었다 — 《The Legend of Zelda: Breath of the Wild》다. 그는 BotW가 오픈월드 탐험을 "관대하게" 보상하는 방식, 즉 모든 디테일을 강박적으로 추적하지 않아도 흥미를 따라가다 보면 이야기가 엮이는 구조에서 영감을 받았다고 했다.

### 시간 제약과 "마이크" 메카닉

게임에는 미묘한 시간·세션 압박 장치가 있다. Karen이 데이터베이스에 접근하는 시간은 사실상 한정돼 있고(노트북 배터리·하룻밤이라는 프레이밍), 한 번의 플레이로 10시간 분량 전부를 보는 것은 불가능에 가깝다. 따라서 플레이어는 **무엇을 볼지 취사선택**해야 하며, 이 선택이 어떤 캐릭터의 이야기를 더 깊이 보게 되는지를 좌우한다. 게임이 제공하는 **세 가지 엔딩**은 플레이어가 어느 인물의 영상을 가장 많이 탐색했느냐에 따라 갈린다 — 누구의 진실에 더 귀 기울였는가가 곧 결말의 색채를 결정하는 셈이다.

### UI/UX 디자인 철학

- **데스크톱 = 게임 세계**: 별도의 게임 월드 없이 노트북 화면 그 자체가 유일한 공간이다. 메모장에 직접 메모하고, 사진을 열어보고, 검색 기록이 쌓인다. 이 "발견된 인터페이스(found interface)" 미학은 이후 데스크톱 호러·추리 장르(《Her Story》 계보)의 토대가 됐다.
- **웹캠 시점의 이중 관음**: 게임은 영상 속 인물을 우리가 훔쳐보게 하는 동시에, 노트북 웹캠을 통해 플레이어(Karen)도 카메라에 잡혀 있음을 끊임없이 상기시킨다. 어두운 방에서 가끔 화면에 비치는 Karen의 실루엣은 "보는 자도 보여지고 있다"는 주제를 UI 차원에서 구현한다.
- **터치 친화 설계**: 키워드 입력·타임라인 스크럽·클립 선택이라는 동작은 마우스보다 손가락에 더 자연스러워, iOS·터치스크린에서 빛을 발한다. 동시 출시 전략이 메카닉과 맞물린 드문 사례다.
- **접근성**: 자막·트랜스크립트가 기본 제공되며(대사 자체가 게임플레이 데이터이므로), 액션 반응 속도가 전혀 요구되지 않아 운동·반응 능력에 관계없이 플레이 가능하다. 다만 영어 음성·텍스트 의존도가 절대적이라, 비영어권 플레이어에게는 언어 장벽이 실질적 진입 장벽으로 작용한다.

---

## 4. 평가

### 평론 점수

《Telling Lies》는 "대체로 호의적(generally favorable)" 평가를 받았다.

- **Metacritic**: iOS 87 / PC 84 / Nintendo Switch 80 / Xbox One 80 / PlayStation 4 79
- **OpenCritic**: 약 86점

주요 매체 점수:

| 매체 | 점수 |
|------|------|
| IGN | 9/10 |
| Game Informer | 9/10 |
| Edge | 9/10 |
| Destructoid | 9/10 |
| PC Gamer (US) | 87/100 |
| GamesRadar+ | 4.5/5 |
| GameSpot | 7/10 |
| Eurogamer | Recommended |

대표 인용:

- **IGN (9/10)**: "날카로운 각본, 설득력 있는 연기, 비틀린 플롯이 《Telling Lies》를 반드시 해봐야 할 탐정 게임으로 만든다(Sharp writing, believable acting and a twisting plot make Telling Lies an essential detective game)."
- **GamesRadar+ (4.5/5)**: "탐색이 완전히 유기적이고 아름답게 페이싱된 느낌(totally organic and beautifully paced)"이라 평하며 "Sam Barlow가 또 하나의 걸작을 손에 쥐었다"고 했다.
- **Kotaku**: 출연진을 "한결같이 탁월하며, FMV 게임에서 본 그 어떤 것보다 뛰어난 연기를 보여준다(uniformly excellent, delivering performances far beyond anything I've seen in an FMV game)"고 평했다.
- **Rock Paper Shotgun**: "전작보다 더 크고, 더 좋고, 더 빠르고, 더 강하다(bigger, better, faster, stronger)"고 요약했다.
- **The Washington Post**: "올해의 가장 빼어난 게임 중 하나(one of the most brilliant games of the year)"로 꼽았다.
- **Eurogamer**: "미지의 영역으로 내딛는 두 번째 아장걸음 — 조금 불안하고 조금 순진하지만, 분명히 용감하고 흥미롭다(a second baby step into uncharted territory: a little wobbly, a little naive. But definitely courageous and exciting)."

### 수상 이력

- **Golden Joystick Awards**: Best Performer 수상 — Logan Marshall-Green
- **Webby Awards**: Best User Experience 수상
- **Pocket Gamer Mobile Games Awards**: Best Storytelling 수상
- **BAFTA Games Awards 2020**: Performer in a Leading Role 후보 — Logan Marshall-Green
- **Writers' Guild of Great Britain**: Best Writing in a Video Game 후보
- **DICE Awards**: Outstanding Achievement in Story 후보
- 그 외 NAVGTR Awards, Hollywood Music in Media Awards, Music + Sound Awards 등에서 후보·수상

IMDb 집계 기준 약 3개 수상·5개 후보 안팎으로 정리된다. 연기상 트랙에서 두드러진 성과를 낸 점이 FMV 장르의 특성을 잘 보여준다 — 이 게임은 게임 디자인만큼이나 배우의 연기로 평가받았다.

### 상업 지표

Annapurna Interactive와 Sam Barlow 측은 《Telling Lies》의 정확한 판매량을 공개하지 않았다. 다만 다음 맥락이 상업적 위상을 가늠하게 한다 — 전작 《Her Story》가 인디로서는 이례적으로 100만 본 이상 팔리며 작은 예산 대비 큰 성공을 거뒀고, 이를 발판으로 Barlow는 Annapurna라는 강력한 퍼블리셔, 할리우드급 배우진(Logan Marshall-Green, Alexandra Shipp 등), 6주 로케이션 촬영이라는 훨씬 큰 예산을 확보할 수 있었다. 즉 《Telling Lies》는 그 자체로 막대한 흥행 신화를 쓰진 않았지만, "한 사람의 실험적 인디 히트작이 어떻게 정규 스튜디오 프로덕션으로 스케일업되는가"를 보여준 사례다. PC·모바일·콘솔 전 플랫폼 출시와 꾸준한 세일을 통해 롱테일로 회수하는 전형적인 프리미엄 내러티브 게임의 경로를 밟았다.

### 유저 평가와 평론-유저 괴리

평론은 전반적으로 높았으나, 유저 반응은 평론보다 다소 갈렸다. Steam·유저 리뷰에서는 "연기와 분위기는 훌륭하지만 검색 메카닉이 후반부로 갈수록 반복적이고 막막해진다", "전작 《Her Story》의 응축된 마법을 그리워하게 된다"는 의견이 적지 않았다. IMDb 유저 평점이 6.5 수준에 머문 것도 이 온도차를 반영한다. 즉 비평적으로는 "야심차고 성취 있는 작품"으로, 일부 플레이어에게는 "전작만큼 손에 쥐어지지 않는 확장판"으로 받아들여진 셈이다.

---

## 5. 성공 요인 분석

### 디자인 측면

1. **"검색이 곧 플레이"라는 발명의 확장**: 《Her Story》에서 Barlow는 "비디오 영상에 탐험형 게임플레이를 적용한다"는 발상을 증명했다. 《Telling Lies》는 이를 "어떻게 더 넓고 더 촉각적으로 만들 것인가"로 밀어붙였다. 단순 키워드 검색에 그치지 않고, 발화 지점부터 재생·수동 스크럽·반쪽 대화라는 제약을 더해, 검색 행위에 추리적 마찰과 긴장을 부여했다.
2. **제약이 만드는 추리극**: "상대방 목소리가 들리지 않는다"는 단 하나의 제약이, 플레이어를 능동적 탐정으로 변모시킨다. 빈 곳을 추론으로 채우고, 다시 검색으로 검증하는 루프가 게임 전체를 관통한다.
3. **연기·각본의 질**: FMV 장르의 고질병은 어설픈 연기와 캠피한 톤이었다. Barlow는 진짜 영화·TV 배우를 캐스팅하고 소설가 Amelia Gray와 공동 집필함으로써, 장르의 오명을 정면으로 반박했다. 비평이 "연기"를 가장 먼저 칭찬한 것은 이 전략의 성공을 보여준다.
4. **음악의 선제 작곡**: 촬영 전에 스코어를 먼저 만들어 영상의 톤을 사전 규정한 워크플로는, 결과적으로 게임 전체에 일관된 정서적 통일감을 부여했다.

### 마케팅·출시 전략

- **Annapurna Interactive의 브랜드 효과**: 《Journey》《What Remains of Edith Finch》《Outer Wilds》등 평단 호평작을 큐레이션해온 Annapurna는 "아트하우스 게임"의 보증수표였다. 그 라인업에 합류했다는 사실 자체가 핵심 마케팅이었다.
- **E3 2019 데모·언론 인터뷰**: 출시 전 E3 데모와 다수의 디렉터 인터뷰(Engadget, Hollywood Reporter, MCV/DEVELOP 등)를 통해 "《Her Story》의 그 사람이 만든 더 큰 게임"이라는 서사를 일찌감치 구축했다.
- **PC·모바일 동시 출시**: 메카닉과 플랫폼을 정확히 매칭한 보기 드문 사례로, 모바일 내러티브 게임 시장까지 동시에 공략했다.

### 타이밍·시장 환경

2019년은 감시 자본주의, NSA·스노든 폭로의 여파, 데이터 프라이버시 논쟁이 대중 의식에 깊이 자리 잡은 시기였다. RETINA라는 대규모 웹캠 감시 데이터베이스라는 설정은 시대적 불안을 정확히 건드렸다. 동시에 데스크톱·발견형 인터페이스 게임(《Her Story》《Orwell》《Hypnospace Outlaw》등)에 대한 관심이 한창 무르익던 때이기도 했다.

### 개발·운영 방법론

Barlow의 "영화식 워크플로"(촬영 전 각본·캐릭터·주제 확정, 음악 선작곡)는 이 장르에서 거의 독보적이다. 그는 게임 개발 일정 안에서 즉흥적으로 내러티브를 끼워 맞추는 대신, 마치 영화감독처럼 사전 제작에 자원을 집중했다. 이 방법론이 산만해지기 쉬운 비선형 서사에 단단한 주제적 척추를 부여했다.

### 동시기 작품 대비 차별점

같은 시기 다른 내러티브 게임들(텔테일식 선택형 분기, 워킹 시뮬레이터)이 "선택의 환상" 또는 "선형 산책"에 머물렀다면, 《Telling Lies》는 **플레이어의 호기심과 추론을 진짜 게임 메카닉으로** 전환했다. 이야기를 받는 게 아니라 발굴하게 만든다는 점에서, 인터랙티브 내러티브의 한 극단을 대표한다.

---

## 6. 비평적 시각 / 한계 / 논란

### "더 커졌지만 더 나아지진 않았다"

가장 자주 제기된 비판은 Engadget의 리뷰 제목이 압축한다 — "《Telling Lies》는 《Her Story》보다 더 크지만, 더 낫지는 않다(bigger, but not better)." 비판의 핵심은 **확장이 응축의 마법을 희석했다**는 것이다.

- **검색 시스템과 규모의 충돌**: 《Her Story》의 검색은 단일 취조실·단일 배우라는 좁은 무대 덕분에 완벽히 작동했다. 모든 디테일이 한 공간에 모여 있어 작은 어긋남도 포착됐다. 반면 《Telling Lies》는 이름·조직·장소·인물이 소방 호스처럼 쏟아져, 플레이어가 무엇을 검색해야 할지 길을 잃기 쉽다. 후반부로 갈수록 "다음 키워드"를 찾는 일이 추리가 아니라 막막한 노동처럼 느껴질 수 있다.
- **캐릭터 클리셰**: Engadget은 등장인물이 "매끄럽지만 고뇌하는 스파이, 순진한 활동가, 이중적인 성 노동자"라는 익숙한 틀에 빠진다고 지적했다. 한 장면에서 6분에 걸쳐 역사적 트라우마를 설명하는 노골적인 해설 대사도 도마에 올랐다.
- **반쪽 대화의 피로**: 모든 대화의 반대편을 따로 찾아야 한다는 제약은 처음엔 영리하지만, 10시간 분량에 걸쳐 반복되면 인내심을 시험한다. 한쪽 화면만 보며 한참을 듣는 구조가 단조롭게 느껴질 수 있다.

### 관음·재현의 문제

게임의 주제 자체가 관음(voyeurism)인 만큼, 카메라가 인물(특히 Maxine 같은 성 노동자, Ava 같은 여성 캐릭터)을 응시하는 방식이 비판적 시선에 노출됐다. 게임은 "보는 행위의 윤리"를 의식적으로 문제 삼고 플레이어를 공범으로 끌어들이지만, 그 의도가 모든 플레이어에게 균등하게 전달되지는 않았다. 일부에게는 주제적 자의식으로, 일부에게는 단지 불편한 응시로 읽혔다.

### 평가가 갈리는 지점

비평가들은 야심과 성취에 후한 점수를 줬지만(IGN·Edge·Game Informer 9점), GameSpot(7점)처럼 "전작의 정교함에 못 미친다"는 신중한 평가도 분명히 존재했다. 결국 이 게임은 "Barlow의 발명을 더 큰 캔버스로 확장한 용감한 시도"라는 합의와 "그 확장이 핵심 매력을 약화시켰다"는 유보 사이에서 줄곧 진동했다.

---

## 7. 영향과 유산

### 장르에 미친 영향

《Telling Lies》는 《Her Story》와 함께 **"검색·발견형 FMV 추리"**라는 하위 장르를 정립한 두 기둥 중 하나다. Sam Barlow는 이 게임으로 단발 히트가 아니라 **일관된 작가적 형식**을 가진 게임 작가임을 증명했다. 데스크톱 인터페이스, 비선형 데이터베이스 서사, 실사 배우 활용, 음악의 선제 작곡 같은 요소가 그의 시그니처로 굳어졌다.

### 후속작과 작가적 진화

- **《Immortality》(2022)**: Barlow와 작곡가 Nainita Desai는 다음 작품 《Immortality》에서 다시 협업했다. 사라진 여배우가 출연한 미공개 영화 3편을 뒤지는 이 게임은 《Telling Lies》의 "영상 데이터베이스 탐색" 메카닉을 한층 진화시켜, 영상 속 특정 사물·인물을 클릭해 다른 영상으로 점프하는 "매치 컷" 메카닉을 도입했다. 《Immortality》는 BAFTA 다관왕을 포함해 더 큰 평단 성공을 거뒀다. 《Telling Lies》는 《Her Story》(증명)에서 《Immortality》(완숙)로 가는 **결정적 중간 단계**이자 실험대였다.
- Barlow의 스튜디오는 Half Mermaid로 정착해 이 형식을 전문 영역으로 삼았다.

### 산업적 의미

이 게임은 인디 출신 작가가 "한 번의 발명"을 어떻게 자본·인력·연기력이 투입된 정규 프로덕션으로 스케일업하는지를 보여준 사례다. FMV라는, 1990년대 이후 오랫동안 조롱받던 장르를 진지한 작가주의 영역으로 끌어올리는 데 결정적으로 기여했다. 또한 게임과 영화·TV 산업의 경계를 흐리는 흐름(할리우드 배우의 게임 출연, 영화식 사전 제작 워크플로)의 선구적 사례이기도 하다.

### 문화적 의미

감시 시대의 불안, 디지털 친밀함의 거짓됨, "우리는 모두 화면 앞에서 자신을 연기한다"는 주제를 게임 메카닉 그 자체로 구현했다는 점에서, 《Telling Lies》는 단순한 추리 게임을 넘어 **매체에 대한 매체적 성찰**로 읽힌다. 플레이어를 관음자이자 유출자(leaker)로 세우고, 그 윤리적 무게를 직접 짊어지게 한다는 점에서 인터랙티브 내러티브가 도달할 수 있는 주제적 깊이의 한 표본을 남겼다.

---

## 8. 부록

### 주요 인터뷰·강연 자료

- Engadget, "'Telling Lies' and the new nonlinear narrative" (2019.6.13) — 비선형 서사 디자인 철학, E3 데모 인터뷰
- Engadget, "'Telling Lies' is bigger, but not better, than 'Her Story'" (2019.8.21) — 규모 확장의 명암에 대한 비평
- MCV/DEVELOP, "Nobody shoots like that. Everyone was out of their comfort zone — Sam Barlow on the process behind making Telling Lies" — 촬영 과정·연출 방법론
- The Hollywood Reporter, "'Telling Lies' Director on Merging Traditional Storytelling With Interactive Video"
- ScreenAnarchy, "Interview: Sam Barlow Talks TELLING LIES and the Future of Interactive Movies" (2019.5)
- Game Developer (Gamasutra), "Composing a soundtrack to match the intimate game design of Telling Lies" — Nainita Desai의 음악 작업
- My Perfect Console with Simon Parkin — Sam Barlow 게임 디렉터 에피소드
- Springer, "Gated Story Structure and Dramatic Agency in Sam Barlow's Telling Lies" (학술 분석, 2020)

### 핵심 통계 표

| 항목 | 내용 |
|------|------|
| 개발사 | Sam Barlow / Furious Bee (Half Mermaid) |
| 퍼블리셔 | Annapurna Interactive |
| 디렉터·각본 | Sam Barlow (공동 각본 Amelia Gray) |
| 작곡 | Nainita Desai (London Contemporary Orchestra 연주) |
| 출시 | 2019.8.23 (iOS/macOS/PC), 2020.4.28 (Switch/PS4/Xbox One) |
| 장르 | 인터랙티브 드라마 / FMV 추리 |
| 개발 시작 | 2016년 1월 |
| 촬영 | LA Mid-City, 약 6주, 로케이션 8곳 |
| 촬영 분량 | 원본 100시간+ → 최종 약 10시간 |
| 주연 | Logan Marshall-Green, Alexandra Shipp, Kerry Bishé, Angela Sarafyan |
| 엔딩 | 3종 (가장 많이 탐색한 인물에 따라 분기) |
| Metacritic | iOS 87 / PC 84 / Switch 80 / Xbox 80 / PS4 79 |
| OpenCritic | 약 86 |
| 대표 수상 | Golden Joystick Best Performer, Webby Best UX, Pocket Gamer Best Storytelling |

### 핵심 메카닉 요약

- RETINA(가공의 NSA 웹캠 감시 데이터베이스)에서 키워드로 영상 검색
- 검색 결과는 최대 5개 클립, 발화 지점부터 재생, 앞부분은 수동 스크럽
- 대화는 한쪽 인물만 표시 — 반대쪽은 별도 키워드로 따로 검색
- 트랜스크립트 누적 → 새 검색어 연쇄 → 수직적 비선형 서사
- 노트북 데스크톱 메타포, 웹캠 시점의 이중 관음

### 참고 자료 목록 (영어권 매체 중심)

- Wikipedia, "Telling Lies (video game)"
- Metacritic — Telling Lies (플랫폼별 평점)
- OpenCritic — Telling Lies
- IGN, Game Informer, Edge, Destructoid, PC Gamer, GamesRadar+, GameSpot, Eurogamer, Kotaku, Rock Paper Shotgun, The Washington Post 리뷰
- Engadget (인터뷰·비평 2건)
- MCV/DEVELOP, The Hollywood Reporter, ScreenAnarchy (디렉터 인터뷰)
- Game Developer / Soundlister / TheGamer (Nainita Desai 음악 인터뷰)
- Nainita Desai 공식 사이트 (nainitadesai.com)
- Springer Link, "Gated Story Structure and Dramatic Agency in Sam Barlow's Telling Lies" (학술 논문)
- TheGamer, "Every Major Telling Lies Spoiler, Explained" (플롯·엔딩 해설)
- Annapurna Interactive 공식 페이지

---

*본 분석서는 2019년 출시작 《Telling Lies》에 대한 영어권 자료 기반 한국어 심층 분석이다. 플롯 관련 서술에는 결말 스포일러가 포함되어 있으며, 판매량 등 비공개 수치는 추정·맥락으로만 다루었다.*
