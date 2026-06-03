# EA Sports WRC (2023) 심층 분석

> 코드마스터스(Codemasters)가 21년 만에 World Rally Championship 공식 라이선스로 돌아온 작품이자, 회사의 간판 자체 엔진 EGO를 버리고 언리얼 엔진으로 갈아탄 첫 레이싱 게임. 그리고 — 출시 1년 반 만에 라이선스가 다시 떠나며 — "코드마스터스가 만든 처음이자 마지막 WRC"가 된 비운의 명작. 《EA Sports WRC》는 시뮬케이드(simcade) 랠리 장르에서 《Dirt Rally 2.0》이 세운 황금률을 계승하면서, 200개가 넘는 스테이지와 직접 차를 설계하는 빌더 모드라는 야심으로 장르의 외연을 넓히려 했다. 본 분석서는 이 게임이 무엇이며, 어떻게 평가받았고, 왜 "위대한 레이싱 게임이 미완성 게임의 껍데기를 뚫고 나오려 애쓰는 작품"이라는 양가적 평가를 받았는지를 영어권 자료를 토대로 종합한다.

---

## 1. 게임 개요

### 기본 정보

- **제목**: 《EA Sports WRC》 (내부적으로는 'WRC 23'으로도 통용)
- **개발사**: Codemasters (영국 Southam·Birmingham 스튜디오, 그리고 Kuala Lumpur 스튜디오)
- **퍼블리셔**: EA Sports (Electronic Arts)
- **출시일**: 2023년 11월 3일 (얼리 액세스/디럭스 에디션은 10월 31일)
- **플랫폼**: PC(Windows), PlayStation 5, Xbox Series X/S
- **장르**: 랠리 레이싱 시뮬레이션(시뮬케이드)
- **엔진**: Unreal Engine 4

### 라이선스의 역사적 무게

이 게임의 정체성을 이해하려면 먼저 라이선스의 계보를 짚어야 한다. 코드마스터스는 1998년 《Colin McRae Rally》로 콘솔 랠리 게임의 표준을 세운 회사다. 그러나 공식 World Rally Championship(FIA WRC) 라이선스는 오랜 기간 다른 손에 있었다 — 2010년대 내내 프랑스 퍼블리셔 Nacon(과거 Bigben Interactive)과 스튜디오 Kylotonn(KT Racing)이 《WRC 5》부터 《WRC Generations》까지 시리즈를 맡았다. 코드마스터스는 그동안 라이선스 없이 《Dirt Rally》(2015), 《Dirt Rally 2.0》(2019)이라는 자체 IP로 "가장 진지한 랠리 시뮬"의 평판을 쌓아왔다.

전환점은 2020년이었다. 코드마스터스가 WRC 라이선스를 (2023년부터 적용되는 조건으로) 따냈고, 거의 동시에 코드마스터스 자체가 Electronic Arts에 인수되었다. 그 결과 탄생한 것이 《EA Sports WRC》다. 위키피디아에 따르면 이 게임은 코드마스터스가 만든 첫 WRC 공식 라이선스 작품이자, 2002년 《Colin McRae Rally 3》 이래로 코드마스터스가 처음 다룬 공식 WRC 라이선스 타이틀에 해당한다. 즉 "랠리 명가가 마침내 공식 챔피언십 간판을 단 작품"이라는 상징성이 출시 전부터 컸다.

### 디렉터·주요 크레딧

- **개발 주체**: Codemasters의 랠리 팀(《Dirt Rally》 계열을 만든 그 조직)
- **게임 디자이너 겸 핸들링 컨설턴트**: Jon Armstrong — 단순한 자문이 아니라 코드마스터스 정직원이자 실제 현역 랠리 드라이버다. EA 공식 소개에 따르면 그는 전 주니어 WRC 드라이버, 현 European Rally Championship(ERC) 드라이버, 그리고 esports WRC 챔피언 출신이다. 게임의 핸들링 모델은 그의 실차 피드백을 반영해 다듬어졌다.
- **시니어 크리에이티브 디렉터**: 인터뷰(GamingBolt, Wccftech 등)에서 엔진 전환의 배경을 설명한 인물로 등장. 자체 EGO 엔진이 한계에 다다랐다고 공개적으로 밝혔다.

