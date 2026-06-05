# 《Tooth and Tail》 (2017) 심층 분석

> "나는 《Monaco》로 잠입 장르에 했던 일을 RTS에 하고 싶다. 그건 컨트롤의 폭을 의도적으로 제약함으로써 실제 물리적 조작을 쉽게 만들되, 게임 자체의 복잡성은 깎아내지 않는 것이다." — Andy Schatz, Pocketwatch Games (Game Developer 인터뷰 의역)

《Tooth and Tail》은 인디 스튜디오 Pocketwatch Games가 2017년에 내놓은 실시간 전략(RTS) 게임이다. 단 한 문장으로 이 게임을 요약하면 "패드로 즐길 수 있는 10분짜리 RTS"다. 하지만 그 한 문장 뒤에는 RTS라는 장르가 1990~2000년대의 황금기 이후 사실상 대중적 활력을 잃어버린 이유를 정면으로 진단하고, 그 진단에 따라 장르의 골격을 분해·재조립한 설계 철학이 깔려 있다. 본 분석서는 《Tooth and Tail》을 단순한 "괜찮은 인디 RTS"가 아니라, **RTS 접근성 문제에 대한 하나의 디자인 선언서**로 읽고, 그 야심·성취·한계를 8개 섹션에 걸쳐 자세히 들여다본다.

---

## 1. 게임 개요

### 기본 정보

- **개발사 / 퍼블리셔**: Pocketwatch Games (자체 개발·자체 퍼블리싱)
- **출시일**: 2017년 9월 12일
- **플랫폼**: Microsoft Windows, macOS, Linux, PlayStation 4
- **장르**: 실시간 전략(RTS) — 단, "마이크로 관리와 높은 APM이 필요 없는 RTS"를 표방
- **엔진/기술**: Pocketwatch가 《Monaco》 시절부터 다듬어 온 자체 기술 기반(MonoGame/.NET 계열의 자체 파이프라인). 절차적 맵 생성 사용
- **플레이 인원**: 싱글플레이 캠페인 + 로컬 분할화면 멀티(최대 4인) + 온라인 랭크/언랭크 매치메이킹

### 주요 크레딧

- **창립자·디자이너·디렉터**: Andy Schatz — Pocketwatch Games의 설립자(2004년 창립). 2010년 IGF에서 《Monaco》 프로토타입으로 최고 영예인 Seumas McNally Grand Prize와 Excellence in Design을 동시 수상한 인물이다.
- **공동 디자이너 / 프로듀서·레벨 디자이너**: Andy Nguyen — 《Monaco》의 프로듀서 겸 레벨 디자이너 출신으로, 《Tooth and Tail》에서는 디자인과 더불어 **오픈 개발(open development) 커뮤니티 운영**을 주도했다. 2017년 GDC에서 "Tooth and Tail: Building Community Within Open Game Development"라는 강연을 진행했다.
- **음악**: Austin Wintory — 《Journey》(2012)로 게임 음악 사상 최초로 그래미 후보에 오른 작곡가이며, 《Monaco》의 음악도 맡았다. 본작으로 2018년 ASCAP Composers' Choice Awards에서 "2017 Video Game Score of the Year" 후보에 올랐다.
- **사운드 디자인**: PowerUp Audio — 인게임에서 동물들이 쓰는 가상 언어(중얼거리는 듯한 의사 언어)는 PowerUp Audio의 Kevin Regamey가 만들었다.

### 개발 규모와 위치

Pocketwatch Games는 미국 샌디에이고에 자리 잡은 소규모 인디 팀이다. Andy Schatz는 Amherst College를 졸업하고 TKO Software 등을 거친 뒤 2004년 자신의 스튜디오를 차렸고, 《Wildlife Tycoon: Venture Africa》(2005), 《Venture Arctic》(2007), 《Monaco: What's Yours Is Mine》(2013)에 이어 《Tooth and Tail》을 다섯 번째 정식 출시작으로 내놓았다(이후 2024~2025년 《Monaco 2》로 이어진다). 본작은 《Monaco》의 상업적·비평적 성공으로 확보한 예산과 명성을 바탕으로, 한 자릿수 규모의 코어 팀이 수년에 걸쳐 만든 결과물이다. 정확한 예산은 공개되지 않았으나, 대형 퍼블리셔 없이 자체 자금과 커뮤니티 기반 테스트로 진행한 전형적인 "중간 규모 인디" 프로젝트다.

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 컨셉과 세계관

