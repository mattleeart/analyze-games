# 《Pizza Tower》 (2023) 심층 분석

> 5년의 익명 개발, MS 페인트를 닮은 1990년대 카툰 미학, 시속 100마일의 광기 어린 플랫포밍. 닌텐도가 15년간 방치한 《Wario Land》 시리즈의 빈자리를 한 명의 익명 디자이너와 한 명의 프로그래머가 채워 넣었고, 그 결과물은 Steam 역사상 가장 높은 평가를 받은 2D 플랫포머가 되었다.

---

## 1. 게임 개요

《Pizza Tower》는 인디 개발팀 **Tour De Pizza**가 제작하고 2023년 1월 26일 Windows(Steam)로 출시한 2D 사이드스크롤 액션 플랫포머다. 가격은 미국 기준 약 20달러였다.

| 항목 | 내용 |
|------|------|
| 개발사 | Tour De Pizza |
| 퍼블리셔 | Tour De Pizza, Fangamer(상품화·물리 에디션) |
| 출시일(PC) | 2023년 1월 26일 (Windows / Steam) |
| 출시일(콘솔) | 2024년 8월 27일 (Nintendo Switch, Nintendo Indie World 발표) |
| 장르 | 2D 사이드스크롤 액션 플랫포머, 스코어 어택 |
| 엔진 | GameMaker |
| 가격 | 약 19.99달러 |

**주요 크레딧.** 개발은 익명의 디자이너 겸 아티스트 **McPig**(별명 "Pizza Tower Guy")와 프로그래머 **Sertif**가 주도했다. McPig은 게임의 기획·아트·애니메이션 전반을 담당했고, Sertif는 프로그래밍과 메카닉 구현을 맡았다. 음악은 **Ronan "Mr. Sauceman" de Castel**, **ClascyJitto**(별명 Frostix), 그리고 타이틀 화면 곡을 맡은 익명의 **Post Elvis**가 담당했다. 두 메인 작곡가가 사운드트랙의 절반씩을 나눠 작업했다.

**개발 기간과 규모.** 약 5년에 걸쳐 개발되었다. McPig은 2018년경부터 작업을 시작했고, Sertif는 2020년 초에 합류한 것으로 알려져 있다. 핵심 인력은 사실상 두 명이었으며, 음악·플레이테스트 등에 소수의 협력자가 가세하는 전형적인 초소형 인디 구조였다. 예산은 공개되지 않았으나, 개발 자금의 상당 부분은 출시 전 Patreon 후원(월 5달러 구독자에게 얼리 액세스 빌드 제공)으로 충당되었다. 약 30명 규모의 테스터 그룹을 운영해 레벨 난이도를 조정한 것으로 알려져 있다.

**기술 스택.** 게임 엔진은 GameMaker(GameMaker Studio 계열)이며, 애니메이션 제작 도구로는 **Aseprite**가 사용되었다. 고해상도 픽셀아트 기반의 카툰풍 스프라이트가 특징이다.

---

## 2. 게임 설명

### 컨셉과 세계관

플레이어는 이탈리아인 피자 셰프이자 망해 가는 피자가게 점주인 **Peppino Spaghetti**(페피노 스파게티)를 조작한다. 어느 날 의식을 가진 채 떠다니는 거대한 피자 **Pizzaface**(피자페이스)가 나타나, 가게 옆에 솟은 거대한 탑(Pizza Tower) 꼭대기의 핵 레이저로 페피노의 피자가게를 날려 버리겠다고 협박한다. 겁에 질리는 동시에 분노한 페피노는 탑을 기어올라 Pizzaface를 박살 내고 가게를 지키기로 결심한다.

세계관은 진지함과는 거리가 멀다. 탑의 각 층은 묘지(시체를 서핑보드처럼 타고 미끄러지는 구간), 《Five Nights at Freddy's》를 오마주한 점프스케어 레벨, 우주·공장·서부극 등 제각각 기괴한 테마로 구성되어 있다. 한마디로 1990년대 카툰 한 편을 통째로 플레이하는 듯한 난장판 세계다.

### 줄거리 (스포일러 포함)