### 개발 규모·기술 스택

가장 중요한 기술적 사건은 **엔진 교체**다. 코드마스터스는 2009~2010년부터 《F1》, 《Grid》, 《Dirt》 전 라인업을 자사 EGO 엔진(Codemasters EGO Engine)으로 굴려왔다. 《EA Sports WRC》는 그 EGO를 버리고 Unreal Engine 4를 채택한 코드마스터스 최초의 레이싱 게임이다.

여기서 영어권 보도에 혼선이 있었음을 짚어둔다. 일부 초기 기사(Wccftech, GamingBolt)는 헤드라인에 "UE5"를 썼지만, 위키피디아와 EA 공식 포럼의 개발사 답변, PCGamingWiki 등은 실제 사용 엔진을 **Unreal Engine 4**로 확정한다. 출시 후 개발사는 Lumen·Nanite 같은 UE5 전용 기능을 추가할 계획이 없다고 밝혔는데, 이는 베이스가 UE4임을 방증한다. 즉 보도상의 'UE5'는 "EGO를 버리고 언리얼로 간다"는 사건을 가리킨 부정확한 표현이었고, 실체는 UE4 기반이다.

엔진을 바꾼 이유는 명확하다. 개발진은 인터뷰에서 "EGO로는 우리가 원하는 길이의 스테이지와, 더 크고 시각적으로 풍부한 환경을, 우리가 가진 시간과 인력으로 만들 수 없었다"고 말했다. 언리얼로 옮긴 결과 코드마스터스는 **30km에 달하는 단일 스테이지**를 구현할 수 있었다 — 《Dirt Rally 2.0》 시절의 약 두 배다. 다만 핸들링 감각만큼은 언리얼이 기본 제공하지 않았기에, **물리는 《Dirt Rally 2.0》의 것을 이식한 뒤 거기서 더 정제**하는 방식을 택했다. "환경·비주얼은 언리얼, 물리는 코드마스터스 자산"이라는 하이브리드 구조가 이 게임의 기술적 핵심이다.

---

## 2. 게임 설명: 이 게임이 무엇인가

### 컨셉

《EA Sports WRC》는 FIA World Rally Championship의 2023 시즌을 공식 라이선스로 재현한 랠리 시뮬레이션이다. 서킷 레이싱처럼 여러 대가 동시에 트랙을 도는 종목이 아니라, **드라이버 한 명과 코드라이버(내비게이터) 한 명이 시간을 다투며 자연 지형의 폐쇄 도로(스테이지)를 질주하는** 랠리 특유의 포맷을 따른다. 화면에는 경쟁자가 보이지 않고, 오직 코드라이버의 페이스노트("right 5, don't cut, into left 4 long...")와 나 자신, 그리고 시계만이 있다.

세계관이나 줄거리는 없다. 대신 게임이 파는 것은 **현실의 World Rally Championship 그 자체** — 핀란드의 점프, 모나코의 빙판 산악 타맥, 케냐 사파리 랠리의 거친 흙길, 스웨덴의 눈 덮인 고속 코스 같은 18개 공식 개최지의 지형적 정체성이다. 200개 이상의 경쟁 스테이지, 600km가 넘는 아스팔트·그래블(자갈/흙)·눈길이 콘텐츠의 뼈대다.

### 차량·콘텐츠 구성

위키피디아 기준 총 78대의 랠리카가 수록되었다. 그중 10대가 현행 WRC급(2022년 도입된 하이브리드 Rally1 규격 차량 — M-Sport Ford, Hyundai, Toyota의 머신 포함)이고, 나머지 약 68대가 클래식 랠리카다. 1960~70년대의 Mini, Lancia Stratos, Audi Quattro 같은 그룹 B 전설부터, 1990~2000년대 WRC 황금기의 Subaru Impreza, Mitsubishi Lancer Evolution, Ford Focus RS WRC까지를 아우른다. 이 클래식 라인업은 코드마스터스가 《Colin McRae》 시절부터 쌓아온 랠리 헤리티지를 상기시키는 장치다.

차량 클래스는 현행 챔피언십 구조를 그대로 반영한다.
- **Junior WRC(WRC3)**: 약 215bhp, 약 1,200kg의 입문급
- **WRC2**: 약 280bhp, 챔피언십의 주력 서포트 시리즈
- **WRC(Rally1)**: 1.6L 터보 + 하이브리드 + 첨단 공력으로 합산 약 500bhp의 최상위

