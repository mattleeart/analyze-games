# It Takes Two (2021) — 협동 어드벤처의 정점, 그리고 그 이면

> 분석 작성일: 2026-05-20
> 분석 대상: It Takes Two (Hazelight Studios / EA Originals, 2021)
> 작성 언어: 한국어 (영어권 원자료 인용 시 원문 병기)

---

## 1. 게임 개요

**It Takes Two**는 스웨덴 스톡홀름에 본사를 둔 **Hazelight Studios**가 개발하고 **Electronic Arts**가 **EA Originals** 레이블로 퍼블리싱한 2인 협동(co-op) 전용 액션 어드벤처 게임이다. 2021년 게임 업계에서 가장 의외이면서도 가장 결정적인 성공 사례 중 하나로 평가받는다.

### 개발사 / 퍼블리셔 / 장르
- **개발사**: Hazelight Studios (2014년 설립, 스톡홀름)
- **퍼블리셔**: Electronic Arts (EA Originals 레이블)
- **장르**: 협동(2인 전용) 액션 플랫포머 / 퍼즐 어드벤처. 챕터마다 장르가 변형되는 "장르 혼합형(genre-bending)" 구조가 특징이다.

### 출시일(플랫폼별)
- **PlayStation 4 / PlayStation 5 / Windows(PC) / Xbox One / Xbox Series X|S**: 2021년 3월 26일 (전 세계 동시)
- **Nintendo Switch**: 2022년 11월 4일 (이식 담당: Turn Me Up Games, 휴대 모드 720p / 도크 모드 1080p, 30fps 목표)

(출처: EA 공식 보도자료, 2020년 12월 10일자 — "EA and Hazelight Announce It Takes Two Coming to Consoles and PC on March 26, 2021"; Wikipedia)

### 디렉터 / 리드 / 주요 크레딧
- **디렉터 / 공동 작가**: Josef Fares (요세프 파레스). 영화감독 출신으로, Starbreeze 시절 **Brothers: A Tale of Two Sons**(2013), Hazelight의 데뷔작 **A Way Out**(2018)을 연이어 감독한 인물.
- **공동 작가**: Soni Jorgensen
- **프로듀서**: Aimar Bergan
- **리드 프로그래머**: Lucas de Vries
- **아티스트**: Claes Engdal
- **작곡**: Gustaf Grefberg, Kristofer Eng
- **주요 성우**: Cody — Joseph Balderrama / May — Annabelle Dowler / Rose — Clare Corbett. Dr. Hakim의 모션 캡처는 Josef Fares 본인이 담당했다.

### 개발 기간 / 규모
- Hazelight는 2018년 A Way Out 출시 직후 차기작에 착수, 약 3년에 걸쳐 개발했다.
- **개발 인력 약 60명** 규모(여러 영어권 매체 및 Wikipedia 공통 언급). AAA 대작 대비 매우 단출한 팀으로, "스튜디오 전체가 단 하나의 게임에 집중한다"는 Hazelight의 단일 프로젝트 철학이 반영됐다.
- 개발 예산의 구체 수치는 공식 비공개. [추정] EA Originals 구조상 EA가 개발비를 선지원하고 회수 후 수익 대부분을 Hazelight에 귀속시키는 모델이었다.

### 엔진 / 기술 스택
- **Unreal Engine 4** 기반.
- 게임플레이 로직 대부분을 Hazelight가 자체 개발한 **UnrealEngine-AngelScript 통합**(오픈소스로 공개: angelscript.hazelight.se)을 통해 **AngelScript**로 작성했다. C++ 대신 빠른 반복(iteration)이 가능한 스크립트 언어를 도입해, 챕터마다 완전히 새로운 메카닉을 끊임없이 시제품화·교체할 수 있었던 것이 이 게임의 "메카닉 폭발" 구조를 가능케 한 핵심 기술적 토대다.

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 컨셉과 핵심 발상
It Takes Two는 단 한 가지 명확한 설계 원칙 위에 세워졌다: **"강제된 협동(forced collaboration)"**. 혼자서는 단 한 발짝도 진행할 수 없으며, 두 플레이어가 끊임없이 말로 소통하고 서로 다른 능력을 맞물려야만 한 화면을 넘어갈 수 있다. Josef Fares는 인터뷰에서 일관되게 "협동(collaboration)이 게임 전체의 중심 테마"이며 "플레이어 간의 의사소통이 진행에 필수적이도록 설계했다"고 강조했다. 싱글플레이에 멀티를 덧붙인 것이 아니라, 기획 단계부터 2인 협동만을 전제로 만든 게임이라는 점이 결정적이다.