《Tooth and Tail》은 **20세기 초 동유럽/러시아 혁명기를 모티프로 한 의인화된 동물들의 내전**을 그린다. 화면을 채우는 것은 군복을 입은 여우, 도롱뇽 같은 도마뱀, 부엉이, 스컹크, 두더지, 다람쥐, 멧돼지 같은 두 발로 걷는 짐승들이다. 세계관은 한 가지 잔혹한 전제 위에 서 있다. **이 사회는 만성적인 식량 부족에 시달리며, 동물들은 서로를 잡아먹는다.** 누가 먹고 누가 고기가 될 것인가 — 그것이 이 세계의 정치이자 전쟁의 이유다.

게임 제목 "Tooth and Tail" 자체가 군사 용어 "tooth-to-tail ratio"(전투 병력 대 후방 보급·지원 인력의 비율)에서 따온 것으로, 전쟁의 잔혹함과 보급·생존이라는 본작의 두 축을 압축한 명명이다. 비평가들은 이 세계관을 조지 오웰의 《Animal Farm》(동물농장)과 브라이언 자크의 《Redwall》 시리즈에 비교했다. 즉 귀여운 동물 우화의 외피를 쓰고 있지만 그 안에는 계급·혁명·기아·식인이라는 무거운 우화가 들어 있다.

### 줄거리와 4개 세력 [일부 스포일러]

이야기의 발단은 **"식량 추첨(lottery) 제도"**다. 지배 계급인 **The Civilized(문명파, 노랑)**가 누가 잡아먹힐지를 제비뽑기로 정하는 제도를 운영하는데, 이는 성직자 계급의 Archimedes가 주도한다. 부유한 상인 Bellafide의 아들이 추첨에 걸려 요리될 위기에 처하자, Bellafide가 이끄는 **The Longcoats(롱코트, 파랑)**가 봉기한다. 이들의 목표는 "능력에 따라 누가 먹히는지를 정하는" 메리토크라시(능력주의)의 도입이다.

여기에 억압받던 떠돌이·빈민들이 Hopper를 지도자로 삼아 **The Commonfolk(평민파)**로 결집해, 투표로 결정하자는 민주주의적 주장을 들고 혁명에 가담한다. 마지막으로 봉건 잔재의 상징인 Tsarina(여제)에게 충성하는 비밀경찰 **The KSR(케이에스아르)**가 Quartermaster를 앞세워 진압에 나선다.

이 네 세력의 혼전 위에 본작의 가장 냉소적인 반전이 놓인다. **돼지(Swine)**다. 이 세계에서 돼지는 고기를 먹지 않는 유일한 종족이며, 그래서 각 세력의 농장에서 사실상 노예 노동력으로 부려진다. [스포일러] 캠페인의 진행에 따라 돼지들은 네 군대를 서로 충돌하도록 교묘히 조종하고, 결국 모두가 지친 마지막 순간에 봉기하여 살아남은 군대를 기습한다. 능력주의든 민주주의든 군주제든, 누군가를 먹어 치우는 구조 자체는 바뀌지 않으며, 가장 밑바닥의 착취당하던 계급이 그 구조를 뒤집는다는 결말은 동물 우화의 외피에 비해 놀랍도록 정치적이다.

### 무드·톤·아트 디렉션

비주얼은 **"현대화된 1990년대 픽셀 아트"**다. 전술 시점은 도트 기반의 거칠고 어두운 픽셀로 그려져 있고, 유닛 카드와 일러스트는 만화적이면서도 그로테스크하게 음울한 톤을 띤다. Schatz는 아트 방향에 대해 "게임은 절대적으로 멋져지기 전까지는 완전히 형편없어 보여야 한다"는 다소 도발적인 원칙을 내걸었는데, 이는 외형보다 시스템의 작동을 먼저 완성하고 비주얼은 마지막에 다듬는 그의 개발 철학을 드러낸다. 전체적인 분위기는 진흙과 화약 냄새가 나는 참호전, 흑백 선전 포스터, 소비에트 구성주의를 떠올리게 하는 우중충하고 비장한 톤이다. 귀여운 동물이지만 결코 명랑하지 않다.

### 사운드와 음악