### 무드·아트 디렉션·사운드

이 장르 특유의 톤은 "고독한 집중"이다. 외부 시점도 있지만 진정한 경험은 보닛/콕핏 뷰에서 코드라이버 음성에 자신의 목숨을 맡기는 데서 나온다. 언리얼 기반의 환경 묘사는 노면 디테일, 식생, 시간대·날씨에 따른 광원 변화에서 EGO 시절보다 확연히 풍부해졌다. 다만 본 분석서 후반에서 다루듯, 이 향상된 비주얼은 프레임레이트 안정성이라는 대가를 치렀다.

사운드 디자인은 이 장르의 절반을 차지한다. 코드라이버의 페이스노트 콜은 타이밍과 명료함이 생명이고, 머신별 엔진음·자갈이 차체 하부를 때리는 소리·서스펜션이 점프 착지에서 비명을 지르는 소리는 몰입의 핵심이다. EA는 출시 전 마케팅에서 force feedback(포스 피드백) 개선과 함께 오디오의 사실성을 전면에 내세웠다.

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

### 코어 게임플레이 루프

랠리의 모먼트-투-모먼트는 단순하지만 가혹하다. 스테이지가 시작되면 코드라이버가 다가오는 코너의 정보를 미리 읽어준다 — 코너의 방향(left/right), 심각도(1=매우 급함부터 6=거의 직선), 거리, 그리고 "don't cut(안쪽을 깎지 마라)", "into(연속)", "over crest(언덕 너머)" 같은 수식어. 플레이어는 **눈으로 보기 전에 귀로 들은 정보를 신뢰해** 브레이킹 포인트와 라인을 결정한다. 30km짜리 스테이지에서는 이 과정이 12~15분간 끊임없이 이어지고, 단 한 번의 집중력 저하가 리타이어로 직결된다. 이 "긴장의 지속"이야말로 랠리 게임의 본질적 쾌감이자 스트레스다.

### Dynamic Handling System (동적 핸들링 시스템)

게임의 심장은 핸들링이다. 마케팅 명칭은 "Dynamic Handling System". 개발진과 매체 설명에 따르면, 베이스는 《Dirt Rally 2.0》의 물리지만 다음 항목들이 개선·확장되었다.
- **타맥(포장도로) 핸들링** 개선 — 전작에서 자주 지적된 "포장로에서의 둥둥 뜨는 느낌"을 줄였다.
- **포스 피드백** 정교화 (휠 사용자의 노면 정보 전달)
- **공력 시뮬레이션**, **드라이브트레인 관성(drivetrain inertia)**, **점진적 브레이킹(progressive braking)** 등 세부 물리 요소 추가

매체 비교(RacingGames.gg 등)는 두 게임의 감각 차이를 이렇게 요약한다. 《EA Sports WRC》는 좀 더 관대(forgiving)하다 — 브레이킹이나 언덕 정상에서 무게 이동이 느껴지지만 비교적 제어가 쉽다. 반면 《Dirt Rally 2.0》은 차가 더 무겁고 사실적이라, 미끄러짐을 잡거나 내리막에서 정돈하려면 더 애써야 한다. 한편 패드(컨트롤러) 사용 시 타맥에서 너무 민감해 오버스티어가 쉽게 난다는 지적도 있었다.

핵심은 이 핸들링이 **실차 드라이버 Jon Armstrong의 피드백으로 검증**되었다는 점이다. 단순 마케팅 수사가 아니라, 현역·esports 챔피언 출신이 팀 내부에 있어 차량별 거동을 실측 기준으로 다듬었다는 것이 이 게임 신뢰성의 근거다.

### 진행 구조: 모드 구성

**커리어 모드(Career)**가 메인이다. Junior WRC부터 최상위 WRC까지 원하는 클래스로 진입해, **자신의 랠리 팀을 직접 꾸린다** — 팀 브랜딩·이름·컬러를 정하고, Chief Engineer(수석 엔지니어)와 Benefactor(후원자)를 선택한다. 시즌을 치르며 챔피언십을 노리고, 성적과 자원에 따라 팀을 성장시킨다. 다만 이 팀 매니지먼트는 후술하듯 "얕다(shallow)"는 비판을 광범위하게 받았다.

