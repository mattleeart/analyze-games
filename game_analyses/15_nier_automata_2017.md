# NieR: Automata (2017) 심층 분석서

> "Everything that lives is designed to end." (살아 있는 모든 것은 끝나도록 설계되어 있다.) — 게임 오프닝 내레이션

/ 한 줄 요약: 폐허가 된 라이선스 의존 액션 스튜디오와 컬트 작가가 손잡고, "한 번의 엔딩으로 끝나지 않는 게임"이라는 도박을 통해 1,000만 장의 메인스트림 히트이자 게임을 예술로 끌어올린 21세기 대표작을 만들어낸 사례.

---

## 1. 게임 개요

### 기본 정보
- **개발사:** PlatinumGames (플래티넘게임즈)
- **퍼블리셔:** Square Enix (스퀘어 에닉스)
- **장르:** 액션 RPG (핵 앤 슬래시 + 슈팅 + 장르 혼합)
- **플랫폼별 출시일** (출처: Wikipedia "Nier: Automata"):
  - PlayStation 4 — 일본: 2017년 2월 23일 / 북미: 2017년 3월 7일 / PAL: 2017년 3월 10일
  - Windows(Steam) — 2017년 3월 17일
  - Xbox One("Become as Gods Edition") — 2018년 6월 26일
  - Nintendo Switch("The End of YoRHa Edition") — 2022년 10월 6일

### 주요 크레딧
- **디렉터/메인 시나리오:** Yoko Taro (요코 타로). 시리즈 크리에이터로서 디렉터 겸 주 각본가를 맡았다.
- **프로듀서:** Yosuke Saito (요스케 사이토, Square Enix), Eijiro Nishimura (니시무라 에이지로)
- **리드 작곡가:** Keiichi Okabe (오카베 케이이치, 스튜디오 MONACA)
- **캐릭터 디자인:** Akihiko Yoshida (요시다 아키히코, Final Fantasy 시리즈 등으로 유명)
- **게임 디자인:** Takahisa Taura (타우라 타카히사, 액션·전투 시스템 총괄), Isao Negishi (네기시 이사오, RPG 요소 담당)
- **영어 로컬라이제이션:** 8-4 (전작 NieR 로컬라이징을 담당했던 동일 업체)

### 개발 규모와 기간
- 개발은 **2014년 시작**, 약 **6개월의 프리프로덕션**을 거쳤다 (출처: Wikipedia).
- 본작은 PlatinumGames가 처음 시도한 **오픈월드이자 첫 RPG 협업 프로젝트**였다.
- 흥미롭게도 기획 초기에는 PlayStation Vita용 **"FarmVille에서 영감을 받은" 모바일성 타이틀**로 구상되었다가 PS4 개발로 방향을 틀었다 (출처: Wikipedia).
- 요코 타로는 PlatinumGames와 직접 협업하기 위해 도쿄에서 오사카로 거처를 옮겼다.
- 각본은 요코 타로의 작품 중 가장 많은 작업량을 요구했으며, 스토리 자체는 개발 중 큰 변화가 없었으나 최종 완성은 예정보다 약 5개월 지연되었다 (출처: Wikipedia, SuperJump 인터뷰).
- 정확한 예산 수치는 공식적으로 공개된 바 없다. [확인된 예산 자료 없음]

### 엔진/기술 스택
- 게임 엔진은 PlatinumGames가 자사 액션 게임에 사용해 온 사내 기술 기반으로 구동되며, Square Enix가 추가 인력과 사운드 디자인으로 프로젝트를 지원했다. PlatinumGames가 핵심 개발을 전담했다.
- Switch 이식은 **Virtuos**가 담당했으며, 프레임레이트를 30fps로 제한하되 다른 버전과 장면별 시각적 동일성을 유지했다 (출처: Wikipedia).

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 컨셉과 세계관
NieR: Automata는 **서기 11945년**을 배경으로, 인류가 만든 안드로이드와 외계 침략자가 만든 기계생명체(Machines) 사이의 **대리전(proxy war)**을 그린다 (출처: Wikipedia, NIER Wiki). 게임은 이른바 "14번째 기계 전쟁(14th Machine War)" 시점에서 시작된다.