탑은 5개 층으로 이루어져 있고, 각 층은 4개의 레벨과 1명의 보스로 구성된다(총 20개 레벨). 페피노는 층을 오르며 거대 파프리카 **Pepperman**(페퍼맨), 치즈 카우보이 **The Vigilante**(자경단원), 그리고 페피노의 숙적이자 TV 스타인 **The Noise**(노이즈) 등을 차례로 격파한다.

**[스포일러]** 최종 보스에 도달하면 Pizzaface의 정체가 드러난다. Pizzaface의 체력을 모두 깎으면 그 껍데기가 열리며 변기에 앉아 신문을 읽던 진짜 흑막 **Pizzahead**(피자헤드)가 튀어나와 머리부터 바닥에 처박힌다. Pizzahead는 잠시 패배한 척하다가 멀쩡히 일어나 이전에 쓰러뜨린 보스들을 모두 불러들여 페피노를 비웃는다. 인내심이 한계에 다다른 페피노가 머리를 부여잡고 비명을 지르자, 그 기세에 The Vigilante·The Noise·가짜 페피노(Fake Peppino)가 화면 밖으로 날아가 버린다. 최종 결전 끝에 페피노는 Pizzahead를 하늘 높이 두들겨 패서 탑에 내리꽂는다. 그러나 엔딩 크레딧에서 Pizzahead는 만신창이가 된 채로도 여전히 살아 있으며, 크레딧 후 일러스트들에서 변장한 채 페피노 곁에 숨어 다음 기회를 노린다. 결말 직전, 페피노가 동료 **Gustavo**(구스타보)와 그가 타고 다니는 거대 쥐 **Brick**(브릭)에게 피자를 대접하며 우정을 다지는 장면이 게임을 마무리한다.

### 캐릭터

- **Peppino Spaghetti** — 주인공. 신경질적이고 늘 땀에 절어 비명을 지르는 이탈리아 셰프. 무브셋은 《Wario Land 4》의 와리오에서 영감을 받았고, 애니메이션 작업 편의를 위해 검은 바지를 입혀 다리 동작을 단순화했다(McPig의 의도적 디자인).
- **Pizzaface / Pizzahead** — 최종 보스. 떠다니는 피자의 외형(Pizzaface)과 그 속의 진짜 본체(Pizzahead)로 나뉜다.
- **The Noise** — 페피노의 숙적이자 TV 스타. 도미노 피자의 광고 마스코트 "The Noid"의 패러디. 팬덤에서 가장 인기 있는 캐릭터 중 하나이며, 후일 무료 업데이트로 플레이어블 캐릭터가 되었다.
- **Gustavo & Brick** — 페피노의 조력자. 작은 인간 Gustavo가 거대 쥐 Brick에 올라타 함께 다니며, 일부 구간에서 플레이어블로 등장한다.
- **Pepperman, The Vigilante** 등 — 각 층의 개성 강한 보스들.

### 무드·톤·아트 디렉션

《Pizza Tower》의 시각은 1990년대 닉툰(Nicktoons)과 카툰 네트워크 작품들 — 《Ren & Stimpy》, 《Rocko's Modern Life》, 《Cow and Chicken》, 《CatDog》, 《Courage the Cowardly Dog》, 《Ed, Edd n Eddy》, 《SpongeBob SquarePants》 — 그리고 프랑스 만화(《Le Concombre Masqué》 등)에서 강하게 영향받은 과장된 "데인지드 애니메이션(Deranged Animation)" 스타일이다. 고해상도 픽셀아트와 거친 손그림이 섞여 마치 MS 페인트로 그린 듯한 의도적인 저예산 질감을 낸다. IGN은 이 "의도적 저예산 예술 스타일"이 게임에 강렬한(striking) 외형을 부여한다고 평했다. 페피노의 풍부한 표정 연기 덕분에 대사 한 줄 없이도 완성된 캐릭터로 느껴진다는 평이 많았다.

### 사운드·음악

사운드트랙은 게임의 정체성에서 결정적인 비중을 차지한다. **Mr. Sauceman**(Ronan de Castel)에게 이 작업은 첫 공식 발표작이었다. 그는 작곡을 취미로만 해 왔고 자신감 부족으로 곡을 공개한 적이 없었는데, 트위터의 게임플레이 영상에 매료되어 데모 트랙을 만들어 McPig에게 이메일로 보냈다. McPig이 그 트랙에 반해 곧장 합류를 제안했다. **ClascyJitto**는 당시 고등학생으로, Discord 서버에서 de Castel 곡의 리믹스를 공유하다 발탁되었다. PC Gamer는 "취미에 불과했던 작곡가가 그해 최고의 사운드트랙 중 하나를 공동 제작했다"는 제목으로 이들을 조명했다.