**빌더 모드(Builder)** — 이 게임의 가장 야심찬 신기능이다. 콜린 맥레이가 직접 자신의 랠리카(McRae R4)를 개발했던 실화에서 영감을 받아, 플레이어가 **처음부터 자기만의 랠리카를 설계·제작**한다. 다섯 개 범주(Body Shells 차체, Chassis Placement 섀시 배치, 내·외장 커스터마이징, Livery Creator 도색, 그리고 브레이크·전기계통·배기·서스펜션 등 기계 부품)에서 품질·비용·외형이 다른 부품을 고른다. 특히 **엔진 레이아웃 선택이 무게 배분과 주행 특성에 실제로 영향**을 주고, 예산을 부품의 품질·내구성·튜닝에 어떻게 분배하느냐가 성능을 좌우한다. 제작한 차는 실차 스펙에 맞게 밸런스가 잡혀 Career, Time Trial, Clubs 등에서 쓸 수 있다. 단순 도색 차원의 커스터마이즈를 넘어 "설계 시뮬레이션"을 표방한 점에서 장르 내 차별 요소였다.

**그 외 모드**:
- **Time Trial / Quick Play**: 단발 스테이지·랠리
- **Clubs**: 플레이어가 자신만의 챔피언십·이벤트를 만들어 커뮤니티와 공유하는 비동기 경쟁 시스템
- **Moments**: 실제 WRC 역사·시즌의 명장면을 재현하는 시나리오 챌린지(《F1》 시리즈의 동명 모드 계보)
- **Regularity Rally**: 속도가 아니라 "지정된 평균 속도/시간을 정확히 맞추는" 클래식 랠리 규칙을 재현한 이색 모드
- **멀티플레이어**: 최대 32명 크로스플랫폼 비동기/동기 경쟁

### 라이브 운영·포스트런치 콘텐츠

EA Sports 브랜드답게 시즌 단위 운영을 시도했다.
- **무료 VR 업데이트**(Update 1.8): 2024년 4월 30일, PC(Steam·Epic·EA App)에 무료로 추가. Meta Quest 2/3/Pro, Valve Index, Oculus Rift S/CV1, HTC Vive 등 폭넓은 PC VR 헤드셋을 지원하고 커리어를 포함한 전 모드를 VR로 플레이 가능. 다만 **콘솔(PSVR2 포함)은 미지원**이며 개발사는 콘솔 VR 추가 계획이 없다고 못 박았다.
- **EA Sports WRC 2024 시즌 확장(WRC 24)**: 2024년 10월 8일 유료 DLC로 출시. 2024 시즌 차량과 신규 개최지 **Rally Latvia·Rally Poland** 2곳을 추가했다.

### 난이도·접근성

핸들링 어시스트(ABS·트랙션 컨트롤·스티어링 어시스트 등)와 AI 난이도, 데미지·기계 고장 정도 등을 세분 조절할 수 있어, 패드 입문자부터 풀 시뮬 휠 유저까지 스펙트럼을 흡수하도록 설계되었다. 코드라이버 콜의 빈도·타이밍, 페이스노트 표기 방식도 커스터마이즈 가능하다.

---

## 4. 평가

### 종합 점수

리뷰 애그리게이터 기준 "대체로 호평(generally favorable)"이다. 위키피디아가 정리한 Metacritic 플랫폼별 점수는 다음과 같다.

| 플랫폼 | Metacritic |
|---|---|
| PC | 80 / 100 |
| PlayStation 5 | 77 / 100 |
| Xbox Series X/S | 76 / 100 |

OpenCritic에서는 46개 매체 리뷰 기준 평균 약 78점으로 "Strong" 등급을 받았다. 주목할 점은 **PC가 가장 높고 콘솔(특히 Xbox)이 낮은** 분포인데, 이는 핸들링·콘텐츠 같은 코어는 호평받되 콘솔 성능 안정성이 발목을 잡았음을 시사한다.

### 주요 평론 인용