배경 설정의 핵심 구조는 다음과 같다 (출처: NIER Wiki "YoRHa", Wikipedia "Machines"):
- 정체불명의 외계 종족이 1차 기계 전쟁 당시 지구의 안드로이드를 전멸시키기 위해 **기계생명체**를 만들었고, 이들은 전 세계 통신 네트워크로 연결되어 있다.
- 그러나 기계들은 점차 자신의 프로그래밍에 의문을 품고 창조자에게 반기를 들어 **외계인을 멸종**시킨다. 이후 네트워크에서 분리되어 인간의 행동·문화·감정을 모방하며 자신의 존재 의미를 찾기 시작한다.
- **YoRHa**는 "인류 평의회(Council of Humanity)"를 섬기고 지구를 외계인과 기계로부터 탈환한다는 명목으로 만들어진 정예 안드로이드 군대로, 위성 궤도의 **벙커(Bunker)**를 거점으로 사령부의 지휘를 받는다.

### 줄거리 (스포일러 포함)
**[스포일러]** 본작 세계관의 핵심 진실은 충격적이다 (출처: Wikipedia, NIER Wiki):
- **인류 평의회는 실제로 존재하지 않으며, 인류는 외계인이 지구에 도착하기 전에 이미 Project Gestalt의 실패로 멸종했다.** 달에 인류가 생존해 있다는 거짓 서사가 만들어졌고, 안드로이드들의 사기 유지를 위해 이 거짓을 퍼뜨릴 정예 부대(YoRHa)가 설계되었다.
- 즉 안드로이드와 기계는 **이미 사라진 두 창조주(인류와 외계인)를 위해 무의미한 전쟁을 끝없이 반복**하는 존재들이다. 이 설정 위에서 "존재의 의미"라는 게임 전체의 주제가 작동한다.

### 다회차 구조와 주요 엔딩 (게임 정체성의 핵심)
NieR: Automata는 **한 번의 플레이로 끝나지 않는** 게임이다. 핵심 엔딩 A~E를 모두 봐야 비로소 전체 이야기가 완성되며, 이외에도 알파벳 F~Z에 해당하는 21개의 단편 엔딩(대부분 의도적 게임오버성 농담 엔딩)을 합해 **총 26개의 엔딩**이 존재한다 (출처: Wikipedia).

- **엔딩 A (루트 A):** 주로 전투형 안드로이드 **2B**의 시점으로 메인 스토리를 1회차 완주한다. 동료 정찰병 **9S**와 함께하지만 일부 구간에서 분리된다 (출처: ScreenRant, Twinfinite, Fextralife).
- **엔딩 B (루트 B):** 동일한 사건을 이번엔 **9S의 시점**으로 재경험한다. 9S의 특기인 "해킹"을 통해 전투로는 보이지 않던 진실이 드러난다 — 같은 사건의 반복이 아니라 **새로운 정보 레이어**다.
- **엔딩 C / D (루트 C):** 루트 A·B 이후의 최종 국면. 로직 바이러스에 감염되어 광기에 빠진 9S가 **A2**에게 결투를 걸고, 플레이어는 둘 중 하나를 선택한다. **A2를 선택하면** A2가 9S를 구하고 자신을 희생해 타워를 파괴한다(엔딩 C). **9S를 선택하면** 두 안드로이드가 서로를 죽이며, 9S는 평화로워진 기계 네트워크에 합류하라는 제안을 받는다(엔딩 D).
- **엔딩 E ("진엔딩"):** C와 D를 모두 본 뒤, 크레딧 도중 동료 보조 로봇 **포드(Pod 042, Pod 153)**가 대화를 시작한다. 이들의 최종 명령은 2B, 9S, A2를 포함한 모든 YoRHa 데이터의 삭제였으나, 포드들은 **프로그래밍을 거부하고** 안드로이드들의 데이터를 복원해 그들에게 새로운 삶의 기회를 주기로 한다. 코드 어디에도 그렇게 하라고 적혀 있지 않은데도. (출처: ScreenRant, Medium "Endings C, D, and E")

**[스포일러] 엔딩 E의 슈팅 게임과 세이브 삭제:** 엔딩 E는 단순한 영상이 아니라 크레딧을 배경으로 펼쳐지는 극악한 슈팅 미니게임이다. 플레이어가 거듭 실패하면, 전 세계 다른 플레이어들이 남긴 응원 메시지와 함께 그들의 데이터가 화면에 합류해 함께 싸운다("다른 사람들의 희생 위에 도달하는 결말"). 그리고 클리어 후 게임은 플레이어에게 **자신의 세이브 데이터를 삭제해 다른 누군가를 돕는 데 바칠 것인지** 묻는다. 이는 전작 NieR의 "세이브 삭제 진엔딩" 전통을 계승·확장한 요코 타로 특유의 메타적 장치다 (출처: Game Informer 인터뷰, PC Gamer 인터뷰).