판매 패키지에는 단 하나의 라이선스로 친구 한 명을 무료로 초대할 수 있는 **Friend's Pass**가 포함된다. 한 명만 본편을 구매하면 두 번째 플레이어는 무료 클라이언트로 풀 게임을 함께 플레이할 수 있어, 협동 전용 게임의 진입 장벽을 구조적으로 허물었다.

### 세계관 / 줄거리 (스포일러 포함)

**[스포일러]** 결혼한 부부 **Cody**(코디)와 **May**(메이)는 서로에 대한 사랑이 식어 이혼을 계획 중이다. 어린 딸 **Rose**(로즈)는 부모의 이혼 소식을 받아들이지 못하고, 자신이 직접 만든 부모 인형(코디·메이를 본뜬 헝겊·점토 인형)을 가지고 헛간으로 가서 "엄마 아빠가 다시 화해하는" 역할극을 한다. 부모는 그런 노력에 전혀 관심이 없다.

로즈가 인형 위에 눈물을 흘리는 순간, 현실의 코디와 메이는 깊은 잠에 빠지고, 깨어나 보니 헛간 안에서 **각각 자신의 인형 몸에 갇혀 있다**. 거기서 둘을 맞이하는 것이 말하는 책 **"Book of Love"(사랑의 책)**, 즉 자칭 관계 상담 전문가 **Dr. Hakim**(닥터 하킴)이다. 하킴은 두 사람이 서로의 차이를 풀어내고 다시 사랑을 회복하기 전까지는 원래 몸으로 돌려보내 주지 않겠다고 선언한다.

두 사람은 로즈의 상상력이 빚어낸 거대한 드림스케이프(나무, 뻐꾸기 시계, 눈사람 스노우글로브, 정원, 다락방 등)를 가로지르며, 진공청소기·말벌·우주 개코원숭이(Space Baboons) 같은 장난감이 생명을 얻은 적들과 맞선다. 각 챕터의 메카닉과 능력은 두 사람의 성격, 그리고 그들 관계의 문제를 은유한다. 진행 과정에서 둘은 자신들의 불화가 딸 로즈를 얼마나 깊이 상처 입혔는지 깨닫는다.

**[스포일러 — 결말]** 마침내 인간의 몸으로 돌아온 부부는 로즈가 남긴 편지를 발견한다. 로즈는 "내가 엄마 아빠 이혼의 원인이라고 생각해서, 두 사람이 다시 친구가 될 수 있도록 가출했다"고 적었다. 코디와 메이는 버스 정류장에서 로즈를 찾아내, 그것은 결코 사실이 아니며 무슨 일이 있어도 둘 다 영원히 사랑할 것이라고 안심시킨다. 일부 매체(Twinfinite, TheGamer)는 결말이 "두 사람이 진짜로 화해해 이혼을 철회한 것인지, 아니면 더 좋은 부모로서 헤어지기로 한 것인지"를 의도적으로 모호하게 남긴다고 분석한다.

### 주요 캐릭터 / NPC
- **Cody**: 다소 게으르고 즉흥적이며 식물·정원을 좋아하던 면모를 잃어버린 아버지. 챕터에 따라 시간 조작·복제·점성 등 다양한 능력을 얻는다.
- **May**: 일에 매몰돼 음악(바이올린)에 대한 열정을 잊은 어머니. 망치·자석·검·돌진 등의 능력을 맡는다.
- **Rose**: 부모의 이혼에 죄책감을 느끼는 어린 딸. 사실상 모든 사건의 정서적 원동력.
- **Dr. Hakim**: 말하는 "사랑의 책". 과장된 라틴/지중해풍 억양과 끊임없는 참견으로 코믹 릴리프 역할을 하지만, 동시에 가장 호불호가 갈리는 캐릭터이기도 하다(아래 6장 참조).