본작의 가장 보편적으로 칭찬받는 요소가 **Austin Wintory의 음악**이다. Wintory와 Schatz는 게임의 음악적 방향을 정하면서 1차 세계대전과 러시아 혁명을 테마로 잡았고, **20세기 초 러시아 악기들로만 연주하되, 게임이 거칠고 광란적이므로 그 악기들을 "취한 듯이(drunkenly)" 연주한다**는 컨셉을 세웠다. 그 결과 23개 트랙의 사운드트랙은 빠른 타란텔라, 오르간·바이올린 탱고, 게르만풍 왈츠, 동유럽 민속춤이 뒤엉킨 독특한 질감을 갖는다. 각 동물 세력마다 고유 테마가 부여되어 있어, 음악 자체가 세계관의 계급·민족적 다층성을 표현한다. 사운드트랙은 Varèse Sarabande에서 2LP 바이닐로도 발매되었다.

---

## 3. 핵심 시스템 / 메카닉 — 가장 자세히

《Tooth and Tail》을 이해하는 핵심은, 이 게임이 RTS의 어떤 "기둥"을 남기고 어떤 기둥을 도려냈는가를 보는 것이다. Schatz는 RTS를 **자원 채집, 군대 관리, 영토 통제**라는 세 개의 가장 본질적인 축으로 환원하고, 그 외의 거의 모든 관습적 부담을 제거했다.

### 가장 급진적인 결정 — 커서를 없애고 지휘관을 직접 조종한다

전통적인 RTS에서 플레이어는 신(神)의 시점에서 마우스 커서로 유닛을 클릭·드래그하며 명령을 내린다. 《Tooth and Tail》은 이 커서 자체를 없앤다. 대신 플레이어는 **자기 세력의 지휘관 캐릭터를 직접 맵 위에서 조종**한다. 깃발을 든 이 지휘관이 곧 플레이어의 분신이자 커서다. 건물을 짓는 것도, 병력을 소집·집결시키는 것도, 특정 표적에 집중 사격을 명령하거나 후퇴를 지시하는 것도 전부 이 지휘관을 통해서만 이루어진다.

이 한 가지 결정이 게임 전체의 성격을 바꾼다. 명령을 내리려면 지휘관이 **물리적으로 그 자리에 가 있어야** 하므로, "어디에 내가 있을 것인가"가 곧 전략이 된다. 게다가 지휘관이 전선에 너무 가까이 가면 **죽을 위험**에 노출된다. 신의 시점에서 안전하게 모든 것을 통제하던 RTS 사령관이, 이제는 전장을 직접 누비며 자기 목숨을 걸어야 하는 한 명의 존재가 된 것이다. 이것이 패드 한 손으로 RTS를 가능하게 만든 결정적 장치다. 좌측 스틱으로 지휘관을 움직이고, 몇 개의 버튼으로 건설·소집·명령을 수행한다. 마우스의 정밀 클릭이 필요 없다.

### 6장 덱 시스템 — Hearthstone와 StarCraft의 교배

매치 시작 전, 플레이어는 **20종의 유닛 풀에서 6종을 골라 자신의 "덱"을 구성**한다(공격 유닛 15종 + 방어/요새 유닛 5종 계열로 구성). Schatz는 이 게임의 목표를 노골적으로 "《StarCraft》를 《Hearthstone》화하는 것(to Hearthstone StarCraft)"이라 표현했다. 즉 StarCraft식의 실시간 macro/micro 깊이를, Hearthstone식의 덱빌딩이라는 사전 선택·메타 게임으로 감싼 것이다.

이 6장 덱이 시스템 전체의 무게중심이다. 전통적 RTS처럼 종족별로 고정된 거대 테크트리를 외울 필요가 없다. 대신 플레이어는 매 판 자신이 들고 갈 6개의 도구를 직접 디자인한다. 초반 견제에 특화된 스웜형 덱, 원거리 화력에 올인한 덱, 방어 요새와 후반 거포에 의존하는 덱 등 무한히 다른 빌드가 가능하며, 이로 인해 발생하는 **상성과 메타 게임**이 멀티플레이의 핵심 재미를 이룬다.

### 유닛 3티어 구조

유닛은 생산 비용과 역할에 따라 대략 세 티어로 나뉜다.

- **티어 1 (저비용 스웜)**: 여우, 족제비 같은 값싼 유닛. 초반 견제와 물량으로 방어선을 압박하는 데 쓰인다.
- **티어 2 (특화 능력)**: 독가스를 던지는 스컹크 같은 원거리 유닛, 화염방사를 쓰는 멧돼지 같은 근접 강화 유닛 등 특수 역할을 맡는다.
- **티어 3 (고투자 거물)**: 공수부대를 투하하는 부엉이, 장거리 폭격용 중포 같은 고비용·고효율 병기. 한 번에 판을 뒤집을 수 있지만 자원 소모가 크다.

