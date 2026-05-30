# 《THE FINALS》 (2023) 심층 분석 — 무너지는 도시를 무대로 한 게임쇼, 그리고 파괴의 재발명

> 무료 팀 기반 1인칭 슈터. Embark Studios 개발/퍼블리싱(모회사 Nexon). 디렉터 Gustav Tilleby. Unreal Engine 5 기반. PC·Xbox Series X|S·PS5로 2023년 12월 7일 The Game Awards에서 깜짝 출시. Metacritic(PC) 80, OpenCritic 85, 피크 동접 242,619명(2023.12.10, Steam 기준).

---

## 1. 게임 개요

《THE FINALS》는 스웨덴 스톡홀름의 **Embark Studios**가 개발하고 자체 퍼블리싱한 무료(free-to-play) 팀 기반 1인칭 슈터다. 게임의 정체성을 한 문장으로 압축하면 "**완전히 부서지는 도시를 무대로 펼쳐지는 가상 VR 게임쇼**"다. 2023년 12월 7일 The Game Awards 시상식 도중, 트레일러 공개와 동시에 PC(Steam)·Xbox Series X|S·PlayStation 5에서 곧바로 플레이 가능한 형태로 **셰도우 드롭(shadow drop, 깜짝 출시)** 되었다. 이는 출시 마케팅의 정석을 거스르는 선택이었지만, 결과적으로 시상식 직후의 화제성을 그대로 동접으로 전환시키는 데 성공했다. 이후 PlayStation 4 버전이 2024년 12월 12일 추가되었고(다만 PS4 서비스는 2026년 3월 18일 종료 예정), 중국판은 2025년 11월 18일 Tencent와의 파트너십으로 출시되었다.

개발사 Embark Studios의 혈통은 이 게임을 이해하는 핵심 열쇠다. Embark는 2018년, EA의 글로벌 스튜디오 총괄(EVP)이자 《Battlefield》 개발사 DICE의 전 CEO였던 **Patrick Söderlund**이 EA를 떠난 직후 설립했다. 창업 멤버에는 Magnus Nordin, Rob Runesson, Stefan Strandberg, Jenny Huldschiner, 그리고 렌더링·엔진 분야의 베테랑 Johan Andersson 등 다수의 전(前) DICE·《Battlefield》 출신 인력이 포진했다. 즉 《THE FINALS》는 "**《Battlefield》의 환경 파괴 DNA를 계승한 인력이, 그 파괴를 게임의 부수 효과가 아니라 게임의 본질로 끌어올린 작품**"이라는 계보 안에 놓인다. 2021년 한국의 **Nexon**이 Embark를 인수해 자회사로 편입했고, 《THE FINALS》는 Nexon 산하에서 만들어진 대표적 서구권 타이틀이 되었다.

디렉터는 **Gustav Tilleby**가 맡았다. 엔진은 **Unreal Engine 5**를 채택하되, Embark가 자체적으로 대규모 개조를 가했다. 특히 후술할 **서버사이드 파괴/물리 시스템**은 상용 엔진의 기본 기능이 아니라 Embark가 백엔드에 직접 구축한 기술로, 이 스튜디오가 스스로를 "**기술 우선 스튜디오(technology-first studio)**"로 규정하는 근거다(Naavik 분석). 개발 규모와 정확한 예산은 비공개지만, Nexon의 투자와 다수의 시니어 출신 인력 구성으로 미루어 상당한 자본·인력이 투입된 프로젝트로 볼 수 있다.

| 항목 | 내용 |
| --- | --- |
| 개발/퍼블리셔 | Embark Studios (스톡홀름) |
| 모회사 | Nexon (2021년 인수) |
| 디렉터 | Gustav Tilleby |
| 주요 창업자 | Patrick Söderlund(CEO), Magnus Nordin, Johan Andersson 등 ex-DICE |
| 엔진 | Unreal Engine 5 (Embark 자체 개조 + 서버사이드 파괴) |
| 장르 | F2P 팀 기반 FPS, 환경 파괴 중심 |
| 출시 | 2023.12.7 (PC/Xbox Series/PS5, TGA 셰도우 드롭) |
| 플랫폼 추가 | PS4 2024.12.12 / 중국판 2025.11.18 |

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 컨셉과 세계관