### 무드 / 톤 / 아트 디렉션
전반적으로 **Pixar 애니메이션**을 강하게 연상시키는 따뜻하고 화사한 컬러 팔레트, 과장된 카툰 캐릭터, 미니어처화된 거대 세계(아이 방·정원·시계 내부 등)가 특징이다. 어두운 주제(이혼·가족 붕괴)를 다루면서도 시각적으로는 밝고 경쾌하며, 챕터마다 완전히 다른 비주얼 컨셉(거대한 나무 왕국, 마법 정원, 우주 록 콘서트, 다락방의 SF·판타지)을 선보여 시각적 다양성이 압도적이다.

### 사운드 / 음악
- **작곡**: Gustaf Grefberg, Kristofer Eng. 공식 OST는 33곡, 약 2시간 27분 분량.
- 챕터별로 오케스트라, 일렉트로닉, 록 등 장르를 넘나든다. 특히 우주 개코원숭이가 등장하는 챕터의 **"Moon Baboon Concert"**는 글램록/신스 사운드와 리듬 게임형 보스전이 결합된, 게임 내에서 가장 자주 회자되는 명장면이다.
- 사운드 디자인 비하인드는 오디오 전문 매체 **A Sound Effect**의 "Co-Oping on the Game Sound and Score for It Takes Two" 기사에 상세히 소개돼 있다.

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

It Takes Two의 게임 디자인적 정체성은 한 문장으로 요약된다: **"매 챕터, 매 구역마다 메카닉을 새로 발명하고, 사용한 뒤 버린다."** 다른 게임이라면 한 작품 전체를 지탱할 시스템 하나를 이 게임은 30분짜리 구간에 쓰고 폐기한다. 이 "기계적 풍요(mechanical abundance)"가 평론가들이 만장일치로 칭송한 지점이다.

### 코어 게임플레이 루프 (모먼트-투-모먼트)
- 화면은 기본적으로 **분할 화면(split-screen)**으로 구성되며, 온라인/로컬 모두 지원한다(온라인 시에도 양쪽에 분할 화면 연출이 적용되는 구간이 많다).
- 두 플레이어는 **항상 서로 다른 능력**을 부여받는다. 어느 한 쪽의 능력만으로는 퍼즐을 풀 수 없고, 반드시 두 능력을 시간차·공간차로 맞물려야 한다.
- 대표 예시(헛간/The Shed): May는 말하는 망치를, Cody는 날아가 박히는 못(nails)을 얻는다. Cody가 벽에 못을 박으면 May는 망치 머리를 못에 걸어 파쿠르로 이동하고, Cody가 플랫폼에 못을 고정하면 May가 그 위로 점프한다.
- 또 다른 예시(Snow Globe): 두 사람은 **서로 반대 극성의 자기력(magnetism)**을 얻어, 상대를 끌어당기거나 금속 구조물에 달라붙으며 진행한다.
- Cody의 시간 되감기(rewind)와 May의 자기 복제(self-replication)처럼, 능력 조합 자체가 곧 퍼즐의 해법이다.

### 진행 구조 (챕터 / 맵)
공식적으로 **7개 메인 챕터** 구조다. 도입부 헛간(The Shed)을 별도 프롤로그로 세면 8개로 보기도 한다.

| 순서 | 챕터 | 대표 컨셉/메카닉 |
|------|------|------------------|
| 0(프롤로그) | The Shed | 망치 + 못. 협동 기본기 튜토리얼 |
| 1 | The Tree | 점성(sap) 발사 + 성냥/폭발. 거대한 나무 왕국 탐험 |
| 2 | Rose's Room | (최장 챕터, 10개 구간·7개 미니게임) 시간 조작·복제 등 다양한 메카닉 집중 |
| 3 | The Cuckoo Clock | 시계 내부의 기계 장치 기반 플랫포밍·보스전 |
| 4 | Snow Globe | 반대 극성 자석. 스키·봅슬레이 액션 |
| 5 | The Garden | 식물 성장·씨앗 발사 등 정원 테마. "Moon Baboon Concert"가 이 부근에 위치 |
| 6 | The Attic | 검·돌진 등 SF/판타지 던전 크롤러풍 클라이맥스 |