핵심은 단순한 유닛들이 **서로 상호작용할 때 복잡성이 발생한다**는 Schatz의 철학이다. 개별 유닛은 외우기 쉽지만, 6장 덱의 조합과 상성, 그리고 전장에서의 배치가 깊은 전략 공간을 만든다.

### 자원·경제 — Gristmill과 식량

경제의 중심은 **Gristmill(제분소)**과 **식량(food/meat)**이다. Gristmill은 식량을 생산하는 자원 시설이고, 이 식량으로 유닛을 뽑고 농지(farmland, 약 60 "meat" 비용)를 사들여 영토를 확장한다. 결정적으로, **Gristmill이 파괴되면 추가 유닛을 생산할 수 없을 뿐 아니라 기존 유닛들이 굶주리기 시작한다**. 즉 보급이 끊기면 군대가 아사한다. 세계관의 "식량 전쟁"이라는 테마가 메카닉으로 직접 구현된 셈이다. Warren(병영) 같은 생산 시설에서 유닛을 찍어내고, Campfire(모닥불)는 자원·생산 기능이 결합된 거점 역할을 한다.

**승리 조건**은 명확하다. 적의 Gristmill과 Campfire를 모두 파괴하면 이긴다. 영토를 장악해 적의 식량 기반을 무너뜨리는 것이 곧 승리로 이어지므로, "영토 통제"라는 RTS의 본질이 압축적으로 살아 있다.

### 진행 구조와 절차적 맵

멀티플레이 한 판은 **약 10분 이내**에 끝나도록 설계됐다. Schatz가 내건 디자인 원칙 — 최소한의 버튼, 줄어든 마이크로, 5~12분 매치, 단순하지만 상호작용으로 복잡해지는 메카닉 — 이 그대로 구현된 길이다. 맵은 **절차적으로 생성**되어 매 판 다른 지형이 나온다. 싱글플레이 캠페인은 네 세력의 시점을 오가는 미션들로 구성되며, 각 미션은 마치 "한입 크기 StarCraft 캠페인"처럼 짧은 전투 시나리오로 짜여 있다(PC Gamer의 표현).

### 컨트롤·접근성·UI 철학

본작의 UI/UX 철학은 한마디로 **"제약을 통한 접근성"**이다. Schatz는 "패드를 잘 활용하는 '좋은' RTS가 하나도 없었다"는 문제의식에서 출발했다. 마우스 정밀 클릭과 높은 APM이라는 진입장벽을 제거하는 대신, 깊이는 덱빌딩·배치·타이밍 같은 다른 차원으로 옮겨 놓았다. 패드와 키보드+마우스를 모두 지원하며, 로컬 분할화면(최대 4인)까지 가능해 거실에서 친구와 RTS를 한다는, 장르적으로 거의 전례 없는 경험을 제공한다.

---

## 4. 평가

### 종합 점수

- **Metacritic (PC)**: 80/100 (27개 평론 기준)
- **Metacritic (PS4)**: 78/100
- **OpenCritic**: 80/100, **"88% Critics Recommend"**
- 종합 컨센서스: 양 플랫폼 모두 "Generally favorable reviews"(대체로 호평)

### 주요 매체 평론

- **Destructoid (Patrick Hancock): 9.5/10** — 본작에 대한 최고 평점 중 하나. "RTS를 싫어하는 사람을 포함해 누구에게나 추천한다"고 단언했다. 접근성과 디자인의 우아함을 극찬했다.
- **GameSpot: 8/10** — "열두 가지 훌륭한 아이디어로 빚은 기묘한 칵테일(a bizarre cocktail of a dozen great ideas)"이라는 인상적인 평을 남겼다.
- **PC Gamer** — "패드로 즐겨도 기분 좋은, 빠른 템포의 실시간 전략"이라 호평하며, 싱글플레이를 "한입 크기 StarCraft 캠페인"에 비유했다. 다만 진입 곡선의 가파름을 지적했다.
- **Polygon (Charlie Hall)** — "현재로서는 초기 학습 곡선이 대부분의 플레이어에게 너무 가파르다"며 접근성 의도와 실제 체감 사이의 간극을 비판적으로 짚었다.
- **Hardcore Gamer: 4/5**, **AusGamers: 8.1/10**, **Eurogamer Italy: 9/10** 등도 대체로 긍정적이었다.
- **IGN** — 2017년 9월 "당신이 놓쳤을지 모르는 게임"으로 소개했고, 연말 "Best of 2017"에서 "Best Strategy Game" 후보에 올렸다.