음악 스타일은 16비트 시대의 전자음원과 펑크·하우스·힙합 샘플링을 결합한 것으로, de Castel은 Chick Corea, Daft Punk, Mr. Oizo, Justice 등을, 게임적 영감으로는 《Sonic CD》와 《Wario Land》(특히 4편)를 꼽았다. 대표곡 "It's Pizza Time!"은 레벨 후반 탈출 시퀀스를 점점 고조시키는 에스컬레이션 테마로, 게임을 상징하는 곡이 되었다. 공식 사운드트랙은 사용 곡 73곡과 미사용 곡 39곡을 포함하며 2023년 2월 1일 Bandcamp, Steam, SoundCloud로 발매되었고, 이후 Materia Collective를 통해 LP 바이닐로도 출시되었다.

---

## 3. 핵심 시스템 / 메카닉

《Pizza Tower》의 본질은 "속도를 잃지 않는 흐름의 쾌감"이다. 표면적으로는 와리오 랜드를 닮았지만, 실제 손맛은 《Sonic the Hedgehog》의 질주감과 격투 게임식 콤보 유지를 한데 섞은 것에 가깝다.

### 코어 게임플레이 루프

플레이어는 각 레벨을 빠르게 돌파하며 (1) 적을 처치해 콤보를 쌓고 (2) 토핑·보물·비밀을 수집하고 (3) 레벨 끝에서 탈출 시퀀스를 발동해 제한 시간 안에 입구로 되돌아온다. 죽음이나 생명 시스템이 없으며(보스전 제외), 장애물에 부딪히면 체력이 깎이는 대신 점수가 줄고 콤보 타이머가 2초 깎인다. 즉 패널티는 "죽음"이 아니라 "점수와 흐름의 손실"이다.

### Mach Run(마하 런) 시스템

페피노의 질주는 4단계로 가속하는 **Mach Run**으로 구현된다. 달리기 입력을 유지하면 속도가 Mach 1에서 Mach 4까지 점진적으로 올라가며, 충돌 없이 공간을 누비거나 코너에서 드리프트해 속도를 보존하는 것이 핵심이다.

- **Mach 1** — 부서지는 블록(Breakable Block)을 파괴하고, 무기를 들지 않은 적을 들이받아 기절시킬 수 있다.
- **Mach 2** — 방향 전환 시 드리프트로 속도를 유지한다. 이 상태에서 점프하면 속도를 그대로 살리는 롱 점프가 나간다.
- **Mach 3** — 금속 블록(Metal Block)까지 파괴하고, 접촉만으로 적을 처치한다. 이 단계 이상에서는 무한 상승하는 슈퍼 점프도 가능하다.
- **Mach 4** — Mach 3와 기능은 같으나 더 빠르고 애니메이션이 다르다.

여기에 **Grab Dash**(잡아 돌진), **Ground Pound**(내려찍기), **벽 타기**(대시 중 벽 접촉 시) 등이 더해진다. 개발자 Sertif가 강조한 핵심은 "상태 간 연결"이다. 예를 들어 경사면에서 Ground Pound를 하면 Mach Dash로 이어지고, 슈퍼 점프를 취소하면 다시 Mach Dash로 돌아간다. 이렇게 각 동작이 서로를 끊김 없이 잇도록 설계된 덕에, 숙련자는 한 레벨을 단 한 번도 멈추지 않고 흘러가듯 주파할 수 있다.

### 콤보 시스템

콤보는 적을 처치할 때마다 1씩 증가하며, 추가 점수와 P-랭크 획득의 핵심이다. 콤보를 유지하려면 일정 시간(약 7초) 안에 다음 적을 처치하거나 아이템을 수집해야 한다. 콤보가 10에 도달하면 화면 내 모든 적을 쓸어버리는 **슈퍼 도발(Super Taunt)**을 쓸 수 있는데, 한 번 쓰면 다시 콤보 10(또는 현재보다 10 높은 수치)에 도달해야 재사용할 수 있다.

### 진행 구조