(출처: Gamerant "It Takes Two: Chapter List", Hone Blog 등 다수의 가이드 매체 종합)

각 챕터는 단순히 배경만 바뀌는 것이 아니라, **장르 자체가 변형**된다. 한 구간은 3인칭 슈터, 다음은 리듬 게임, 또 다른 곳은 Diablo식 던전 크롤러나 비행 슈팅으로 변한다. 클리어 시간은 통상 **약 12~14시간**이며, 미니게임을 포함하면 그 이상이다.

### 협동 / 멀티 시스템
- **2인 전용**, 싱글플레이 불가. AI 동료 없음.
- **Friend's Pass**: 한 명만 구매하면 친구 한 명을 무료 초대 가능. 협동 게임의 고질적 진입 장벽(둘 다 사야 함)을 정면으로 해소한 핵심 마케팅·접근성 장치.
- **25개의 경쟁 미니게임**(게임 내 통계 기준): 체스, 눈싸움, 두더지 잡기, 비행기 경주 등 본편 진행과 무관한 선택형 경쟁 콘텐츠가 맵 곳곳에 숨어 있어, 협동 속에 가벼운 경쟁의 긴장을 더한다.

### 자원 관리 / 경제 / 진척도
- 전통적 RPG식 자원·경제·레벨업 시스템은 사실상 없다. 진척은 챕터·구간 클리어로만 이뤄지며, 능력은 부여→사용→폐기되는 일회성이다.
- 라이브 서비스, 시즌 패스, 마이크로트랜잭션(MTX) **전무**. 단발 패키지 판매형 프리미엄 타이틀로, 출시 시 비교적 저렴한 가격($39.99)으로 책정돼 가성비 인식도 높았다.

### 난이도 / 접근성
- 별도의 세분화된 난이도 옵션은 제한적이나, 액션 강도가 높지 않고 사망 시 즉시 부활(체크포인트 관대)하여 게이머가 아닌 파트너(연인·가족)와 함께 즐기기 용이하도록 설계됐다.
- 분할 화면 + 명확한 시각적 신호로, 게임에 익숙하지 않은 한쪽 플레이어도 따라올 수 있게 한 점이 "Best Family Game" 수상으로 이어졌다.

### UI/UX 디자인 철학
- HUD를 최소화하고, 퍼즐의 해법을 환경 디자인과 시각적 신호로 전달한다. "설명 대신 보여주기"가 원칙.
- 분할 화면은 단순 분할이 아니라 연출 도구로 활용된다. 한쪽이 줌아웃되어 전체 상황을 보고 다른 쪽이 클로즈업되는 식의 비대칭 화면 연출로, 두 사람이 서로 다른 정보를 보고 말로 공유하도록 강제한다.

---

## 4. 평가

### Metacritic / OpenCritic
- **OpenCritic**: 평균 **88점**, 151개 평론 기준(상위 평가). "Mighty(강력 추천)" 등급.
- **Metacritic 평론 점수(플랫폼별)**:
  - PC: **89/100**
  - PS4: **89/100**
  - PS5: **88/100**
  - Xbox Series X|S: **89/100**
  - Nintendo Switch: **83/100** (이식판은 기술적 타협으로 약간 낮음)