대다수 평론에서 **멀티플레이가 싱글플레이보다 더 높은 찬사**를 받았다. 비평가들은 한결같이 아트 스타일, 사운드트랙, 오디오 디자인을 극찬했고, 멀티플레이의 짜릿함·뉘앙스·접근성을 높이 샀다. 반면 싱글플레이 캠페인의 난이도 스파이크는 즐거움을 해친다는 지적이 반복됐다.

### 수상 및 후보

- **Intel Level Up 2016**: "Best Character Design" 수상
- **Media Indie Exchange 2016**: "Guest's Pick" 수상(Giant Cop과 공동)
- **The Game Awards 2017**: "Best Strategy Game" 후보
- **PC Gamer 2017 GOTY**: "Best Strategy Game" 후보 + "Best Game Music" 리스트 선정
- **IGN Best of 2017**: "Best Strategy Game" 후보
- **2018 Independent Games Festival(IGF)**: "Excellence in Narrative" 후보
- **2017 SXSW Gaming Awards**: "Gamer's Voice (Multiplayer)" 후보
- **2018 ASCAP Composers' Choice Awards**: Austin Wintory의 음악, "2017 Video Game Score of the Year" 후보

소규모 인디 RTS로서 The Game Awards·IGN·PC Gamer의 "올해의 전략 게임" 후보에 동시에 오른 것은 의미가 작지 않다. 이는 AAA 전략 게임이 희소해진 시기에 본작이 장르의 대표 주자로 인식되었음을 보여준다.

### 유저 평가와 상업 지표

Steam에서 본작은 대체로 긍정적 평가를 유지했고, 특히 멀티플레이의 깊이와 짧은 호흡, 패드 지원을 높이 사는 코어 팬층을 확보했다. 다만 정확한 판매량은 Pocketwatch가 공식적으로 공개하지 않았다. [추정] 《Monaco》 수준의 대형 히트에는 미치지 못했으며, 충성도 높지만 규모가 큰 편은 아닌 플레이어 베이스를 가졌다고 보는 것이 합리적이다. 유저 사이에서 가장 갈린 지점은 평론과 동일하게 **싱글 캠페인의 난이도와 절차적 맵의 운**, 그리고 출시 이후 온라인 멀티플레이 모집단의 규모였다.

---

## 5. 성공 요인 분석 (핵심)

### (1) 명확한 문제 정의 — "RTS는 왜 대중을 잃었나"

본작의 출발점은 트렌드가 아니라 **장르 진단**이었다. Schatz는 RTS가 1990~2000년대의 정점 이후 대중적 활력을 잃은 이유를 마이크로 관리 부담과 높은 APM, 그리고 마우스 의존적 인터페이스에서 찾았다. 《Monaco》에서 잠입 장르의 컨트롤을 극단적으로 단순화해 성공한 경험을, 그대로 RTS에 적용한 것이다. "컨트롤의 폭은 좁히되 게임의 복잡성은 유지한다"는 일관된 철학이 디자인 전반을 관통한다. 성공 요인의 9할이 여기서 나온다 — **무엇을 덜어낼 것인가에 대한 확신.**

### (2) 패드 RTS라는 미개척 시장

"패드로 제대로 되는 RTS가 없다"는 빈틈은 명백했고, 본작은 지휘관 직접 조종 + 6장 덱이라는 두 장치로 그 빈틈을 정확히 메웠다. PS4 동시 출시와 로컬 분할화면 4인 지원은, 거실에서 친구와 즐기는 RTS라는 거의 독점적인 경험을 가능하게 했다. 콘솔 전략 게임이라는 희소한 카테고리에서 본작은 강력한 차별점을 가졌다.

### (3) 오픈 개발(Open Development)과 커뮤니티 빌딩

본작 성공 방법론의 정수는 **개발 과정 자체를 공개한 것**이다. Pocketwatch는 일찍부터 개발 과정을 Twitch로 생중계했고, Schatz는 이를 "소형 PAX"라 불렀다. Andy Nguyen이 2017년 GDC에서 발표한 "Building Community Within Open Game Development" 강연은 이 방법론의 교본이다. 핵심 골자는 다음과 같다.