《THE FINALS》의 무대는 2100년경의 가까운 미래, **"THE FINALS"라는 이름의 가상현실(VR) 전투 게임쇼**다. 플레이어는 실제 사람이 아니라, 이 게임쇼에 출전하는 "컨테스턴트(Contestant)" — 즉 디지털로 백업·복제된 아바타를 조종한다. 이 설정은 게임 디자인에 우아한 알리바이를 제공한다. 도시 한 블록을 통째로 무너뜨려도, 동료가 폭사한 뒤 부활 동상에서 되살아나도, 그것은 어디까지나 "쇼를 위한 가상 무대"이기 때문에 톤이 가볍고 폭력의 무게가 없다. 화려한 색감, 관중의 환호, 스폰서 로고, 그리고 끊임없이 떠드는 **AI 해설진**이 모든 경기를 실시간 중계 예능처럼 포장한다.

이 "게임쇼" 프레이밍은 단순한 분위기 장치가 아니라 게임의 거의 모든 UI/연출을 관통하는 일관된 디렉션이다. 라운드 시작 시 무대가 솟아오르고, 캐시아웃이 성공하면 지폐가 분수처럼 쏟아지며, 해설자는 "관중이 이 장면을 사랑합니다!" 식의 멘트를 던진다. 톤은 시종일관 밝고 과장돼 있어, 같은 시기의 어둡고 무거운 라이브 서비스 슈터들과 명확히 차별화된다.

### 무드·아트 디렉션

비주얼은 깨끗하고 채도 높은 현대 도시(서울에서 영감 받은 SYS$HORIZON 등 다양한 아레나)와, 그 위에 덧씌워진 방송 그래픽이 충돌하는 구조다. 핵심 미감은 "**질서정연한 도시가 매 순간 카오스로 붕괴해가는 과정**" 그 자체에 있다. 유리가 산산조각 나고, 콘크리트가 분진을 일으키며 무너지고, 가구·드럼통 같은 소품이 물리적으로 굴러다닌다. 시각적 쾌감의 상당 부분이 "부수는 행위"의 즉물적 피드백에서 나온다.

### 사운드와 AI 음성 논란

사운드 디자인에서 《THE FINALS》는 게임 산업의 중요한 분기점에 섰다. **모든 컨테스턴트의 보이스 바크와 해설진 대사를 AI text-to-speech(ElevenLabs 기반)로 생성**했기 때문이다. 이는 2023년 10월 오픈 베타 중 오디오 디자이너의 언급으로 드러나 큰 논란이 됐다(자세한 내용은 6장). 음악·효과음 자체는 게임쇼의 들뜬 분위기에 맞춰 경쾌하게 설계됐으나, "목소리"라는 게임의 핵심 정서 전달 채널을 AI에 맡긴 결정은 작품의 예술적 정체성을 둘러싼 가장 큰 쟁점이 되었다.

---

## 3. 핵심 시스템 / 메카닉 — 가장 자세하게

### 3-1. 코어 루프: Cashout

《THE FINALS》의 심장은 **Cashout(캐시아웃)** 이라는 목표 기반 메카닉이다. 전형적인 진행은 다음과 같다.

1. 보통 **세 팀**(팀당 보통 3인)이 동시에 한 아레나에 투입된다.
2. 맵 곳곳에 **금고(Vault)** 가 스폰된다. 팀은 금고를 열어 현금을 꺼내고, 그것을 들고 **Cashout Station(입금기)** 까지 운반해 투입한다.
3. 금고를 입금기에 꽂는 순간 타이머가 시작되고, **즉시 전체 금액의 20%가 적립**된다. 타이머가 끝까지 돌아가면 나머지 80%가 적립된다.
4. 결정적 디자인: **다른 팀이 진행 중인 입금을 탈취할 수 있고, 이때 카운트다운 진행도가 리셋되지 않는다.** 즉 90%까지 채워진 입금기를 막판에 뺏으면, 그 90% 진행분을 그대로 이어받아 가로챌 수 있다.