### 캐릭터
- **2B (YoRHa No.2 Type B):** 과묵하고 전투에 특화된 안드로이드. 영어판에서는 "무감정"이 아니라 "건조한(droll)" 톤으로 재해석되었다 (출처: Wikipedia, 8-4 로컬라이징).
- **9S (YoRHa No.9 Type S):** 정찰·해킹 특화 유닛. 호기심 많고 감정적이며, 이야기가 진행될수록 가장 비극적인 궤적을 그린다.
- **A2 (YoRHa Type A No.2):** 루트 C/D에서 비중이 커지는 구형 프로토타입 안드로이드.
- 그 외 **Pod 042/153**(보조 로봇), 사령관(Commander), 거대 가수형 기계 **Simone(시몬)** 등. 요코 타로는 시몬을 "플레이어가 도저히 공감할 수 없도록" 디자인했다고 밝혔다 — 시체로 자신을 치장하고 한 남자에게 헌신하는 캐릭터로(출처: PC Gamer 인터뷰).
- **Jean-Paul:** 사이드 퀘스트에 등장하는 기계로, 철학자 **장폴 사르트르**에서 이름을 땄다. 원래 "Sartre"였으나 사르트르 재단의 저작권 문제로 "Jean-Paul"로 변경되었다. "실존은 본질에 앞선다(Existence precedes essence)"는 명제를 직접 읊는다 (출처: Wikipedia, 철학 분석 자료).

### 무드/톤/아트 디렉션
멸망 이후의 폐허(폐허가 된 도시, 유원지, 사막, 침수 지대)를 무대로 한 우울하고 멜랑콜리한 톤이 지배적이다. 요시다 아키히코의 캐릭터 디자인은 단정한 고딕풍 의상의 안드로이드와 녹슨 기계생명체의 대조를 통해 "인간을 흉내 내는 비인간"이라는 주제를 시각화한다.

### 사운드/음악
오카베 케이이치가 그의 스튜디오 밴드 **MONACA**(Keigo Hoashi, Kuniyuki Takahashi 등)와 함께 음악을 총괄했다 (출처: Wikipedia "Music of Nier", PlayStation Blog). 보컬은 **Emi Evans**가 주축이며, 가상의 인공 언어(소위 "카오스 언어")로 노래해 시대를 초월한 비현실감을 자아낸다.
- 대표곡 **"Weight of the World"**는 오카베 작곡으로, 엔딩 E에서 흐르는 게임의 상징적 테마다. 일본어·영어·자작 언어 버전이 존재하며, NieR:Automata 발매 홍보를 위해 Final Fantasy XV의 인게임 음악 플레이어에 수록되기도 했다 (출처: Wikipedia "Music of Nier").
- 사운드트랙에는 동적 음악 시스템이 적용되어, 9S가 적을 해킹해 미니게임에 진입하면 같은 곡이 **8비트 칩튠 버전("Hacking Tracks")으로 변형**된다. 사운드트랙 초판에는 16곡의 보너스 해킹 트랙 변주가 포함되었다 (출처: Wikipedia).

---

## 3. 핵심 시스템 / 메카닉

### 코어 게임플레이 루프
NieR: Automata는 PlatinumGames의 장기인 **실시간 핵 앤 슬래시**를 기반으로 한다 (출처: Wikipedia, Fextralife "Combat"). 모먼트-투-모먼트의 골격은 다음과 같다:
1. **근접 공격:** 약공격/강공격을 조합한 콤보. 무기는 **단검(short swords), 장검(long swords), 건틀릿(bracers), 창(spears)**의 4개 클래스로 나뉘며, 두 종류의 무기를 세팅해 "약-강" 슬롯에 배정할 수 있다.
2. **회피:** 적의 공격을 정확한 타이밍에 회피하면 무적 프레임 또는 반격 보너스를 얻는다(퍼펙트 닷지). 베요네타의 "위치 타임"에 대응하는 핵심 방어 메카닉.
3. **포드(Pod) 원거리 공격:** 비행 보조 로봇 포드가 커스터마이즈 가능한 원거리 공격을 발사한다. **머신건 / 레이저 / 호밍 미사일**의 세 가지 타입이 있으며, 본작 데미지의 상당 부분이 포드 사격에서 나온다 (출처: Fextralife, Steam).