탑은 5개 층, 층당 4개 레벨 + 1명의 보스로 구성되어 총 20개의 사이드스크롤 레벨이 있다. 각 레벨은 묘지·공장·서부·우주 등 고유 테마와 그에 맞는 전용 기믹(예: 시체 서핑, 점프스케어)을 갖는다. 진척의 허브는 탑 내부를 직접 걸어 다니는 로비 형태다.

### Pizza Time(탈출 시퀀스)과 Lap 2

레벨 후반의 핵심 기둥 **Pillar John**을 파괴하면 "**Pizza Time**" 탈출 시퀀스가 발동한다. 탑이 무너지기 시작하고 화면 우측에서 Pizzaface가 추격해 오는 가운데, 플레이어는 제한 시간 내에 레벨 입구로 되돌아가야 한다. 탈출 경로 초반에 **Pizza Portal**이 활성화되는데, 이곳에 진입하면 "**Lap 2**"가 발동해 타이머가 리셋되고 Pillar John 방으로 다시 돌아가 두 번째 주행을 하게 된다. Lap 2 진입만으로 3,000점이 주어지며, 까다로운 레벨에서 S-랭크에 필요한 점수를 확보하는 핵심 수단이다.

### 자원·진척도·랭크 시스템

레벨 내에는 의식을 가진 다섯 가지 재료 **Toppins**(버섯·치즈·토마토·소시지·파인애플)가 흩어져 있어 점수와 돈을 준다. 다섯 개를 모두 모으면 추가 5,000점을 받는다. 최종 목표는 등급 시스템의 정점인 **P-랭크(Perfect Rank)**다. P-랭크를 얻으려면 다음을 모두 충족해야 한다.

1. S-랭크에 필요한 충분한 점수 획득
2. 비밀의 눈(Secret Eyes) 3개 발견
3. 탑 비밀 보물(Tower Secret Treasure) 수집
4. 레벨 첫 방부터 최종 출구까지 **단 한 번도 끊기지 않는 콤보** 유지
5. Pizza Portal에 진입해 **Lap 2 완주**

이처럼 P-랭크는 단순한 "클리어"가 아니라 레벨 레이아웃을 완전히 암기하고 경로를 최적화해야만 도달하는 숙련의 증표다.

### 멀티/협력 시스템

기본 게임은 싱글플레이지만, 후술할 The Noise 업데이트에서 The Noise로 게임을 완주하면 이스터에그로 2인 **Swap Mode**(플레이어 간 조작권을 교대하는 협력 모드)가 해금된다.

### 라이브 운영 / MTX

《Pizza Tower》는 시즌 패스나 MTX(소액 결제)가 전혀 없는 완전 패키지 게임이다. 출시 후 추가 콘텐츠는 모두 무료 업데이트로 제공되었으며, 그중 핵심이 The Noise 업데이트다.

### 난이도·접근성 / UI·UX 철학

이 게임에는 전통적인 난이도 선택지가 없다. 대신 "각 플레이어가 자신이 원하는 목표를 직접 고른다"는 접근을 택했다. 그냥 끝까지 가기만 하면 누구나 클리어할 수 있지만, 점수·콤보·P-랭크라는 자발적 도전이 무한한 깊이를 제공한다. Polygon은 이를 두고 "전통적 난이도 단계 대신 플레이어가 원하는 것을 직접 성취하도록 한 우아한 난이도 설계"라고 평했다. 개발자 스스로도 "선택하기 어렵고, 설명하기 어렵고, 숙달하기 어려운 게임을 만들고 있으므로, 실패의 부담(stakes)을 낮춰 플레이어가 자기 속도대로 게임을 즐기게 했다"고 밝혔다. 죽음이 없는 설계에 대해서는 "밸런스를 잘 못 맞춰서 죽는 기능을 빼버렸다"고 농담하기도 했다.

---

## 4. 평가

### 평론 점수