- **Eurogamer**: 4/5 — 핸들링과 스테이지 품질을 높이 평가.
- **VG247**: 4/5.
- **Hardcore Gamer**: 4/5.
- **Shacknews**: 8/10.
- **IGN**: 6/10 (Series X 기준) — 성능 문제에 강하게 비판적이었고 커리어 모드도 빈약하다고 봤다. 콘솔 점수를 끌어내린 대표적 사례.

평론들이 공유한 결론은 거의 한 문장으로 압축된다 — *"EA Sports WRC feels like a great racing game trying to fight its way out of an unfinished one."*("훌륭한 레이싱 게임이 미완성 게임의 껍데기를 뚫고 나오려 안간힘을 쓰는 느낌이다.") 즉 **운전 그 자체는 동세대 최고의 랠리 경험이지만, 그것을 감싼 커리어·성능·완성도는 거칠다**는 양가적 평가다. RacingGames.gg는 "완전한 기능과 훌륭한 핸들링을 원한다면 올해(2023년) 랠리 게임의 챔피언은 의심의 여지 없이 《EA Sports WRC》지만, PC 유저는 아직 다듬어야 할 기술적 버그가 있음을 알아야 한다"고 평했다.

대표적 비판 인용: *"Despite a responsive driving model and decent rally stages, EA Sports WRC offers an awkward career mode with shallow team management."*("반응성 좋은 주행 모델과 괜찮은 스테이지에도 불구하고, 커리어 모드는 어색하고 팀 매니지먼트는 얕다.") 또 다른 리뷰는 "커리어가 어설프고 다소 짜증스러우며, 연출이 들쭉날쭉하고 무작위 스터터가 끼어든다"고 적었다.

### 상업 지표와 유저 평가

규모 면에서는 EA의 거대 포트폴리오(FY2024 GAAP 순매출 약 76억 달러) 안에서 작은 비중이다. Steam 매출 추정치(steam-revenue-calculator 류, 비공식)는 출시 이후 총매출 약 1,675만 달러, 개발사 추정 순매출 약 494만 달러 수준으로 잡힌다. EA가 별도 판매량 수치를 공식 발표하지는 않았다(이 수치는 비공식 추정이며 콘솔 판매를 포함하지 않는다).

Steam 유저 평가는 누적 약 5,638개 리뷰 중 긍정 58% 수준의 "복합적(Mixed)"으로 보고되었다. 이 평가의 분열은 곧 평론-유저 괴리의 핵심이다 — 핸들링은 칭찬하되, **PC 출시 초기의 셰이더 스터터링·프레임 드랍·VR 부재(초기)·DRM/EA App 강제** 등에 대한 누적된 불만이 유저 점수를 끌어내렸다.

### 수상

위키피디아·BAFTA 자료에 따르면 제20회 British Academy Games Awards(2024)에서 **British Game(영국 게임)** 부문 후보에 올랐다. 대형 GOTY 트로피를 휩쓰는 류의 작품은 아니었으나, 영국 개발 명가의 작품으로서 자국 시상식에서 인정받은 셈이다.

---

## 5. 성공 요인 분석 (핵심)

"성공"의 정의를 어디에 두느냐에 따라 이 게임의 평가는 갈리지만, **장르 팬에게 사랑받고 평론 78~80점대를 확보한** 부분적 성공의 요인은 비교적 명확하다.

### 5-1. 디자인: "랠리는 코드마스터스가 가장 잘한다"는 명성의 계승

가장 결정적인 성공 요인은 **《Dirt Rally 2.0》의 물리를 베이스로 삼은 결정**이다. 코드마스터스의 랠리 핸들링은 이미 장르 최고로 인정받고 있었고, 새 엔진에서 처음부터 물리를 다시 만드는 모험 대신 검증된 자산을 이식·정제했다. 그 위에 실차 드라이버 Jon Armstrong을 팀에 두고 거동을 보정한 것이 신뢰성을 더했다. 평론들이 "주행만큼은 동세대 최고"라고 입을 모은 것은 우연이 아니다.

### 5-2. 콘텐츠 물량과 스테이지 길이라는 차별점