### 장르 혼합과 시점 전환 — 본작의 진짜 정체성
요코 타로/PlatinumGames는 슈팅 요소를 **탄막(bullet hell) 게임에서 차용**했고, 전투에 다중 카메라 시점을 의도적으로 도입했다 (출처: Wikipedia). 그 결과:
- **3인칭 액션**이 기본이지만, 구간에 따라 갑자기 **탑다운 슈팅, 횡스크롤(2D), 종스크롤 슈팅**으로 카메라와 장르가 전환된다.
- 비행 유닛 구간에서는 본격 **슈팅 게임(슈뮤)**이 되며, 일부 시퀀스는 **텍스트 어드벤처**로 진행되기도 한다.
- 이 끊임없는 장르 변주가 "한 게임 안에 여러 게임이 들어 있다"는 본작 특유의 감각을 만든다.

### 9S의 해킹 시스템
두 번째 주인공 9S는 약공격과 **해킹**을 조합한다 (출처: Wikipedia, Fextralife). 적을 해킹하면 **탑다운 트윈스틱 슈팅 미니게임**에 진입하고, 짧은 시간 안에 클리어하면 적을 폭발시키거나 일시적으로 아군화할 수 있다. 루트 B(9S 시점)에서는 이 해킹을 통해 적과 환경의 숨은 텍스트·진실이 노출되어 같은 사건을 전혀 다른 정보량으로 재서술한다.

### 칩(Plug-in Chip) 시스템 — 본작의 자원 관리/경제
플레이어는 안드로이드의 능력을 **플러그인 칩**으로 커스터마이즈한다 (출처: Fextralife, Neoseeker, Fandom "Plug-in Chips"). 핵심은 다음과 같다:
- 칩은 데미지 증가, 아이템 드롭 증가, 방어·회피 강화, 특수 능력 부여 등 다양한 퍽을 제공한다.
- 모든 칩은 **메모리 용량**을 차지하며, 캐릭터가 보유한 총 메모리 한도 내에서만 장착할 수 있어 빌드 선택을 강제한다.
- **[스포일러] OS 칩:** 가장 메타적인 요소는 HP 게이지·미니맵·경험치 표시 같은 **UI 자체도 칩**으로 구현되어 있다는 점이다. UI 칩을 빼면 화면이 비워지지만 메모리에 여유가 생긴다. 그리고 절대 빼서는 안 되는 "OS 칩"을 일부러 제거하면 즉시 게임오버되고 농담 엔딩 하나가 잠금 해제된다. UI를 게임 메카닉이자 서사 장치로 끌어들인 디자인이다.

### 진척도/사망 시스템
- 경험치를 얻으면 체력·방어·공격력이 상승한다 (출처: Wikipedia).
- 캐릭터가 사망하면, 다크 소울식으로 **이전 시체가 필드에 남아** 회수 시 보너스를 되찾거나, 시체를 수리·재가동해 일시적 아군으로 부릴 수 있다.
- 4단계 난이도(Easy~Very Hard)가 제공되며, Easy에서는 **Auto-fight/Auto-evade/Auto-Pod 칩**으로 거의 자동 전투가 가능해 스토리만 즐기려는 플레이어를 위한 접근성 옵션을 보장한다 (출처: Wikipedia).

### UI/UX 디자인 철학
앞서 언급한 "UI=칩" 구조가 핵심이다. 일반적인 게임에서 HUD는 시스템 영역이지만, 본작은 이를 **세계관 내 안드로이드의 OS**로 통합해 "당신이 보는 화면 정보조차 한 기계의 인지"라는 메타픽션을 구축한다. 이는 요코 타로가 일관되게 추구해 온 "게임 디자인 관습 자체를 비평하는" 태도의 연장이다.

### 멀티 / 라이브 운영
본작은 본질적으로 **싱글플레이 작품**으로, 시즌패스나 상시 라이브 운영 모델을 채택하지 않았다. 다만 엔딩 E의 "다른 플레이어 데이터가 합류·세이브 희생"이라는 비동기적 상호작용이 유일한 온라인 요소다. 사후 DLC로 콜로세움 콘텐츠 **"3C3C1D119440927"**(2017)이 추가되었다.

---

## 4. 평가

### Metacritic / 평론 점수
플랫폼별 Metacritic 메타스코어 (출처: Metacritic, Wikipedia):
- **PS4: 88/100** (107개 리뷰)
- **PC: 84/100** (14개 리뷰) — PC 포트 기술 문제가 점수에 반영
- **Xbox One(Become as Gods): 90/100** (30개 리뷰)
- **Nintendo Switch: 89/100** (35개 리뷰)