| 매체 | 점수 | 핵심 평가 |
|------|------|-----------|
| Metacritic(PC) | 89/100 | "전반적으로 호평(generally favorable)" |
| OpenCritic | "Mighty" (약 91, 추천율 100%) | 최상위 등급 |
| PC Gamer (US) | 90/100 | "영감이 된 《Wario Land》를 제대로 계승할 뿐 아니라 능가한다" |
| IGN | 9/10 | "영감을 초월해 더 위대한 무언가가 된 매우 특별한 2D 플랫포머" |
| Nintendo Life | 9/10 | "영감이 된 작품을 거의 모든 면에서 개선한 보기 드문 게임" |
| Polygon | 추천 | "《Wario Land》의 기묘한 틈새를 날카롭게 다듬고, 진화시켜 거의 완성했다" |
| MeriStation | 9/10 | "즉각적인 클래식이자 인디 사이드스크롤 씬에 부는 신선한 바람" |
| Multiplayer.it | 8/10 | "펑크와 메탈을 결합하며 1990년대 플랫포머 스타일을 유지" |

PC Gamer의 결론 인용이 특히 회자되었다: "Pizza Tower is an unashamed ode to Wario Land—but in my eyes it has eclipsed it."(《Pizza Tower》는 《Wario Land》에 바치는 거리낌 없는 헌사지만, 내 눈에는 그것을 능가했다.) 평론가들은 공통적으로 이 게임의 완성도에 "놀랐다"고 표현했으며, 닌텐도가 부활시킬지 모를 《Wario Land》 신작이 이만큼 활기차고 독창적일 수 있을지 의문이라는 식의 찬사를 보냈다.

### 수상 이력

| 연도 | 시상식 | 부문 | 결과 |
|------|--------|------|------|
| 2023 | Golden Joystick Awards | Best Indie Game | 노미네이트 |
| 2023 | The Game Awards | Best Debut Indie Game | 노미네이트 |
| 2023 | Steam Awards | Best Soundtrack | 노미네이트 |
| 2024 | New York Game Awards | Off Broadway Award for Best Indie Game | 노미네이트 |
| 2024 | Game Developers Choice Awards (24회) | Best Debut | 노미네이트 |

The Game Awards 2023의 Best Debut Indie Game 부문 후보 명단은 Cocoon, Dredge, Pizza Tower, Venba, Viewfinder였다. TheGamer의 Stacey Henley는 《Pizza Tower》가 Best Debut Indie Game에는 올랐으나 더 넓은 Best Independent Game 부문에는 빠진 것을 "어울리지 않는다(incongruous)"고 지적했다.

### 상업 지표

- **초반 판매.** 출시 첫 달에 약 10만 장이 팔렸고 매출은 약 300만 달러에 달했다(GameSensor 보도 기준).
- **누적 추정치.** Steam 매출 분석 사이트(Gamalytic 등) 추정에 따르면 출시 이후 누적 총매출 약 7,240만 달러, 개발자 순수익 약 2,140만 달러로 집계된다. Steam 보유자는 약 100만~200만 명으로 추정된다(SteamSpy 등 제3자 추정치, 공식 수치 아님).
- **동시 접속.** Steam 동시 접속 역대 최고치는 2024년 3월 12일(The Noise 업데이트 출시일)에 기록한 9,074명이다.

### 유저 평가

Steam에서 《Pizza Tower》는 출시 하루 만에 2023년 최고 평가 게임 중 하나로 올라섰다. 2024년 8월 기준으로는 Steam에서 가장 높은 평가를 받은 2D 플랫포머로, 《Super Meat Boy》(2010), 《Celeste》(2018), 《Katana Zero》(2019)를 앞섰다. 출시 전부터 형성된 강력한 팬덤(Discord 서버 멤버가 출시 후 5,000명에서 20,000명으로 급증)이 유저 평가의 든든한 기반이 되었다.

### 평론-유저 괴리

이 게임은 평론과 유저 평가 사이의 괴리가 거의 없는, 보기 드물게 양쪽 모두에서 압도적 호평을 받은 사례다. 다만 조작 정밀도에 대한 호불호는 코어 유저층 내부에서 갈렸다(아래 6장 참고).

---

## 5. 성공 요인 분석

### 디자인 측면

가장 큰 성공 요인은 "닌텐도가 비워 둔 자리를 정확히 겨냥"한 것이다. 《Wario Land》 시리즈는 2008년 《Wario Land: Shake It!》 이후 사실상 휴면 상태였고, 그 특유의 "변신·파괴·탐색"형 플랫포밍을 그리워하던 코어 팬층이 두텁게 존재했다. 《Pizza Tower》는 이 공식을 그대로 모방하는 데 그치지 않고, 죽음을 없애고 속도·콤보·스코어 어택을 전면에 내세워 "흐름을 끊지 않는 쾌감"이라는 새로운 정체성으로 진화시켰다. 무브셋의 각 상태를 끊김 없이 연결한 설계, 그리고 P-랭크라는 무한 숙련 목표가 리플레이성을 극대화했다.