### 주요 평론 인용
- **IGN — 9/10**: "a beautiful, breakneck-paced, co-op adventure that's bubbling over with creativity"(아름답고 숨 가쁘게 질주하는, 창의성이 흘러넘치는 협동 어드벤처). 메카닉이 게임 내내 끊임없이 진화한다고 평가.
- **GameSpot — 9/10**: 창의성과 페이싱을 호평. "새로운 아이디어를 끊임없이 도입해 경험이 정체되지 않게 한다"고 평가.
- **GamesRadar+ — 5/5**: "근래 가장 독창적인 협동 플랫포머 중 하나".
- **Game Informer — 9.25/10**: 감정적 스토리를 협동 챌린지에 잘 연결했다고 평가.
- **PC Gamer — 80/100**: 상상력은 칭찬하면서도 "스크립트의 일부"와 **Dr. Hakim 캐릭터가 짜증난다(irritating)**고 명시적으로 비판.
- **Eurogamer — Recommended**: "스토리를 무시할 수 있다면, It Takes Two는 수년 내 최고의 협동 게임플레이를 제공한다"(If you can ignore the story...). 게임플레이는 극찬, 스토리는 약점으로 분리 평가한 대표 사례.
- **Jeuxvideo.com — 18/20**, **Shacknews — 9/10** 등 다수 매체 고평가.

### 수상 이력
- **The Game Awards 2021**: **Game of the Year(올해의 게임)** + **Best Multiplayer Game** + **Best Family Game** — 3관왕.
- **25th D.I.C.E. Awards (2022)**: **Game of the Year** + **Outstanding Achievement in Game Design** — 2관왕.
- **18th British Academy Games Awards(BAFTA, 2022)**: 8개 부문 후보(Returnal과 공동 최다), **Multiplayer** 및 **Original Property(오리지널 IP)** 부문 수상. (시상식: 2022년 4월 7일, 런던)
- **Golden Joystick Awards 2021**: Best Multiplayer Game.
- **The Steam Awards 2021**: "Better With Friends(친구와 함께가 더 좋은)" 부문.
- **SXSW Gaming Awards**: Excellence in Multiplayer.
- 그 외 Best Game Direction, Best Narrative 등 다수 후보 지명.

### 상업 지표 (판매량)
- 출시 1개월 내(2021년 4월): **100만 장**
- 2022년 중반: **700만 장**
- 2024년 10월: **2,000만 장 돌파** (Hazelight 공식 발표, GameSpot/Nintendo Life 등 보도)
- 2026년 4월 기준(Wikipedia): **3,000만 장 이상**으로 갱신

협동 전용 게임으로서, 또한 신규 IP로서 이 판매 곡선은 업계에서 대단히 이례적이다. Friend's Pass로 인해 "실제 플레이 인원은 판매량의 약 2배"라는 추정도 가능하다.

### 유저 평가 / 평론-유저 괴리
- Steam·각종 플랫폼에서 유저 평가도 매우 긍정적("압도적으로 긍정적" 수준)이며, "헤어진 커플이 클리어 후 다시 사귀거나, 클리어 도중 헤어졌다"는 식의 밈이 양산될 만큼 정서적 화제성을 얻었다.
- 다만 평론·유저 모두 게임플레이에는 만장일치에 가까운 호평을 보내면서도, **스토리·각본·캐릭터 톤**에 대해서는 분명한 균열이 존재한다(ResetEra의 "we kinda hate it" 스레드 등 소수의 강한 반대 의견도 존재). 이는 점수의 괴리라기보다 "게임플레이 vs 내러티브"라는 내부 분열에 가깝다.

---

## 5. 성공 요인 분석 (핵심)

### 1) 디자인 측면 — "강제 협동 + 메카닉 폭발"
가장 본질적인 성공 요인은 **타협 없는 2인 협동 전용 설계**와 **끊임없는 메카닉 교체**다. 대부분의 협동 게임이 싱글플레이에 협동을 덧붙이는 반면, Hazelight는 기획부터 협동만을 전제로 했다. 그 결과 "한 화면을 넘기려면 반드시 옆 사람과 말로 합을 맞춰야 하는" 경험이 만들어졌고, 이는 게임을 넘어 **두 사람의 관계를 시험하는 사회적 체험**으로 확장됐다. AngelScript 기반의 빠른 시제품화 파이프라인이 이 "발명-사용-폐기" 사이클을 기술적으로 뒷받침했다.