주요 매체 개별 점수 (출처: Wikipedia, Metacritic):
- **Famitsu: 39/40** (일본 평단 최상위권)
- **GameSpot: 9/10**
- **IGN: 8.9/10**
- **Destructoid: 9/10**
- **GamesRadar+: 4.5/5**
- **Eurogamer: "Recommended"**
- **Game Informer: 7.75/10** (상대적으로 낮은 점수 — 사이드퀘스트의 반복적 심부름, PlatinumGames 기준 미흡한 액션 깊이 등을 지적)
- **Nintendo World Report: 10/10** (Switch판)

대표적 평론 인용 (출처: Metacritic 종합):
> "NieR: Automata is the rare gaming experience in which narrative, aesthetics, and gameplay all complement each other to form a perfect storm of master class game design. A truly exemplary example of what video games are capable of as an art form." (서사·미학·게임플레이가 서로를 보완해 마스터클래스급 게임 디자인의 완벽한 폭풍을 이루는, 비디오게임이 예술로서 무엇을 할 수 있는지 보여주는 모범 사례.)

### 수상 이력
- **The Game Awards 2017:** Best Score/Music **수상**, Best Narrative·Best RPG **노미네이트** (출처: The Game Awards, IMDb)
- **D.I.C.E. Awards 2018:** Role-Playing Game of the Year **수상**
- **SXSW Gaming Awards 2018:** Excellence in Musical Score, Excellence in Technical Achievement **수상**
- **Game Developers Choice Awards 2018:** Audience Award **수상**
- **BAFTA Games Awards:** Game Innovation, Game Design 부문 **2개 노미네이트** (출처: Steam News, BAFTA)
- **Japan Game Awards:** Award for Excellence **수상**
- **NAVGTR:** Camera Direction in a Game Engine, Original Dramatic Score (Franchise) 수상

### 상업 지표 (시간대별 판매 추이)
출처: Wikipedia, Gematsu, Square Enix 공식 발표, Statista
- 발매 첫 주(일본): 198,500장 이상
- 2017년 4월: 50만 장 돌파(일본·아시아 합산)
- 2017년 5월: 150만 장(PS4+PC)
- 2019년 5월: **400만 장** 돌파(전 세계)
- 2020년 3월: 450만 장
- 2024년 2월: 800만 장
- 2024년 12월: **900만 장** 돌파 (Square Enix 공식 발표)
- 2026년 2월(초): **1,000만 장** 돌파

→ 800만에서 900만까지 약 10개월 걸린 점에서 보듯, 발매 후 9년이 지나도록 **롱테일로 꾸준히 판매**되는 보기 드문 작품이다. Square Enix는 본작의 성과가 "회사의 판매 기대치를 크게 초과했다"고 밝혔다 (출처: Wikipedia).

### 유저 평가
- **Steam:** 누적 리뷰 약 149,755개 중 130,792개가 긍정(부정 18,963개)으로 "Very Positive", 플레이어 스코어 87/100 (출처: Steambase). 커뮤니티 허브 팔로워 약 514,600명으로 강력한 팬덤을 보유.
- 평론과 유저 평가 모두 매우 높지만, **PC판은 별도의 논란**이 있었다(아래 6장 참조).

### 평론-유저 괴리
순수 콘텐츠 측면에서는 평론과 유저 모두 극찬으로 일치한다. 다만 **기술적 완성도(특히 PC 포트)**와 **사이드퀘스트의 반복적 동선** 측면에서 일부 유저·평론(Game Informer 등)의 점수가 다른 매체보다 낮게 형성된 지점이 존재한다.

---

## 5. 성공 요인 분석

### (1) 디자인 측면 — "다회차를 강제가 아닌 보상으로"
본작의 가장 큰 성공 요인은 **다회차 구조를 단순 반복이 아니라 서사적 재발견으로 설계**한 점이다. 루트 B는 같은 사건을 9S의 해킹 시점으로 재서술해 새로운 정보를 주고, 루트 C는 완전히 새로운 후속 서사로 진입한다. "엔딩 A가 끝이 아니라 시작"이라는 구조가 입소문(word of mouth)을 폭발시켰다 — "끝까지 가봐야 진짜를 안다"는 메시지가 커뮤니티 전파의 동력이 되었다.

### (2) 두 강점의 결합 — 작가성 × 액션 장인
NieR(2010)는 강한 작가성·음악·세계관을 가졌으나 전투가 약했고, PlatinumGames는 Bayonetta·Metal Gear Rising: Revengeance로 최고의 액션을 만들었으나 서사가 약했다 (출처: Wikipedia, Game Informer). 두 진영이 각자의 약점을 상대의 강점으로 메우는 **상호 보완적 협업**이 본작의 본질적 성공 요인이다. Square Enix와 NieR 핵심 스태프가 "더 액션 지향적인 NieR"을 원해 PlatinumGames에 직접 접촉한 것이 출발점이었다.