이 한 줄짜리 규칙이 만들어내는 긴장은 엄청나다. 입금기를 처음 가동한 팀은 "지키는 자"가 되고, 나머지 두 팀은 "빼앗는 자"가 되어 자연스럽게 3파전 교전이 한 지점으로 수렴한다. 끝까지 방어할지, 일부러 막판에 난입할지, 두 적팀이 서로 싸우게 둘지 — 매 라운드 전략이 달라진다. "두 라운드도 같은 적이 없다(no two rounds play the same)"는 마케팅 카피는 이 구조와 파괴 시스템의 결합에서 나온다.

### 3-2. 세 가지 클래스(Contestant)

플레이어는 매치 전 **Light / Medium / Heavy** 세 체급 중 하나를 고른다. 체급은 캐릭터의 외형 크기, 이동 속도, 체력을 동시에 규정하는 직관적 삼각 구도다.

| 클래스 | 체력 | 특성 | 대표 전문화 | 대표 무기 | 대표 가젯 |
| --- | --- | --- | --- | --- | --- |
| Light | 150 HP | 가장 빠르고 가장 작다 | Grappling Hook(그래플 훅) | Sword, SH1900(소드오프 샷건), SR-84(스나이퍼) | Smoke·Glitch Grenade |
| Medium | 250 HP | 균형형, 전형적 보병 | Healing Beam(힐 빔) | R.357, Model 1887 | Zipline, Explosive Mine, Goo Grenade, Defibrillator |
| Heavy | 350 HP | 가장 느리고 가장 크다 | Charge 'n Slam(돌진 강타) | Lewis Gun, Sledgehammer | Pyro Mine, Barricade |

- **Light**는 그래플 훅으로 건물 사이를 날아다니며 측면을 치고 빠지는 암살자형이다. 체력이 낮아 한 번의 실수가 치명적이다.
- **Medium**은 **Healing Beam**으로 팀을 유지시키고, **Defibrillator로 약 3초 만에 동료를 부활**시킬 수 있어 사실상 팀의 중추다. Zipline·Goo Grenade로 즉석 지형(통로·벽)을 만드는 유틸리티도 강력하다.
- **Heavy**는 350 HP의 탱크로, Sledgehammer로 벽과 적을 동시에 부수고 Charge 'n Slam으로 돌진한다. 파괴 잠재력이 가장 커서, 후술하듯 경쟁 환경에서 과도하게 채택되는 밸런스 이슈를 낳았다.

부활 시스템도 독특하다. 쓰러진 동료는 작은 **부활 동상(revive statue)** 으로 변하고, 팀원이 **5초간 연속 상호작용**하면 되살아난다(Medium의 제세동기는 더 빠른 3초). 즉 "팀원을 살리려 위험 지역에 5초간 묶이는" 리스크-리워드가 모든 교전에 내장돼 있다.

### 3-3. 파괴 — 이 게임의 진짜 주인공

《THE FINALS》가 다른 슈터와 결정적으로 갈리는 지점이 **완전 파괴 가능 환경(fully destructible environment)** 이다. 벽에 구멍을 뚫어 새 사선을 열고, 다리를 끊어 적의 동선을 차단하며, **건물의 지지벽(load-bearing wall)을 집중 파괴해 건물 전체를 무너뜨리고**, 지붕을 뚫어 위에서 강하하는 식의 플레이가 가능하다. 파괴는 단순 연출이 아니라 전술의 1차 변수다. 입금기를 지키던 팀의 발밑 바닥을 통째로 날려버려 추락사시키거나, 막힌 벽을 뚫어 새 진입로를 만드는 식으로 맵 자체를 무기화한다.

기술적으로 가장 주목할 점은 **서버사이드 파괴/물리 연산**이다. 보통의 물리 파괴는 각 플레이어의 PC/콘솔에서 따로 계산돼 클라이언트마다 잔해가 다르게 보이기 쉽다. Embark는 **파괴와 물리 시뮬레이션을 자사 서버에서 처리**하도록 설계해, 모든 플레이어에게 동일한 잔해·붕괴 결과가 보이도록 했다(GamesBeat, Digital Trends 보도). 한 개발자는 경쟁사들이 이 기술을 보면 "패닉에 빠질 것(panic)"이라고 농담했을 정도다. Embark는 이 기술이 자매작 《Arc Raiders》에도 적용된다고 예고했다. 이 서버사이드 접근은 "결정론적이고 공정한 파괴"를 보장하는 대신 서버 부하라는 비용을 감수하는 선택이다.