### 개발 방법론 — "Speedy Implementation"

Game Developer 인터뷰에서 Sertif가 밝힌 개발 방식은 "빠른 구현·빠른 폐기" 사이클이었다. "메카닉을 떠올리면 정착시킨 뒤 내가 프로토타이핑과 테스트를 시작하고, 그 사이 McPig이 Aseprite로 애니메이션을 만든다. 끝나면 평가하고 같은 과정을 반복했다." 그 결과 "수많은 메카닉과 스프라이트가 버려졌지만, 그것이 이 게임에 최선이었다"고 그는 말했다. 빠른 애니메이터와 빠른 코더가 짝을 이뤄, 더 큰 팀이라면 시도조차 못 했을 양의 실험을 거친 셈이다. 각 레벨은 "변화하는 속도 중심 철학을 수용하기 위해" 최근 3년간 평균 2~3회씩 리메이크되었다.

### 마케팅·출시 전략 — 데모와 커뮤니티

별도의 대형 마케팅 예산 없이, 출시까지 5년에 걸친 공개·비공개 데모와 Patreon 얼리 액세스가 곧 마케팅이었다. 특히 2019년 SAGE(Sonic Amateur Game Expo)에서 공개한 데모가 큰 주목을 받으며 인지도가 급상승했다. 개발자들은 트위터에 스크린샷을 올리고 Discord를 운영하며 팬덤을 직접 키웠다. Sertif는 거대 팬덤의 형성을 "데모, Patreon 빌드, 그리고 Vinesauce(Vinny) 같은 스트리머의 방송" 덕분이라고 명시했다.

### 플레이어 관찰을 통한 방향 전환

2019년 데모에서 "더 자유로운 무브셋"을 실험한 결과, 플레이어들이 속도를 추구하는 방식을 관찰한 개발자들은 게임의 무게중심을 속도와 스코어 어택으로 옮겼다. 초기에는 의도치 않은 플레이를 막으려 여러 제한을 넣었지만 "재미가 없어서" 자유로운 무브셋으로 회귀한 것이 결정적이었다.

### 타이밍과 시장 환경

2023년 초는 인디 플랫포머에 우호적인 시기였다. 《Celeste》, 《Hollow Knight》 등으로 다져진 인디 플랫포머 시장의 기대치가 높았고, "20달러에 압도적 가성비"라는 평가가 입소문을 타기 좋은 환경이었다. 강렬한 비주얼과 음악은 트위치·유튜브 클립으로 퍼지기에 최적화되어 있었다.

### 커뮤니티·IP 효과

The Noise(도미노 The Noid 패러디)를 비롯한 캐릭터들이 밈으로 폭발했다. 출시 직후 "Lario" 밈이 유튜브·트위터에서 유행했고, Pizzahead와 그의 테마곡을 둘러싼 농담이 끊임없이 재생산되었다. 데인지드 애니메이션풍 비주얼은 그 자체로 "밈의 분수"가 되었다. Tour De Pizza는 Fangamer와 협력해 봉제인형·티셔츠·핀 등 상품을 출시하며 IP 가치를 확장했다.

### 동시기 작품 대비 차별점

같은 시기 인디 명작들(《Sea of Stars》, 《Dave the Diver》, 《Cocoon》, 《Dredge》 등)이 대체로 신중하고 정제된 톤이었던 데 반해, 《Pizza Tower》는 "광기·속도·소음"이라는 정반대 노선으로 확실한 차별화를 이뤘다. 점잖은 인디 씬에서 가장 시끄럽고 빠른 게임이라는 위치 선정이 강한 인상을 남겼다.

---

## 6. 비평적 시각 / 한계 / 논란

압도적 호평 속에서도 몇 가지 한계가 지적되었다.

### 디자인적 약점