엔진 교체의 실익이 가장 분명히 드러난 지점이 **콘텐츠 규모**다. 18개 공식 개최지, 200개 이상의 스테이지, 600km 이상의 노면, 그리고 최대 30km에 달하는 단일 스테이지 — 이는 《Dirt Rally 2.0》(13개 로케이션, 169 스테이지, 통상 6~10km)을 양적으로 압도한다. 긴 스테이지는 "집중을 오래 유지하는" 랠리 본연의 경험을 강화했고, 공식 라이선스 덕분에 실제 2023 챔피언십의 전 일정을 재현했다는 정통성도 확보했다.

### 5-3. 빌더 모드라는 신선한 후크

직접 랠리카를 설계하는 빌더 모드는 동시기 어떤 랠리 게임에도 없던 신선한 제안이었다. 콜린 맥레이의 실화에 뿌리를 둔 서사적 정당성, 그리고 "내가 만든 차로 챔피언십을 달린다"는 소유감은 마케팅 후크이자 장기 플레이 동기가 되었다. 비록 일부 평론은 깊이가 기대만 못하다고 봤지만, 장르에 새로운 표면적을 더한 시도였다는 점은 분명하다.

### 5-4. 공식 라이선스와 EA Sports 브랜드 파워

코드마스터스가 21년 만에 되찾은 WRC 공식 라이선스, 그리고 EA Sports의 마케팅·유통 인프라는 《Dirt Rally》가 누리지 못한 가시성을 보장했다. EA App·콘솔 스토어 전면 노출, EA Play 구독 편입 등은 장르 코어 너머의 일반 유저까지 끌어들이는 채널이 되었다.

### 5-5. 시장 타이밍

2023년 말은 직접적 경쟁작이 부재한 시기였다. 직전 공식 시리즈인 Kylotonn/Nacon의 《WRC Generations》(2022)와 세대 교체가 맞물렸고, 코드마스터스의 정통성 있는 신작이 "올해 유일하게 진지한 랠리 신작"으로 자리 잡았다. RacingGames.gg가 "올해 랠리 게임의 챔피언은 의심의 여지 없이 이 게임"이라 단언한 배경이다.

---

## 6. 비평적 시각 / 한계 / 논란

### 6-1. 성능 문제 — 가장 치명적인 약점

이 게임을 따라다닌 가장 큰 그림자는 **기술적 완성도**다. PC에서는 셰이더 컴파일에 기인한 **스터터링(stuttering)**이 출시 초기 광범위하게 보고되었다(이후 Unreal PSO 캐싱 도입으로 완화). 고사양 PC(RTX 3090급)에서도 울트라 설정의 특정 스테이지는 40fps대로 떨어졌다는 보고가 있을 만큼 최적화가 무거웠다. 콘솔에서는 Xbox Series X의 화면 찢어짐(tearing)과 스터터가 IGN의 6/10 평가를 끌어낸 직접 원인이었다. 위키피디아의 종합 평가도 "프레임레이트 문제, 특히 Windows에서"를 핵심 단점으로 명시한다. 결국 콘솔 Metacritic이 PC보다 낮은 비대칭은 이 성능 격차의 직접적 결과다.

### 6-2. 얕은 커리어·팀 매니지먼트

복수의 매체가 **커리어 모드의 빈약함**을 지적했다. 팀을 꾸리는 외형은 갖췄지만 매니지먼트의 깊이가 얕고, 진행이 어색하며 연출이 들쭉날쭉하다는 평가다. 빌더 모드라는 신기능에 비해, 그것을 담는 그릇인 커리어의 서사·운영 깊이가 따라오지 못했다는 것이다.

### 6-3. 빌더 모드의 깊이 논쟁

야심찬 빌더 모드도 "기대만큼 깊지 않다"는 양면 평가를 받았다. 차량 거동에 영향을 주는 진짜 설계라기보다, 실차 밸런스에 맞춰 조정된 범위 내의 선택이라는 점에서 시뮬레이션적 자유도에 한계가 있다는 지적이 있었다.

### 6-4. 사임 레이싱 커뮤니티의 "여전히 DR2가 낫다"

가장 흥미로운 논란은 코어 팬덤의 반응이다. OverTake.gg 같은 사임 레이싱 커뮤니티에서는 **스테이지 품질·랠리크로스 부재·성능** 등을 이유로 여전히 《Dirt Rally 2.0》을 선호한다는 목소리가 적지 않았다. "신작이 전작의 시그니처 깊이와 폴리시를 잃었다"는 정서다. 더 길어진 스테이지가 디테일·다양성 면에서 전작의 정교하게 다듬어진 스테이지만 못하다는 역설적 비판도 있었다.