- 무료 온라인 도구를 활용해 개발 중 커뮤니티를 키우고 기대감을 형성한다.
- 그 커뮤니티가 개발을 보조하고 프로젝트 범위를 오히려 확장시킨다 — 커뮤니티 주도 경쟁 씬, 지원받는 스트리밍 콘텐츠 네트워크, 꾸준한 테스트·QA, 끊임없는 플레이어 피드백과 밸런스 데이터.
- 클로즈드 알파 단계에서 이미 활발한 경쟁 씬이 형성되어, 단순해 보이는 게임에 깊은 micro/macro가 존재함을 입증했다.
- PAX East 등 오프라인 행사에서 'Glyde' 같은 핵심 커뮤니티 멤버가 개발을 돕고 신규 플레이어 피드백 창구를 만들었다.

흥미롭게도 Pocketwatch는 Early Access를 검토했으나 **거부**했다. 대신 커뮤니티 테스트는 받되 정식 출시는 완성된 형태로 한다는 길을 택했다. 이는 소규모 팀이 자금·QA·밸런스·마케팅을 외부 인력 없이 해결하면서도 출시 시점의 완성도를 지키는, 영리한 절충이었다.

### (4) 음악과 아트의 정체성

Austin Wintory의 "취한 러시아 악단" 사운드트랙과 우중충한 픽셀 아트는, 단순한 외피가 아니라 게임의 정체성 그 자체였다. 모든 평론이 입을 모아 칭찬한 이 두 요소는, 본작이 수많은 인디 RTS 사이에서 즉각적으로 기억되게 만들었다. 능력주의·민주주의·군주제·노예 봉기를 동물 우화로 풀어낸 IGF "Excellence in Narrative" 후보급 서사 역시, 게임플레이만으로는 얻기 어려운 비평적 무게를 더했다.

### (5) 비교 가능한 동시기 작품 대비 차별점

2017년 전후는 AAA RTS가 사실상 고갈된 시기였다. StarCraft II는 마지막 확장팩 이후 운영 단계였고, 새로운 대형 RTS는 드물었다. 이 공백에서 본작은 "10분, 패드, 덱빌딩"이라는 완전히 다른 문법으로 등장해, 기존 RTS의 무게에 지친 이들과 RTS를 한 번도 즐기지 못했던 이들 양쪽을 동시에 겨냥했다. 같은 인디 전략군의 다른 작품들이 깊이나 그래픽으로 승부할 때, 본작은 **장르 자체의 재설계**로 승부했다는 점이 결정적 차별점이다.

---

## 6. 비평적 시각 / 한계 / 논란

### (1) 싱글플레이 캠페인의 난이도와 설계 결함

본작의 가장 일관된 약점은 **싱글플레이 캠페인**이다. 여러 평론과 유저가 "짧고 평범한 캠페인", "난이도 스파이크가 즐거움을 해친다"고 지적했다. 특히 문제가 된 것은 **절차적 맵 생성**이다. 미션 맵이 무작위로 생성되다 보니, 난이도가 순전히 "맵이 어떻게 굴러나왔는가"에 좌우되는 경우가 생겼다. 한 유저는 특정 미션을 15~20회 실패하고도 무엇을 다르게 해야 할지 알 수 없었다고 토로했는데, 시작 위치가 자원 농장에서 너무 멀거나 통과 불가능한 지형에 둘러싸여 **처음부터 패배가 확정된** 판이 나올 수 있다는 것이 핵심 불만이었다. 멀티에서 매판 다른 맵이 신선함을 주는 장점이, 싱글에서는 통제 불가능한 운으로 변질된 셈이다.

또한 캠페인은 유닛 각각의 특성이나 전략을 충분히 설명하지 않는다는 비판도 있었다. 튜토리얼 기능을 겸해야 할 캠페인이, 오히려 신규 플레이어를 충분히 안내하지 못한다는 모순이다.

### (2) 접근성 의도와 학습 곡선의 간극

본작은 "접근성"을 표방했지만, 역설적으로 Polygon은 "초기 학습 곡선이 대부분의 플레이어에게 너무 가파르다"고 평했다. 컨트롤은 단순해졌으나, 6장 덱의 상성·타이밍·배치라는 새로운 깊이를 익히는 과정은 결코 쉽지 않았다. 즉 "조작은 쉽지만 잘하기는 어렵다"는 구조가, 캐주얼 유입을 노린 의도와 충돌하는 지점이 분명히 존재했다.

### (3) 멀티플레이 모집단의 지속성

본작의 진짜 가치는 멀티플레이에 있다는 데 평론이 일치하지만, 그렇기에 **온라인 플레이어 모집단의 규모와 지속성**이 게임의 장기 수명을 좌우하는 약점이 되었다. 짧은 매치와 깊은 메타를 갖춘 경쟁 RTS는 충성도 높은 코어 씬에 의존하는데, 인디 규모로는 그 씬을 대규모로 유지하기 어렵다. 출시 후 시간이 지나며 신규 매칭이 어려워졌다는 우려가 커뮤니티에서 제기되었고, 이는 PvP 중심 인디 전략 게임이 공통적으로 겪는 구조적 한계였다.