### 2) 마케팅 / 출시 전략 — Friend's Pass
협동 게임의 최대 약점인 "둘 다 사야 함"을 **Friend's Pass**로 정면 돌파했다. 한 명만 사면 친구가 무료로 합류하므로, 구매 결정의 심리적·금전적 장벽이 절반으로 줄었다. 더불어 출시가 $39.99로 책정돼 풀프라이스 대비 저렴해, "한 번 사면 둘이 즐기는 가성비 게임"이라는 인식을 굳혔다. 입소문(word of mouth)이 마케팅의 중심이 됐고, 이는 판매 곡선이 출시 후에도 장기간 우상향한 핵심 이유다.

### 3) 타이밍 / 시장 환경
2021년 3월은 **COVID-19 팬데믹**으로 사람들이 집에 머물며 가족·연인·동거인과 함께할 콘텐츠를 갈구하던 시기였다. "함께, 그러나 안전하게" 즐길 수 있는 로컬/온라인 협동 게임 수요가 정점이던 시점에 출시돼, 시대적 정서와 정확히 맞아떨어졌다.

### 4) 개발 / 운영 방법론 — 단일 프로젝트 집중 + EA Originals
Hazelight는 약 60명 규모의 작은 팀이 단 하나의 게임에만 집중하는 구조다. EA Originals 모델은 EA가 개발비를 대고 Hazelight가 창작 통제권과 수익 대부분을 가져가는 형태로, 대형 퍼블리셔의 자금력과 인디의 창작 자유를 결합했다. Josef Fares는 이 모델 덕에 "타협 없이 자기 비전을 밀어붙일 수 있었다"고 여러 차례 밝혔다.

### 5) 커뮤니티 / IP / 인물 효과
- Josef Fares는 2017년 The Game Awards에서 "**Fuck the Oscars!**"를 외친 것으로 유명하며(이 장면은 It Takes Two 안에 이스터에그로 삽입됨), 게임 매체에서 화제성이 큰 인물이다. A Way Out의 주인공 Leo·Vincent가 카메오로 등장하는 등 Hazelight 작품 간 연결고리도 팬덤을 자극했다.
- 스트리머·유튜버가 "둘이 함께 비명 지르며 협력하는" 콘텐츠로 소비하기에 최적화돼, 자연 발생적 바이럴이 강력했다.

### 6) 동시기 작품 대비 차별점
2021년에는 Returnal, Deathloop, Resident Evil Village 같은 강력한 싱글플레이 대작이 즐비했다. 그 속에서 It Takes Two는 "오직 협동, 오직 둘이서"라는 명확한 포지셔닝과 매 순간 새로운 메카닉이라는 차별성으로, GOTY 경쟁에서 대작들을 제치고 정상에 올랐다.

---

## 6. 비평적 시각 / 한계 / 논란

만장일치에 가까운 호평에도 불구하고, It Takes Two는 분명한 약점과 논쟁 지점을 안고 있다. 흥미롭게도 그 비판은 거의 전적으로 **게임플레이가 아니라 내러티브·각본**에 집중된다.

### 1) 스토리·각본의 약점 (가장 일관된 비판)
- Eurogamer의 "스토리를 무시할 수 있다면(If you can ignore the story)"이라는 표현은 이 게임의 내러티브 평가를 압축한다. 즉, 게임플레이는 최고지만 스토리는 따라오지 못한다는 것.
- Trusted Reviews 등은 내러티브를 "**contrived(작위적)**"하며 "**게임의 가장 약한 요소(easily the weakest element)**"라고 평했다. 일부 평론은 "뛰어난 레벨 디자인과 저급한 각본 사이의 격차가 대단히 어색하다(incredibly jarring)"고 지적했다.
- 캐릭터들이 "**다섯 살짜리처럼 말한다**", 끊임없이 티격태격하며 유치한 빈정거림을 반복한다는 비판이 존재한다(어른 부부의 대화로는 부자연스럽다는 것).

### 2) Dr. Hakim 캐릭터 논란
- PC Gamer는 Dr. Hakim을 "**irritating(짜증난다)**"고 직접 비판했다.
- 일부 평론·플레이어는 그의 과장된 라틴/지중해풍 억양과 캐리커처가 "**경계선상의 인종적 스테레오타입(borderline racist stereotype)**"에 가깝다고 문제를 제기했다. 반면 "오히려 두 주인공보다 하킴이 훨씬 재미있다"는 옹호도 공존해, 호불호가 극명히 갈린다.