### 6-5. 플랫폼·DRM 마찰

PC 유저층에서는 EA App 강제, 초기 VR 부재(2024년 4월에야 추가), 콘솔 VR 영구 미지원 같은 결정이 불만을 샀고, 이는 Steam 유저 평점의 "Mixed" 기조에 기여했다.

---

## 7. 영향과 유산

### 7-1. 코드마스터스 EGO 시대의 종언과 언리얼 전환

산업적으로 가장 의미 있는 사건은 **코드마스터스가 2009년부터 이어온 EGO 엔진 체제를 끝내고 언리얼로 이행**했다는 점이다. 이는 한 명가의 기술 패러다임 전환이며, 이후 EA 산하 코드마스터스 레이싱 라인업의 방향성을 가늠하는 분기점이었다. 동시에 "검증된 자체 엔진을 버린 첫 작품이 성능 문제로 비판받았다"는 사실은, 레거시 엔진과 범용 엔진 전환의 트레이드오프를 보여주는 업계 사례로 남았다.

### 7-2. "처음이자 마지막" — 라이선스의 이른 종료

이 게임의 유산을 규정하는 결정적 사건은 라이선스의 이른 종료다. 2025년 5월, 코드마스터스/EA가 **향후 WRC 타이틀 개발을 중단**한다고 발표하면서, 《EA Sports WRC》는 코드마스터스가 만든 처음이자 마지막 WRC 게임이 되었다(2024 시즌 확장이 마지막 메이저 업데이트). 곧이어 **WRC 공식 게임 라이선스는 다시 Nacon에게 돌아갔고, Nacon은 2027~2032년 독점권을 확보해 2027년 신작(완전한 리부트)을 예고**했다(VGC, DirtFish, Gamereactor 등 보도). 즉 라이선스는 EA·코드마스터스를 거쳐 단 한 작품 만에 원래 보유자에게 회귀한 셈이다. 사임 레이싱 커뮤니티에서는 "오래 기다린 EA·코드마스터스의 WRC 협업이 단 한 게임으로 끝났다"는 아쉬움이 컸다.

### 7-3. 장르적 의미

그럼에도 《EA Sports WRC》는 **시뮬케이드 랠리 장르에서 '한 게임 안에 최대 콘텐츠 + 빌더라는 신기능 + 검증된 핸들링'을 묶은 레퍼런스**로 남는다. 특히 긴 스테이지·공식 라이선스 풀 시즌 재현·차량 빌더의 조합은, 이후 Nacon의 리부트나 경쟁작이 의식할 수밖에 없는 기준선을 제시했다. 동시에 "코어 주행은 위대했으나 그릇(성능·커리어)이 못 따라간" 사례로서, 범용 엔진 전환기에 기술 부채를 어떻게 관리할지에 대한 반면교사이기도 하다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
|---|---|
| 개발/퍼블 | Codemasters / EA Sports |
| 출시 | 2023년 11월 3일 |
| 플랫폼 | PC, PS5, Xbox Series X/S |
| 엔진 | Unreal Engine 4 (EGO 엔진에서 전환) |
| 수록 차량 | 78대 (현행 WRC급 10대 + 클래식 약 68대) |
| 개최지 | 18개 공식 로케이션 |
| 스테이지 | 200개 이상, 총 600km+ |
| 최장 스테이지 | 약 30km |
| 멀티 | 최대 32인 크로스플랫폼 |
| Metacritic | PC 80 / PS5 77 / XSX 76 |
| OpenCritic | 평균 약 78 ("Strong", 46개 리뷰) |
| Steam 유저 평가 | Mixed (긍정 약 58%, 5,638개 기준) |
| VR | PC VR 무료 추가(2024-04-30), 콘솔 미지원 |
| 유료 확장 | WRC 24(2024-10-08, Rally Latvia·Poland) |
| 라이선스 종료 | 2025년 5월 개발 중단, 2027년부터 Nacon |
| 수상 | 제20회 BAFTA Games Awards British Game 부문 후보 |

### 주요 인터뷰·자료