### (3) 개발 방법론 — 절박함이 만든 도박
- 디자이너 **Takahisa Taura는 전작 NieR의 팬으로서 먼저 Square Enix에 "제발 속편을 만들게 해 달라"고 요청**했다 (출처: GodisaGeek 인터뷰). 그는 "Nier를 너무 사랑해서 직접 찾아갔다"고 회고한다.
- 프로듀서 **Saito는 "이 프로젝트를 못 하게 하면 회사를 그만두겠다"**고 강하게 밀어붙여 기획을 성사시켰다 (출처: USgamer/Game Developer 포스트모템).
- 즉 본작은 시장 분석으로 기획된 안전한 프로젝트가 아니라, **개인들의 절박한 의지로 떠밀린 도박**이었다. 요코 타로는 GDC 포스트모템에서 개발이 "성공이라기보다 지옥에 가까웠다"고 표현했다.

### (4) 음악과 분위기 — 정서적 각인
오카베 케이이치의 사운드트랙은 단순 BGM을 넘어 게임 정체성의 절반이다. The Game Awards Best Music 수상이 이를 공인했고, "Weight of the World"는 게임을 넘어선 문화적 곡이 되었다. 음악만으로 게임을 기억하고 재구매하는 팬층을 만들었다.

### (5) 캐릭터 IP의 폭발력
2B는 발매 직후부터 거대한 코스프레·팬아트·밈 현상을 일으켰고, 이 시각적 임팩트가 NieR을 컬트에서 메인스트림으로 끌어올린 마케팅 동력이 되었다. Soulcalibur VI(2018), Final Fantasy XIV: Shadowbringers의 YoRHa 레이드, 그리고 2026년 Overwatch 콜라보까지 이어지는 크로스오버가 IP의 생명력을 증명한다 (출처: Wikipedia).

### (6) 동시기 작품 대비 차별점
2017년은 Horizon Zero Dawn, The Legend of Zelda: Breath of the Wild, Persona 5 등 대작 RPG가 쏟아진 해였다. 그 사이에서 NieR: Automata는 **"철학적 메타픽션 + 장르 혼합 액션"이라는 어떤 경쟁작과도 겹치지 않는 포지션**으로 차별화에 성공했다. 누구도 흉내 낼 수 없는 작가성이 곧 해자였다.

---

## 6. 비평적 시각 / 한계 / 논란

### (1) 액션 게임으로서의 한계
PlatinumGames의 명성을 감안하면, 일부 평론은 본작의 전투가 "견고하지만 제한적(solid but limited)"이라고 평했다. 베요네타나 Metal Gear Rising만큼의 깊은 콤보·메카닉 숙련 곡선이 없다는 지적이다 (출처: 평론 종합). 본작은 액션의 깊이보다 **장르 혼합과 서사 전달**을 우선했기에 발생한 트레이드오프다.

### (2) 사이드퀘스트와 동선 문제
- 다수 퀘스트가 **목표 마커까지 장거리를 왕복**하는 심부름성 구조다.
- **패스트 트래블이 게임 중반에야 해금**되어 초반의 이동 피로도가 크다 (출처: ResetEra 토론, GamesRadar).
- 다만 평론·유저 다수는 이 퀘스트들의 **이야기 자체는 세계관과 캐릭터를 깊게 들여다보게 하는 보석**이라고 평가한다 — 메인 스토리가 어둡고 무거운 반면 사이드퀘스트는 더 인간적인 단면을 보여준다.

### (3) PC 포트 논란 (가장 큰 운영 이슈)
2017년 3월 Windows판은 심각한 기술 문제를 안고 출시되었다 (출처: TheGamer, Steam 커뮤니티):
- 프레임레이트가 사실상 고정되고, 풀스크린·해상도·UI 스트레칭 버그가 만연했으며, 키보드·마우스 조작이 부자연스러웠다.
- 팬들은 비공식 패치(소위 **"FAR" 등의 팬 픽스**)에 의존해야 했다.
- Square Enix는 **약 4년 뒤인 2021년 7월에야 공식 패치**(Windows Store/Microsoft 협업판)를 내놓았다 (출처: Wikipedia, TheGamer). "AAA 게임이 표준 성능과 정상적 마우스·키보드 조작을 위해 모드를 강요해선 안 된다"는 비판이 거셌다.
- 이 사건은 이후 Steam에서 **리뷰 폭격(review-bombing)**의 빌미가 되기도 했다 (출처: GamesRadar, NME).