여기에 날씨·시간대 변화, 화분·의자·드럼통 등 물리 상호작용 오브젝트가 더해져 아레나는 살아 있는 시스템처럼 작동한다.

### 3-4. 게임 모드와 진행 구조

- **캐주얼**: Quick Cash(3팀, 먼저 2회 캐시아웃 달성 시 승), Power Shift(5v5, 이동하는 플랫폼을 점령하는 킹 오브 더 힐), Team Deathmatch(5v5, $3,000=30킬 선취).
- **경쟁**: **Ranked Tournament**(Bronze~Diamond 랭크, 상위 500명에게 별도 **Ruby** 랭크 부여), **World Tour**(주간 로테이션 토너먼트, 리더보드 기반).
- **토너먼트 구조**: Quick Cash의 더 긴 변형으로, **동시에 두 경기가 진행**되고 각 경기 상위 팀이 녹아웃 라운드로 진출, 다시 상위 팀이 titular finals(결승)로 올라가 최종 우승을 가린다. 제한된 부활 수가 적용돼 후반으로 갈수록 긴장이 고조된다.
- **제거/한정 모드**: Bank It(4팀이 코인 수집, $40,000 적립 시 승), Terminal Attack(5v5 공격/수비, best-of-7), Head-2-Head 등.
- **이벤트 모드**: Steal The Spotlight, Smoking Guns, Bunny Bash, Heavy Hitters, Blast Off!, Super Cashball, Heaven or Else, Ghoul Rush 등 시즌·시기별 한정 모드.

### 3-5. 경제·라이브 운영·MTX

인게임 화폐는 두 축이다. **VR**(소프트 화폐, 보유 한도 5,000, 대부분 코스메틱 500 VR·시즌 아이템 약 2,200 VR)과 하드 화폐 **Multibucks**. 배틀패스는 **1,150 Multibucks**에 판매되며, 무과금 트랙은 레벨 91 도달 시 375 Multibucks를 돌려준다 — 즉 하드 화폐를 과금 없이 얻는 사실상 유일한 경로가 배틀패스라, 코스메틱 가격이 비싸다는 커뮤니티 불만으로 이어졌다.

라이브 운영은 **시즌제**다. 각 시즌마다 신규 맵·무기·가젯·전문화·배틀패스가 추가된다. 예를 들어 **시즌 2**(2024.3.14~6.13)는 해커 집단 CNS를 둘러싼 스토리와 레트로 게이밍 테마로, 신맵 SYS$HORIZON, Power Shift·Terminal Attack 모드, 무기 93R·FAMAS·KS-23, 가젯 Anti-Gravity Cube·Gateway·Data Reshaper, 전문화 Dematerializer를 도입했고 배틀패스는 12페이지 96보상으로 구성됐다. **시즌 6**(2025.3.20~6.11)은 Las Vegas Stadium 신맵, LARN-220·MCB-01 Repeater·HM134 Minigun 무기, Team Deathmatch 모드를 추가했다. 이후 시즌 9(Point Break 모드)·시즌 10까지 운영이 이어졌다.

### 3-6. UI/UX·접근성

UI는 게임쇼 방송 그래픽을 차용해, 입금 진행도·팀 순위·잔여 시간을 직관적 HUD로 보여준다. 풀 크로스플레이를 지원하며, Steam Deck/SteamOS도 (커널 레벨 안티치트 도입에도) 지원이 유지됐다. 다만 Xbox One은 하드웨어 한계로 미발매다.

---

## 4. 평가

### 평론