### (4) 평가가 갈리는 지점 정리

- **"우아한 재설계"인가, "얄팍한 단순화"인가**: 일부는 본작을 RTS의 본질을 꿰뚫은 우아한 압축으로 봤고(Destructoid 9.5), 일부는 단순화의 대가로 전통 RTS의 묵직함을 잃었다고 봤다.
- **싱글 vs 멀티**: 멀티는 거의 만장일치 호평, 싱글은 거의 만장일치 아쉬움. 어느 쪽을 주로 즐기느냐에 따라 체감 만족도가 크게 갈렸다.
- **운(절차적 맵) 의존**: 신선함의 원천이자 불공정의 원천이라는 양날의 검.

---

## 7. 영향과 유산

### 장르에 미친 영향

《Tooth and Tail》은 상업적 메가히트는 아니었지만, **"RTS는 어떻게 단순화될 수 있는가"에 대한 가장 명료한 사례 연구** 중 하나로 남았다. 지휘관을 직접 조종하는 커서 제거, 6장 덱빌딩, 10분 매치, 패드 우선 설계라는 조합은, RTS 접근성 문제를 논할 때 반복적으로 인용되는 레퍼런스가 되었다. 특히 "마우스 클릭과 APM 없이도 전략적 깊이를 유지할 수 있는가"라는 질문에 본작은 분명한 긍정의 증거를 제시했다.

### 오픈 개발 방법론의 교본

본작의 더 큰 유산은 **개발 방법론**에 있다. Andy Nguyen의 GDC 강연 "Building Community Within Open Game Development"는, 소규모 팀이 Twitch 생중계·커뮤니티 테스트·경쟁 씬 육성으로 부족한 자원(QA, 밸런싱, 마케팅)을 메우는 방법의 교본이 되었다. Early Access를 쓰지 않으면서도 커뮤니티의 힘을 빌려 출시 완성도를 끌어올린 사례로, 인디 개발 담론에서 자주 거론된다.

### 후속·계보

Pocketwatch Games는 이후 《Monaco 2》(2024~2025) 개발로 방향을 틀었으나, 《Tooth and Tail》에서 입증한 "컨트롤 제약을 통한 접근성"이라는 스튜디오의 일관된 디자인 DNA는 그대로 이어진다. 또한 본작은 출시 후에도 커뮤니티 피드백 기반의 무료 업데이트로 유닛·밸런스·모드를 보강하며, 소규모 팀이 라이브 운영에 가까운 사후 지원을 시도한 사례를 남겼다.

### 산업적·문화적 의미

산업적으로 본작은 **AAA RTS 공백기에 장르의 명맥을 인디가 이어받은** 상징적 사례다. 콘솔/패드 전략 게임이라는 희소 카테고리를 개척했고, "전략 게임은 PC 마우스 전용"이라는 통념에 균열을 냈다. 문화적으로는 귀여운 동물의 외피 속에 계급·혁명·기아·식인이라는 묵직한 정치 우화를 담아, 게임이 우화로서 정치를 말하는 한 방식을 보여주었다. 《Animal Farm》과 《Redwall》을 동시에 떠올리게 한다는 비평은, 본작이 단지 잘 만든 RTS를 넘어 **하나의 이야기로서도 진지하게 읽혔음**을 의미한다.

---

## 8. 부록

### GDC / 포스트모템 자료

- **Andy Nguyen, "Tooth and Tail: Building Community Within Open Game Development" (GDC 2017)** — 오픈 개발과 커뮤니티 빌딩 방법론의 핵심 강연. GDC Vault 및 YouTube에서 시청 가능.
  - GDC Vault: https://gdcvault.com/play/1024164/Tooth-and-Tail-Building-Community
  - YouTube: https://www.youtube.com/watch?v=7_B--jnAuCM
- **Andy Schatz, "A Journey to Monaco: Andy Schatz Looks Back" (Game Developer/Gamasutra)** — 스튜디오 역사와 디자인 철학의 배경.

### 주요 인터뷰