### (4) 평가가 갈리는 지점
- "다회차 강제"를 두고, 다수는 "필수적 서사 장치"로 옹호하지만 일부는 "1회차 후 반복 피로"를 호소한다.
- 요코 타로의 의도적 "스트레스 유발 디자인"(세이브 삭제, 극악 슈팅 등)에 대해서도 "예술적 도전"과 "불친절한 과시"로 평가가 나뉜다. 요코 본인은 "다른 개발자들이 이미 만족스러운 게임을 만들고 있으니, 나는 스트레스를 줘도 괜찮다"고 말했다 (출처: Game Informer 인터뷰).

---

## 7. 영향과 유산

### 장르·산업적 영향
- NieR: Automata는 **"중견 규모의 작가주의 일본 액션 RPG도 글로벌 메인스트림 히트가 될 수 있다"**는 것을 증명했다. 이는 이후 일본 단일 비전형 프로젝트(예: Square Enix 내부의 다양한 실험작들)에 대한 투자 정당성을 강화했다.
- **PlatinumGames의 회생작:** 본작 직전 PlatinumGames는 Wii U 독점의 Bayonetta 2(2014)와 혹평받은 Star Fox Zero(2016) 사이에서 라이선스 게임을 만들며 부진했다. NieR: Automata는 이 스튜디오의 평판과 사기를 되살린 결정적 전환점이었다 (출처: USgamer 포스트모템 분석). 본작의 디자인 노하우는 PlatinumGames의 후속작 **Astral Chain(2019)**으로 이어졌다(타우라가 디렉터).
- 게임 디자인 담론에서 본작은 **"UI·세이브·크레딧 같은 메타 레이어를 서사에 통합한 사례"**의 교과서가 되었다. 엔딩 E의 "타인의 희생으로 도달하는 결말"은 비동기 멀티플레이의 정서적 활용 사례로 자주 인용된다.

### 후속·확장
- **애니메이션:** A-1 Pictures 제작 "NieR:Automata Ver1.1a"가 2023~2024년 방영 (출처: Wikipedia).
- **소설·만화·연극:** Jun Eishima의 소설 시리즈, 만화 "YoRHa Pearl Harbor Descent Record", 그리고 요코 타로가 본편보다 먼저 만든 무대극 **YoRHa**(2014)가 세계관 전사를 이룬다.
- **크로스오버:** Soulcalibur VI(2B DLC, 2018), Final Fantasy XIV: Shadowbringers의 "YoRHa: Dark Apocalypse" 레이드, Overwatch 콜라보(2026) 등.

### 문화적·학술적 의미
- 본작은 **알베르 카뮈의 부조리주의("시지프 신화")**, 실존주의, 니힐리즘, 페미니즘 이론 등 철학을 직접 텍스트로 끌어들였다 (출처: 다수 철학 분석, scholarworks.uni.edu 논문). "Everything that lives is designed to end"로 시작하는 니힐리즘적 전제를 깔되, **엔딩 E를 통해 "그럼에도 의미를 만들어내는 togetherness(함께함)"**라는 반(反)니힐리즘적 결론으로 자기 메시지를 전복한다.
- 사르트르의 "실존은 본질에 앞선다", "Jean-Paul" 캐릭터 등은 게임이 철학 텍스트를 진지하게 다룬 사례로 학계(루도뮤지콜로지 포함)에서 연구 대상이 되었다.
- 2B를 비롯한 캐릭터는 게임 외부에서 거대한 팬덤·코스프레·밈 문화를 형성하며, NieR을 단순한 게임을 넘어선 **하나의 문화 현상**으로 끌어올렸다.

---

## 8. 부록

### GDC 강연 / 포스트모템
- **GDC 포스트모템:** "Yoko Taro and Platinum Games' postmortem of Nier: Automata" — Game Developer(구 Gamasutra)
  - https://www.gamedeveloper.com/design/video-yoko-taro-and-platinum-games-postmortem-of-i-nier-automata-i-
  - 요약 기사: "It Felt More Like Hell Than Success: A Nier: Automata Postmortem" (USgamer) — https://captionit.co/articles/nier-automata-postmortem-yoko-taro-platinumgames
  - 핵심: 요코 타로가 출근 시간(9:30) 문제로 한 달간 갈등하다 프로젝트가 취소 직전까지 갔고, 자신이 "거의 해고될 뻔했다"고 회고. Saito 프로듀서가 그를 붙잡았다.