- **Metacritic(PC) 80점**, **OpenCritic 85점**으로 "전반적 호평" 구간에 안착했다.
- **IGN 8/10**: "팀 기반 PVP 슈터에 대한 신선하고 흥미로운 해석이며, 어떤 FPS와 견줘도 최고 수준의 환경 파괴를 담았다."
- **GameSpot 8/10**(2023.12.19, Eric Switzer): "탄탄한 사격에 역동적 파괴와 게임쇼 연출이 어우러져, 짜릿하게 혼란스러운 조합을 만들어낸다." 그래플 훅으로 전장을 날거나 헐크처럼 건물을 부수는 감각이 엄격한 목표 기반 모드와 섞이는 것을 "신선한 바람(a breath of fresh air)"으로 평했다.
- **Game Informer 9/10**: 출시 직후 가장 높은 점수대 중 하나로, 파괴와 모드 디자인을 높이 샀다.
- **Eurogamer 3/5**(Rick Lane): 가장 비판적이었다. "Embark의 멀티플레이어 슈터는 순간순간 눈부시지만, AI 음성은 더 폭넓은 예술적 비전의 부재를 드러내는 증상"이라며, 기술적 화려함과 정서적·작가적 깊이의 괴리를 지적했다.

### 수상

- **제27회 D.I.C.E. Awards**: Online Game of the Year, Outstanding Technical Achievement 부문 후보.
- **Steam Awards 2024**: "Best Game You Suck At(가장 못하게 되는 게임)" 후보 — 높은 진입 난도와 팬층의 애정을 동시에 보여주는 지명이다.

### 상업·플레이어 지표

플레이어 수치(이하 Steam/PC 기준, 콘솔 미포함)는 라이브 서비스 슈터의 전형적 "폭발 후 안정화" 곡선을 그렸다.

| 시점 | 지표 |
| --- | --- |
| 오픈 베타(2023.10.26~) | Steam 최다 플레이 상위 5위, 약 30만 동접 근접 (Game World Observer) |
| 2023.12.10 | **역대 피크 동접 242,619명** |
| 2023.12 월평균 | 약 120,211명 |
| 2024.1.7 | 마지막으로 동접 10만 돌파 |
| 2024.2 월평균 | 약 24,848명 |
| 2024.3 월평균 | 약 21,712명 (이후 월평균 2만 회복 못함) |
| 2025.2 | 월평균 11,760명, 피크 19,499명 (역대 피크 대비 약 95% 감소) |

다만 이 수치는 PC만 반영하며, 콘솔(PS5/PS4/Xbox) 플레이어와 무료 게임 특유의 유입·재유입을 포함하지 않는다. F2P 슈터로서 "출시 폭발 → 큰 이탈 → 코어 팬층 중심 안정 운영"이라는 궤적은 동시기 다수 작품과 유사하다.

### 유저 평가와 평론-유저 괴리

Steam 유저 평가는 대체로 긍정적이었으며, 특히 파괴 시스템과 그래플 훅 기동성은 호평이 일관됐다. 다만 ① AI 음성, ② 경쟁 모드의 클래스 밸런스(Heavy 편중), ③ 코스메틱 가격, ④ 안티치트/성능 이슈에서 불만이 누적됐다. 평론은 "기술적 성취"에 높은 점수를 줬고, 일부 유저·비평가(Eurogamer)는 "기술은 빛나지만 영혼·작가성에서 아쉽다"는 분리된 평가를 내렸다.

---

## 5. 성공 요인 분석 — 핵심

### 5-1. 디자인: "부수기"를 부수적 효과가 아닌 게임의 본질로

대다수 슈터에서 파괴는 양념이거나 일부 벽이 부서지는 한정 연출이다. 《THE FINALS》는 파괴를 **승패를 직접 결정하는 1차 변수**로 끌어올렸다. 입금기 아래 바닥을 날려 적팀을 추락시키거나, 막힌 동선을 폭파로 뚫는 행위가 사격만큼 중요해지자, 슈터에 익숙한 플레이어조차 "처음 보는 의사결정"을 강요받았다. 이 "차별화된 코어 동사(verb)"가 출시 화제성의 근원이었다.

### 5-2. 기술: 결정론적 서버사이드 파괴