- **"Crafting Tooth & Tail, a gamepad RTS that aims 'to Hearthstone StarCraft'" (Game Developer / Gamasutra)** — Schatz의 디자인 철학("StarCraft를 Hearthstone화"), 컨트롤 제약 철학이 가장 잘 드러나는 인터뷰. https://www.gamedeveloper.com/design/crafting-i-tooth-tail-i-a-gamepad-rts-that-aims-to-i-hearthstone-starcraft-i-
- **Gamereactor, "Andy Schatz on Tooth and Tail"** — 세계관과 개발 방향 인터뷰.
- **The PC Gamer Show / Super BS Presents** — Schatz가 직접 플레이하며 디자인 의도를 설명하는 영상 인터뷰.

### 핵심 통계 표

| 항목 | 내용 |
| --- | --- |
| 개발사·퍼블리셔 | Pocketwatch Games (자체) |
| 디렉터·디자이너 | Andy Schatz / 공동 디자이너 Andy Nguyen |
| 음악 | Austin Wintory (《Journey》, 《Monaco》 작곡가) |
| 사운드 | PowerUp Audio (가상 언어: Kevin Regamey) |
| 출시일 | 2017년 9월 12일 |
| 플랫폼 | Windows, macOS, Linux, PlayStation 4 |
| 장르 | 실시간 전략(RTS), 패드 친화·저(低)마이크로 |
| 워킹 타이틀 변천 | Dino Drop(대학 시절) → [ARMADA](2014.3) → LEADtoFIRE(2014.8) → Tooth and Tail(2015.8) |
| 핵심 메카닉 | 지휘관 직접 조종, 20종 중 6종 덱빌딩, Gristmill 식량 경제, 절차적 맵 |
| 매치 길이 | 약 10분 이내 |
| Metacritic (PC) | 80/100 (27 평론) |
| Metacritic (PS4) | 78/100 |
| OpenCritic | 80/100, 88% Critics Recommend |
| 대표 평점 | Destructoid 9.5 · GameSpot 8 · Hardcore Gamer 4/5 · AusGamers 8.1 · Eurogamer Italy 9 |
| 주요 후보 | TGA·IGN·PC Gamer "Best Strategy Game"(2017), IGF "Excellence in Narrative"(2018), ASCAP "Score of the Year"(2018) |

### 참고 자료 목록 (영어권 매체 중심)

- Wikipedia, "Tooth and Tail" — https://en.wikipedia.org/wiki/Tooth_and_Tail
- Wikipedia, "Andy Schatz" — https://en.wikipedia.org/wiki/Andy_Schatz
- Game Developer (Gamasutra), "Crafting Tooth & Tail, a gamepad RTS..." — https://www.gamedeveloper.com/design/crafting-i-tooth-tail-i-a-gamepad-rts-that-aims-to-i-hearthstone-starcraft-i-
- GDC Vault, "Building Community Within Open Game Development" — https://gdcvault.com/play/1024164/Tooth-and-Tail-Building-Community
- GameSpot, "Tooth and Tail Review" (8/10) — https://www.gamespot.com/reviews/tooth-and-tail-review/1900-6416765/
- Destructoid, "Review: Tooth and Tail" (9.5/10) — https://www.destructoid.com/reviews/review-tooth-and-tail/
- PC Gamer, "Tooth and Tail review" — https://www.pcgamer.com/tooth-and-tail-review/
- PC Gamer, "Tooth and Tail's singleplayer plays like a bite-sized StarCraft campaign" — https://www.pcgamer.com/tooth-and-tails-singleplayer-plays-like-a-bite-sized-starcraft-campaign/
- Metacritic, "Tooth and Tail" — https://www.metacritic.com/game/tooth-and-tail/
- OpenCritic, "Tooth and Tail" — https://opencritic.com/game/4840/tooth-and-tail
- Austin Wintory (Bandcamp), "Tooth and Tail" 사운드트랙 — https://austinwintory.bandcamp.com/album/tooth-and-tail-2
- DualShockers, "Journey Composer's Tooth and Tail Original Soundtrack..." — https://www.dualshockers.com/tooth-and-tail-soundtrack-digital-physical-journey/
- TV Tropes, "Tooth and Tail (Video Game)" 및 "Characters/ToothAndTail" — 세계관·세력 정리 참고
- Tooth and Tail Wiki (Fandom) — Gristmill, Strategy, Gameplay, Story Mode 문서

---

*본 분석서는 2017년 출시 당시의 영어권 평론·인터뷰·개발 자료를 바탕으로 작성되었으며, 공개되지 않은 정확한 판매량 등 일부 상업 지표는 [추정]으로 명시했다. 인용된 점수·날짜·발언은 위 참고 자료에 근거한다.*