### 3) 이혼이라는 주제의 피상성
- Paste Magazine은 "It Takes Two는 이혼을 다루지만, 정작 이혼에 대해 할 말이 별로 없다(doesn't have much to say about it)"고 지적했다. 무거운 주제를 다루면서도 정서적 깊이나 현실적 통찰이 부족하고, 결국 "관계 회복"이라는 결말로 봉합해 버린다는 비판이다.
- TheGamer의 "It Takes Two Made Me Root For Divorce(나는 오히려 이혼을 응원하게 됐다)" 같은 칼럼은, 주인공들의 미숙한 태도 탓에 플레이어가 화해보다 결별을 바라게 된다는 역설을 꼬집는다.

### 4) 강제 협동의 양면성
- "혼자 못 함"이라는 강점은 동시에 약점이다. 함께 플레이할 파트너가 없으면 게임을 시작조차 할 수 없다. 한쪽의 게임 실력 격차가 크면 한 사람이 양쪽 퍼즐을 사실상 캐리하게 되는 구간도 있다.

### 5) 평가가 갈리는 지점
- 점수 자체는 거의 갈리지 않지만(대부분 9점대), "이 게임을 GOTY로 인정할 것인가"를 두고는 의견이 갈렸다. 협동 전용·짧은 분량·약한 서사를 이유로 "혁신적 게임플레이는 맞지만 시대를 정의한 작품은 아니다"라는 시각도 있었다. 반대편에서는 "장르 자체를 재정의했다"는 평가가 우세하다.

---

## 7. 영향과 유산

### 장르에 미친 영향
It Takes Two는 **협동 어드벤처를 진지한 GOTY 후보 장르로 격상**시켰다. A Way Out에서 시작된 Hazelight의 "협동 전용 서사 게임" 공식을 완성형으로 끌어올렸고, "매 챕터 메카닉 교체"라는 디자인 언어를 업계에 각인시켰다. 협동 게임이 단순한 부가 모드가 아니라 그 자체로 최고 영예를 받을 수 있음을 증명한 분기점이다.

### 후속작 / 모방작 / 장르 확장
- Hazelight의 차기작 **Split Fiction**(2025년 3월 출시)은 It Takes Two의 공식을 정면 계승·확장했다. Mio와 Zoe라는 두 작가(SF·판타지)를 주인공으로, 이전작의 액션·플랫폼 요소에 더 풍부한 선택형 사이드 스토리와 한층 강화된 서사를 결합했다. 다수 매체(ScreenRant, DualShockers)는 Split Fiction이 "It Takes Two의 약점이던 각본·대사를 개선했다"고 평가하며, Hazelight가 협동 장르를 거듭 혁신하고 있다고 본다.
- It Takes Two의 성공 이후 "강제 협동 + 메카닉 다양성"을 표방하는 협동 게임 기획이 다수 등장했다.

### 산업적 의미
- **EA Originals 모델의 정당성**을 입증했다. 대형 퍼블리셔가 작은 스튜디오에 창작 자유를 주고 수익을 나누는 구조가 GOTY + 2,000만 장(이후 3,000만 장)이라는 결과를 낼 수 있음을 보여주며, 퍼블리셔-인디 협업 모델의 모범 사례가 됐다.
- AngelScript-Unreal 통합을 오픈소스로 공개해, 빠른 게임플레이 반복을 원하는 다른 개발사들에 기술적 영향을 줬다.