화려한 파괴는 흔히 클라이언트마다 다르게 보여 경쟁 게임에 부적합하다. Embark는 파괴·물리를 서버에서 처리해 **모든 플레이어에게 동일한 결과**를 보장함으로써, "화려한 파괴"와 "공정한 경쟁"이라는 상충하는 요구를 동시에 충족했다. 이는 ex-DICE 기술진의 강점이 가장 직접적으로 발현된 부분이며, 마케팅에서 "거의 가짜 같은(almost don't believe it's real)" 파괴로 회자됐다(PC Gamer).

### 5-3. 출시 전략: TGA 셰도우 드롭

The Game Awards 2023에서 트레일러와 동시에 즉시 플레이 가능하게 푼 깜짝 출시는, 시상식의 폭발적 주목을 곧장 다운로드·동접으로 전환시켰다. 무료라는 진입 장벽 제거와 맞물려 피크 24만, 오픈베타 30만 근접이라는 초기 폭발을 이끌었다.

### 5-4. 컨셉의 일관성: 게임쇼 프레이밍

"VR 게임쇼"라는 설정은 톤(밝고 과장된 예능감), 디자인(부활·복제·파괴의 정당화), UI(방송 그래픽)를 하나의 정합적 세계로 묶었다. 어둡고 진지한 동시기 라이브 슈터들 사이에서 이 경쾌함은 뚜렷한 차별점이 됐다.

### 5-5. 혈통과 자본: ex-DICE + Nexon

《Battlefield》 파괴 유산을 직접 만든 인력이, EA의 IP·관료제 밖에서 자유롭게 그 아이디어를 극단까지 밀어붙였다. Nexon의 자본과 장기 운영 역량이 라이브 서비스 지속을 뒷받침했다. 흥미롭게도 개발진은 "이미 슈터를 해봤기에 처음엔 슈터를 만들 생각이 없었고, 만든다면 아무도 안 하는 독창적인 것이어야 한다"고 판단했다 — 그 결론이 곧 파괴 중심 게임쇼였다(GamesRadar).

### 5-6. 동시기 작품 대비 차별점

같은 시기의 히어로 슈터·배틀로열·전술 슈터들과 달리, 《THE FINALS》는 "환경 그 자체가 게임 메카닉"이라는 단일하고 강력한 축으로 정체성을 세웠다. 모방하기 어려운 서버사이드 파괴 기술이 이 차별성을 진입장벽으로 굳혔다.

---

## 6. 비평적 시각 / 한계 / 논란

### 6-1. AI 음성 논란 (가장 큰 쟁점)

2023년 10월 오픈 베타 중, Embark의 오디오 디자이너가 "모든 컨테스턴트 보이스 바크와 해설 멘트는 AI text-to-speech(ElevenLabs 기반)"라고 밝히면서 논란이 폭발했다. 개발진의 정당화는 "**AI TTS가 이제 매우 강력해, 몇 달이 아니라 몇 시간 만에 대사를 뽑을 수 있다**"는 것이었다(PC Gamer). 이는 실제 성우들의 반발을 샀다. 성우 Gianni Matragrano는 "성우들도 하루이틀 안에 급행 세션을 쉴 새 없이 처리한다, 우리를 쓰는 건 매우 쉽다"고 반박했고, 《Baldur's Gate 3》 등에 참여한 Elsie Lovelock은 "아무리 사실적이라고 우겨도 결국 형편없게 들린다"고 직격했다. Embark는 "게임 품질에 집중"하기 위해 AI 음성을 계속 쓰겠다는 방침을 고수했다. 이 사건은 한 게임의 논란을 넘어, 생성형 AI가 창작 노동을 대체하는 문제를 둘러싼 업계 전체의 시금석이 됐다.

### 6-2. 밸런스: Heavy 편중

파괴 잠재력과 350 HP를 동시에 가진 Heavy 클래스가 **경쟁 모드에서 과도하게 채택**되는 문제가 지적됐다(위키 reception 정리: "Heavies tend to be ubiquitous in competitive modes"). 시즌 패치로 무기·가젯이 추가·조정되며 메타가 바뀌었지만, 체급 기반 비대칭 디자인의 본질적 밸런싱 난도는 상시 과제였다.

### 6-3. 라이브 서비스 지속성: 급격한 이탈