- 엔진 전환 배경: GamingBolt, Wccftech, RacingGames.gg(EGO 엔진을 떠난 이유), Traxion(언리얼 + DR2 물리 혼합)
- 핸들링 컨설턴트: EA 공식 — Jon Armstrong(현역 ERC 드라이버·esports WRC 챔피언) 소개
- 빌더 모드: EA Help(빌더 가이드), Red Bull(빌더 모드 소개), Insider Gaming, RacingGames.gg
- 라이선스 향방: VGC, DirtFish, Gamereactor, ESPN, TopGear, TheSixthAxis(Nacon 2027 신작·리부트)

### 참고 자료 목록 (영어권 중심)

- [EA Sports WRC — Wikipedia](https://en.wikipedia.org/wiki/EA_Sports_WRC)
- [EA Sports WRC — Metacritic](https://www.metacritic.com/game/ea-sports-wrc/)
- [EA Sports WRC — OpenCritic](https://opencritic.com/game/15766/ea-sports-wrc)
- [Why EA Sports WRC is Ditching Codemasters' EGO Engine — RacingGames.gg](https://racinggames.gg/article/why-ea-sports-wrc-is-ditching-codemasters-ego-engine)
- [EA Sports WRC Devs Explain Why They Switched to UE — Wccftech](https://wccftech.com/ea-sports-wrc-devs-explain-why-they-switched-to-ue5/)
- [Tech Q&A: No Plans to Add Lumen or Nanite — Wccftech](https://wccftech.com/ea-sports-wrc-tech-q-no-plans-to-add-lumen-or-nanite/)
- [Why EA Sports WRC will use Unreal mixed with DiRT Rally physics — Traxion](https://traxion.gg/why-ea-sports-wrc-will-use-unreal-engine-mixed-with-dirt-rally-physics/)
- [EA Sports WRC vs DIRT Rally 2.0 Comparison — RacingGames.gg](https://racinggames.gg/article/ea-sports-wrc-vs-dirt-rally-20-comparison-graphics-cars-stages-audio-handling-career)
- [Why our community still prefers DiRT Rally 2.0 — OverTake.gg](https://www.overtake.gg/news/stages-rallycross-performance-why-our-community-still-prefers-dirt-rally-2-0-over-ea-sports-wrc.2547/)
- [Build your own rally car in EA Sports WRC — Red Bull](https://www.redbull.com/int-en/build-your-own-rally-car-in-ea-sports-wrc)
- [How to play / Builder Mode — EA Help](https://help.ea.com/en/help/wrc/wrc-builder-mode/)
- [Jon Armstrong: WRC driver, esports champion, and EA employee — EA](https://www.ea.com/news/jon-armstrong-wrc)
- [EA Sports WRC VR mode details — Charlie Intel](https://www.charlieintel.com/games/ea-sports-wrc-vr-mode-details-271269/)
- [WRC 2024 Season Expansion 보도자료 — EA Investor Relations](https://ir.ea.com/press-releases/press-release-details/2024/Elevate-Your-Rally-Experience-With-the-EA-SPORTS-WRC-2024-Season-Expansion/default.aspx)
- [WRC rights return to Nacon after EA's Codemasters ends rally game development — VGC](https://www.videogameschronicle.com/news/wrc-rights-return-to-nacon-after-eas-codemasters-ends-rally-game-development/)
- [WRC game license returns to previous developer — DirtFish](https://dirtfish.com/rally/wrc/wrc-game-license-returns-to-previous-developer/)
- [WRC licence goes back to Nacon, new game in 2027 — Gamereactor](https://www.gamereactor.eu/wrc-video-game-licence-goes-back-to-nacon-new-game-in-2027-1549293/)
- [20th British Academy Games Awards — Wikipedia](https://en.wikipedia.org/wiki/20th_British_Academy_Games_Awards)
- [EA Sports WRC — Steam](https://store.steampowered.com/app/1849250/EA_SPORTS_WRC/)

---

*본 분석서는 영어권 매체·공식 자료·커뮤니티 자료를 종합해 작성되었다. 비공식 추정 수치(Steam 매출 추정 등)는 본문에 명시했으며, EA가 별도 공식 판매량을 발표하지 않은 점을 감안해 해석할 것.*