- **조작 정밀도의 진입장벽.** Rock Paper Shotgun과 Multiplayer.it은 페피노를 능숙하게 다루기까지 상당한 정밀도가 요구된다는 점을 지적했다. RPS는 이를 게임의 "가장 큰 불만"으로 꼽으며, 와리오 랜드식으로 느리고 신중하게 설계된 레벨 구조와 빠른 이동을 기대하는 게임의 요구 사이에서 반복적 좌절이 발생한다고 비판했다. 다만 일부 유저는 이런 "거친 모서리(rough edges)"를 게임 매력의 필수 요소로 받아들였다.
- **보스전의 무작위성.** Nintendo Life의 유일한 불만은 보스들이 무작위성에 의존해 다소 답답하다는 점이었다.

### 평가가 갈리는 지점

P-랭크 난이도는 코어 유저 사이에서 호불호가 갈린다. 커뮤니티 토론에서는 Pizzascare, Peppibot Factory, Gnome Forest, Bloodsauce Dungeon 등이 P-랭크 획득이 가장 어려운 레벨로 자주 거론되며, 일부 플레이어는 이를 "좌절스러울 만큼 어렵다"고 표현했다. 그러나 P-랭크는 어디까지나 자발적 도전이라는 점에서 주요 평론가들의 비판으로 이어지지는 않았다.

### 운영·논란 이슈