피크 24만에서 두 달여 만에 월평균 2만대로 떨어진 곡선은 F2P 슈터의 가혹한 현실을 보여준다. 신선한 코어 동사에도 불구하고, 초기 콘텐츠 폭(맵·모드 수)·온보딩·매치메이킹·반복 동기 부여에서 장기 잔존을 확보하기 어려웠다는 평가가 따른다. Embark는 시즌제·이벤트 모드로 코어 팬층을 유지하는 방향으로 운영을 전환했다.

### 6-4. 기타: 성능·안티치트·코스메틱 가격

초기 클로즈드 베타에서 프레임·성능 문제가 보고됐고, 커널 레벨 안티치트 도입은 일부 플랫폼·사용자 우려를 낳았다(다만 Steam Deck 지원은 유지). 하드 화폐를 무과금으로 얻는 통로가 배틀패스에 한정돼 코스메틱이 비싸다는 불만도 누적됐다.

### 6-5. 평가가 갈리는 지점

"기술적으로는 동시대 최고 수준의 파괴를 구현했으나, 작가성·서사·정서(특히 AI 음성)에서는 비어 있다"는 분리 평가가 핵심이다. Eurogamer가 대표적으로, 순간의 화려함과 지속적 예술적 비전 사이의 간극을 문제 삼았다.

---

## 7. 영향과 유산

### 7-1. 장르적 영향: 파괴의 재정의

《THE FINALS》는 "**환경 파괴를 핵심 메카닉으로 삼은 경쟁 슈터가 상업적으로 성립할 수 있음**"을 실증했다. 《Battlefield》가 대규모 전장의 연출로서 파괴를 다뤘다면, 《THE FINALS》는 그것을 **소규모·고밀도 목표 기반 경쟁의 1차 전술 변수**로 압축했다. 서버사이드 결정론적 파괴라는 기술적 청사진은, 향후 파괴를 진지하게 다루려는 후발 슈터들이 참조할 레퍼런스를 만들었다.

### 7-2. Embark의 도약과 《Arc Raiders》

《THE FINALS》에서 검증된 파괴·물리 기술과 운영 노하우는 자매작 **《Arc Raiders》**(2025)로 이어졌다. 《Arc Raiders》는 출시 수개월 만에 **전 세계 1,400만 장 이상 판매**되며 Nexon의 "블록버스터" 프랜차이즈로 떠올랐고, 그 성공에 힘입어 **Patrick Söderlund은 Nexon의 executive chairman으로 임명**돼 회사 전반의 장기 전략·창작 방향에 대한 폭넓은 권한을 갖게 됐다(PC Gamer). 즉 《THE FINALS》는 그 자체로 메가히트는 아니었어도, Embark를 "기술 우선 스튜디오"로 각인시키고 후속 대박의 토대를 닦은 **전략적 마일스톤**이었다.

### 7-3. 산업적 의미: AI 창작 논쟁의 시금석

AI 음성 채택은 게임 산업에서 생성형 AI가 창작 노동을 대체하는 문제를 공론장으로 끌어낸 초기 대표 사례다. 이 논쟁은 이후 다른 스튜디오의 AI 활용 방침, 성우 노조(예: SAG-AFTRA)의 대응, 이용자 인식에 영향을 미쳤다.

### 7-4. 문화적 의미

"게임쇼 슈터"라는 신선한 톤과 무너지는 도시의 스펙터클은, 진지하고 무거운 라이브 서비스 일색이던 시장에 경쾌한 대안을 제시했다. 비록 동접 곡선은 급락했지만, 코어 팬층과 e스포츠(2025년 The Grand Majors 스톡홀름 개최, NTMR이 Team Secret을 꺾고 우승, 1위 상금 $37,500)를 통해 장수 운영의 길을 모색했다.

---

## 8. 부록

### 핵심 통계 표