### 문화적 의미
- "It Takes Two로 커플 관계를 시험한다"는 밈이 정착할 만큼, 게임이 사회적 체험이자 관계의 리트머스로 소비됐다.
- **영화·TV 각색**이 dj2 Entertainment, Amazon MGM Studios, Story Kitchen, 그리고 Dwayne Johnson의 Seven Bucks Productions 협업으로 추진됐다(주연으로 Dwayne Johnson이 거론됨). 다만 Josef Fares는 2025년 진행 속도가 더디다며 불만을 표한 바 있고, Take-Two Interactive와의 상표권 분쟁(Hazelight가 상표 출원을 철회)도 보도됐다. 영화화 진척은 [추정] 2026년 현재에도 유동적이다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
|------|------|
| 개발사 | Hazelight Studios (스톡홀름) |
| 퍼블리셔 | Electronic Arts (EA Originals) |
| 디렉터 | Josef Fares |
| 엔진 | Unreal Engine 4 (게임플레이는 AngelScript) |
| 개발 인력 | 약 60명 |
| 출시일(콘솔/PC) | 2021년 3월 26일 |
| 출시일(Switch) | 2022년 11월 4일 (Turn Me Up Games 이식) |
| 장르 | 2인 협동 액션 플랫포머/퍼즐 어드벤처 |
| 챕터 수 | 7개 메인 챕터(+프롤로그 The Shed) |
| 미니게임 | 25개 |
| 클리어 시간 | 약 12~14시간 |
| Metacritic(PC) | 89/100 |
| OpenCritic 평균 | 88점 (151개 평론) |
| 대표 평론 | IGN 9/10, GameSpot 9/10, Game Informer 9.25/10, PC Gamer 80/100, Eurogamer Recommended |
| 주요 수상 | TGA 2021 GOTY·Best Multiplayer·Best Family / DICE 2022 GOTY·Game Design / BAFTA 2022 Multiplayer·Original Property |
| 판매량 | 100만(2021.4) → 700만(2022) → 2,000만(2024.10) → 3,000만+ (2026.4 기준) |
| 가격(출시 시) | $39.99 |
| 특이사항 | Friend's Pass(친구 1인 무료 초대), 라이브서비스·MTX 없음 |

### 주요 인터뷰 / 개발 자료
- **Unreal Engine 공식 개발자 인터뷰**: "It Takes Two lovingly marries story and gameplay together" — unrealengine.com
- **A Sound Effect**: "Co-Oping on the Game Sound and Score for It Takes Two" (사운드/음악 비하인드)
- **Hollywood Reporter**: "The Independent Gamer: 'It Takes Two' Director Josef Fares on Being Inspired by 'The Urge of Doing Something That Hasn't Been Done'"
- **Xbox Wire(2025)**: Josef Fares가 Split Fiction과 협동 장르 확장을 논한 인터뷰
- **Hazelight UnrealEngine-AngelScript 공식 문서**: angelscript.hazelight.se (오픈소스 기술 스택)

### 참고 자료 목록 (영어권 매체 중심)
- Wikipedia — "It Takes Two (video game)" / "Hazelight Studios" / "Josef Fares" / "AngelScript"
- Electronic Arts 공식 보도자료 (2020-12-10): 출시일 발표
- Metacritic — It Takes Two critic & user reviews (플랫폼별 점수)
- OpenCritic — It Takes Two (평균 88, 151 평론)
- GameSpot — Review(9/10) / Review Roundup / 2,000만 장 판매 보도
- IGN, GamesRadar+, Game Informer, PC Gamer, Eurogamer — 개별 리뷰
- Hollywood Reporter / VGC / NME — 2022 BAFTA 후보 및 수상 보도
- Nintendo Life — 2,000만 장 판매 및 Switch판 보도
- Paste Magazine — "It Takes Two Is About Divorce, but Doesn't Have Much to Say About It"
- TheGamer — "It Takes Two Made Me Root For Divorce" / 미답 질문 정리
- Twinfinite — Story Summary & Ending Explained
- Trusted Reviews / ResetEra — 내러티브 비판 및 소수 반대 의견
- ScreenRant / DualShockers — Split Fiction과의 비교 및 유산 분석
- A Sound Effect — 오디오/음악 제작 비하인드
- PCGamesN / PC Gamer — 영화화 및 Josef Fares 관련 보도

---

*본 분석서는 영어권 매체 및 공식 자료를 기반으로 작성됐으며, 수치·날짜는 출처를 명시했다. 일부 비공개 정보(정확한 개발 예산 등)는 [추정]으로 표기했다.*