### 주요 인터뷰
- Game Informer, "Nier's Yoko Taro On Success, Drinking, And Death" (2017.11) — https://gameinformer.com/b/features/archive/2017/11/24/yoko-taro-nier-automata-interview-game-informer.aspx
- Game Informer, "Talking To Yoko Taro, PlatinumGames' Takahisa Taura, And Composer Keiichi Okabe About Life, Death, And Opportunity" (2019.01)
- PC Gamer, 요코 타로 인터뷰 (Simone·Sartre 설계 의도, "내가 파악하기 어려운 이야기를 만들고 싶었다") — https://www.pcgamer.com/games/yoko-taro-wanted-nier-automata-to-be-a-story-id-have-trouble-grasping-myself...
- GodisaGeek, "An interview with Taro Yoko, Yosuke Saito and Takahisa Taura" (2017.02) — https://godisageek.com/2017/02/nier-automata-interview-yosuke-saito-takahisa-taura/
- PlayStation Blog, "One Year Later, Composer Keiichi Okabe Looks Back at Nier:Automata" (2018.03) — https://blog.playstation.com/2018/03/07/one-year-later-composer-keiichi-okabe-looks-back-at-nierautomata/
- SuperJump, "An Interview with Yoko Taro, Yosuke Saito, and Keiichi Okabe" — https://www.superjumpmagazine.com/nier-automata-switch-interview-with-yoko-taro-yosuke-saito-and-keiichi-okabe/

### 핵심 통계 표

| 항목 | 내용 | 출처 |
|---|---|---|
| 디렉터 | Yoko Taro | Wikipedia |
| 개발사 / 퍼블리셔 | PlatinumGames / Square Enix | Wikipedia |
| 개발 시작 | 2014년 (프리프로덕션 6개월) | Wikipedia |
| PS4 출시 | 2017.02.23(일) / 03.07(북미) | Wikipedia |
| PC(Steam) 출시 | 2017.03.17 | Wikipedia |
| Switch 출시 | 2022.10.06 | Wikipedia |
| Metacritic PS4 | 88/100 (107 리뷰) | Metacritic |
| Metacritic Xbox One | 90/100 (30 리뷰) | Metacritic |
| Metacritic PC | 84/100 (14 리뷰) | Metacritic |
| Famitsu | 39/40 | Wikipedia |
| 누적 판매 | 1,000만 장 이상(2026.02 기준) | Square Enix / Wikipedia |
| The Game Awards 2017 | Best Score/Music 수상 | The Game Awards |
| D.I.C.E. 2018 | RPG of the Year 수상 | Wikipedia |
| Steam 유저 평가 | "Very Positive" (약 87/100) | Steambase |
| 메인 엔딩 / 총 엔딩 | A~E(5개) / 26개 | Wikipedia |
| PC 공식 패치 | 2021년 7월(발매 4년 후) | Wikipedia / TheGamer |

### 참고 자료 목록 (영어권 매체 중심)
- Wikipedia — "Nier: Automata", "Music of Nier", "Machines (Nier: Automata)", "Keiichi Okabe", "Yoko Taro" — https://en.wikipedia.org/wiki/Nier:_Automata
- Metacritic — NieR: Automata (플랫폼별) — https://www.metacritic.com/game/nier-automata/
- Gematsu — "NieR: Automata shipments and digital sales top nine million" (2024.12) — https://www.gematsu.com/2024/12/nier-automata-shipments-and-digital-sales-top-nine-million
- Square Enix Asia Newsportal — "NieR:Automata Surpassed 9 Million Units" — https://www.square-enix.com/asia/newsportal/en/topics/nierautomata-eoy/post02.html
- Push Square — "NieR: Automata Just Keeps Winning, Passes 9 Million" (2024.12)
- The Game Awards (X/Twitter) — 2017 Best Score/Music 수상 발표
- TheGamer — "Square Enix, What Is Going On With The Nier PC Ports?"
- GamesRadar+ — "Here's why Nier: Automata is getting review bombed on Steam"
- Steambase — NieR:Automata Reviews — https://steambase.io/games/nier-automata/reviews
- ScreenRant / Twinfinite / Fextralife / Medium(@azdiff) — 엔딩 A~E 해설
- ResetEra — 사이드퀘스트 토론 스레드
- scholarworks.uni.edu — "Nihilism in NieR: Automata's Narrative and Musical Score" (학술 논문)
- Game Developer(Gamasutra) — GDC 포스트모템 영상

---

*본 분석서는 영어권 매체 및 공식 출처를 기반으로 작성되었으며, 확인되지 않은 정보(예: 정확한 개발 예산)는 추측하지 않고 [확인된 자료 없음]으로 표기했다.*