| 지표 | 값 | 출처 |
| --- | --- | --- |
| Metacritic (PC) | 80 | Metacritic |
| OpenCritic | 85 | OpenCritic |
| IGN | 8/10 | IGN |
| GameSpot | 8/10 | GameSpot |
| Game Informer | 9/10 | Game Informer |
| Eurogamer | 3/5 | Eurogamer |
| 역대 피크 동접(Steam) | 242,619명 (2023.12.10) | Steam Charts |
| 2024.2 월평균(Steam) | 약 24,848명 | Steam Charts |
| 2025.2 월평균(Steam) | 11,760명(피크 19,499) | Steambase/Insider Gaming |
| 클래스 체력 | Light 150 / Medium 250 / Heavy 350 HP | Wikipedia |
| 배틀패스 가격 | 1,150 Multibucks | THE FINALS Wiki |

### 주요 일지

- 2022년: 《THE FINALS》 최초 공개(실제 게임플레이 트레일러).
- 2023.3.7~21: 클로즈드 베타 1.
- 2023.6.14~21: 클로즈드 베타 2.
- 2023.10.26~11.5: 오픈 베타(AI 음성 논란 발생).
- 2023.12.7: TGA 2023 셰도우 드롭 정식 출시.
- 2024.3.14: 시즌 2 시작.
- 2024.12.12: PS4 버전 출시.
- 2025.3.20: 시즌 6 시작.
- 2025.11.18: 중국판 출시(Tencent).

### 참고 자료 (영어권 매체 중심)

- The Finals — Wikipedia: https://en.wikipedia.org/wiki/The_Finals
- THE FINALS on Steam: https://store.steampowered.com/app/2073850/THE_FINALS/
- Game Informer(출시 보도): https://gameinformer.com/the-game-awards-2023/2023/12/07/the-finals-embark-studios-free-to-play-shooter-is-out-right-now
- GameSpot Review (8/10): https://www.gamespot.com/reviews/the-finals-review-an-explosive-game-show/1900-6418164/
- OpenCritic — The Finals: https://opencritic.com/game/15962/the-finals
- THE FINALS — Steam Charts(동접): https://steamcharts.com/app/2073850
- Game World Observer(오픈베타 30만 동접): https://gameworldobserver.com/2023/10/30/the-finals-created-by-former-dice-employees-enters-steams-top-five-most-played-games-attracting-nearly-300k-concurrent-players
- PC Gamer(AI 음성 논란): https://www.pcgamer.com/the-finals-uses-ai-text-to-speech-because-it-can-produce-lines-in-just-a-matter-of-hours-rather-than-months-baffles-actual-voice-actors/
- PC Gamer(파괴 사실감): https://www.pcgamer.com/i-almost-dont-believe-the-destructibility-in-this-fps-is-real/
- GamesBeat(파괴 기술 공개): https://gamesbeat.com/embark-studios-unveils-the-finals-team-based-shooter-game/
- Digital Trends(서버사이드 파괴/“panic”): https://www.digitaltrends.com/gaming/the-finals-preview-destruction-will-make-developers-panic/
- GamesRadar(파괴 물리/개발 배경): https://www.gamesradar.com/the-finals-preview-hands-on-march-2023/
- GamesRadar(슈터 안 만들려 했던 배경): https://www.gamesradar.com/the-finals-devs-werent-even-going-to-make-a-shooter-at-first-but-what-else-are-you-gonna-do-with-a-team-full-of-battlefield-veterans/
- Naavik(Embark, 기술 우선 스튜디오): https://naavik.co/digest/embark-technology-first-studio/
- PC Gamer(Arc Raiders 성공 / Söderlund Nexon 회장): https://www.pcgamer.com/gaming-industry/arc-raiders-is-such-a-huge-hit-nexon-has-put-embark-studios-ceo-patrick-soderlund-in-charge-of-everything-else-too/
- Embark Studios — Wikipedia: https://en.wikipedia.org/wiki/Embark_Studios
- THE FINALS Wiki(시즌/배틀패스): https://www.thefinals.wiki/

> 본 분석서는 영어권 매체 보도·공식 자료·위키 정보를 종합해 한국어로 재구성했다. 일부 수치(동접 등)는 Steam/PC 기준이며 콘솔 플레이어를 포함하지 않는다. 출시 후 시즌 업데이트로 무기·모드·밸런스가 지속 변동되므로, 시즌별 세부 수치는 발표 시점 기준이다.