게임 자체를 둘러싼 큰 논란은 없었다. 익명 개발진 운영, 무료 업데이트 정책, MTX 부재 등 운영 측면은 오히려 모범 사례로 평가받는다. 다만 출시 후 한때 활발하던 공식 Discord 서버를 McPig과 Sertif가 폐쇄한 것, 그리고 물리 에디션(특히 Collector's Edition)이 미국 관세 이슈 등으로 출시가 지연된 점이 팬덤 내에서 아쉬움으로 거론되었다.

---

## 7. 영향과 유산

### 장르에 미친 영향

《Pizza Tower》는 휴면 상태였던 《Wario Land》식 플랫포밍의 정신적 후계자로 확고히 자리매김했다. 동시에 "죽음 없는 스코어 어택 + 흐름 기반 속도감"이라는 조합을 현대 2D 플랫포머의 유효한 설계 언어로 재증명했다. 출시 이후 등장한 여러 고속 플랫포머가 《Pizza Tower》와 비교되었으며, GamesRadar는 닌텐도 인디 쇼케이스에 등장한 한 신작이 "Pizza Tower 클론"이라 불렸으나 실제로는 둘 다 2001년 《Wario Land 4》라는 같은 뿌리에서 나왔다고 정리했다. 이는 《Pizza Tower》가 이 장르의 현대적 기준점이 되었음을 방증한다.

### 후속 콘텐츠와 확장

- **The Noise 업데이트 (2024년 3월 12일, v1.1.0).** 악역 The Noise를 플레이어블 캐릭터로 추가한 대형 무료 업데이트. 스케이트보드·제트팩 중심의 독자적 무브셋, 일부 레벨·보스의 변형, UI·음악 변경을 포함하며, 사실상 New Game Plus로 설계되었다. PC Gamer는 이를 "일종의 뉴 게임 플러스로 생각하라"는 개발자 표현과 함께 소개했다. 이 업데이트로 Steam 동시 접속이 9,000명을 넘으며 역대 최고치를 경신했다.
- **Nintendo Switch 이식.** 2024년 8월 27일 Nintendo Indie World 및 Partner Showcase에서 발표·출시되어 콘솔 유저층으로 확장되었다.
- **물리 에디션.** Fangamer가 표준판과 수집가판(Peppino 계란 타이머, 아트북, 미술 카드 등 포함)을 준비했으며, 일부는 관세 이슈로 일정이 조정되어 2025년에 출시되었다.

### 산업적 의미

두 명 규모의 익명 개발팀이 Patreon 후원과 데모 중심 커뮤니티 빌딩만으로 5년을 버텨, 추정 누적 매출 수천만 달러 규모의 성공을 거둔 사례다. 대형 퍼블리셔나 마케팅 예산 없이 "데모를 통한 직접 검증"과 "스트리머 바이럴"만으로 성공할 수 있음을 보여준 현대 인디 성공 방정식의 교과서적 예시다.

### 문화적 의미

데인지드 애니메이션 미학과 강렬한 사운드트랙은 게임 밖에서 독립적인 밈·팬아트·팬게임 생태계를 형성했다. The Noise, Pizzahead, 페피노의 비명 등은 게임을 플레이하지 않은 사람도 아는 인터넷 문화 아이콘이 되었다. 사운드트랙은 Materia Collective를 통해 바이럴리 LP로 발매되며 게임 음악으로서의 수명을 게임 본편 너머로 확장했다.

---

## 8. 부록

### 개발자 자료·인터뷰

- Game Developer — "How speedy implementation fed the fast-paced platforming of Pizza Tower" (Sertif·McPig의 개발 방법론 인터뷰)
  https://www.gamedeveloper.com/design/how-speedy-implementation-high-paced-platformer-pizza-tower
- PC Gamer — "Despite music being just 'a hobby' this composer co-created one of the year's best soundtracks" (Mr. Sauceman 인터뷰)
  https://www.pcgamer.com/despite-music-being-just-a-hobby-this-composer-co-created-one-of-the-years-best-soundtracks/

### 주요 리뷰·인터뷰

- PC Gamer 리뷰 (90/100): https://www.pcgamer.com/pizza-tower-review-madcap-platforming-at-100mph/
- Nintendo Life 리뷰 (9/10): https://www.nintendolife.com/reviews/switch-eshop/pizza-tower
- Gaming Reinvented — McPig 인터뷰: https://gamingreinvented.com/interview/an-interview-with-the-developer-of-wario-land-successor-pizza-tower/

### 핵심 통계 표

| 지표 | 수치 | 출처 |
|------|------|------|
| 출시일(PC) | 2023년 1월 26일 | Wikipedia |
| 출시일(Switch) | 2024년 8월 27일 | Wikipedia |
| 개발 기간 | 약 5년 (2018~2023) | Wikipedia / Game Developer |
| 레벨 수 | 20개 (5층 × 4레벨 + 보스) | Pizza Tower Wiki |
| Metacritic(PC) | 89/100 | Metacritic |
| OpenCritic | "Mighty" | OpenCritic |
| 첫 달 판매 | 약 10만 장 / 약 300만 달러 | GameSensor |
| 누적 매출(추정) | 약 7,240만 달러 (순수익 약 2,140만 달러) | Gamalytic 추정 |
| Steam 보유자(추정) | 약 100만~200만 명 | SteamSpy 등 추정 |
| Steam 동시 접속 최고 | 9,074명 (2024-03-12) | SteamDB |
| 사운드트랙 곡 수 | 사용 73곡 + 미사용 39곡 | Pizza Tower Wiki |
| 가격 | 약 19.99달러 | PC Gamer |

### 참고 자료 목록 (영어권 매체 중심)

- Wikipedia — Pizza Tower: https://en.wikipedia.org/wiki/Pizza_Tower
- Metacritic — Pizza Tower: https://www.metacritic.com/game/pizza-tower/
- OpenCritic — Pizza Tower: https://opencritic.com/game/14233/pizza-tower
- Game Developer (Sertif 인터뷰): https://www.gamedeveloper.com/design/how-speedy-implementation-high-paced-platformer-pizza-tower
- PC Gamer (리뷰 / 사운드트랙 인터뷰 / The Noise 업데이트 기사)
- Nintendo Life (Switch 리뷰): https://www.nintendolife.com/reviews/switch-eshop/pizza-tower
- GamesRadar — Golden Joystick 2023 후보 / "Pizza Tower 클론" 분석
- The Game Awards 2023 (Wikipedia): https://en.wikipedia.org/wiki/The_Game_Awards_2023
- Know Your Meme — Pizza Tower: https://knowyourmeme.com/memes/subcultures/pizza-tower
- Pizza Tower Wiki — Ranks, Soundtrack, The Noise Update, SAGE 2019 Demo: https://pizzatower.wiki/
- Mr. Sauceman Bandcamp (사운드트랙): https://ronandecastel.bandcamp.com/album/pizza-tower-soundtrack
- SteamDB — Pizza Tower: https://steamdb.info/app/2231450/
- GameSensor (판매 보도): https://gamesensor.info/news/pizza_tower

---

*본 분석서는 2026년 5월 기준 영어권 공개 자료를 바탕으로 작성되었다. 판매량·매출의 일부 수치는 제3자 추정치이며 개발사 공식 발표가 아님을 명시한다.*
