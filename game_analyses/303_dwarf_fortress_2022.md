# 《Dwarf Fortress》 (2022, Steam판) 심층 분석

> 20년 넘게 ASCII 문자로만 존재하던 전설적 시뮬레이션이, 두 형제의 의료보험을 위해 마침내 그래픽을 입고 대중 앞에 섰다. 출시 24시간 만에 2개월 목표를 달성한 이 사건은 인디 게임 역사상 가장 기묘하고 감동적인 성공담 중 하나다.

---

## 1. 게임 개요

### 개발사·퍼블리셔·크레딧

《Dwarf Fortress》는 미국의 1인(실질적으로 2인) 개발 스튜디오 **Bay 12 Games**가 만든 콜로니 시뮬레이션이다. 핵심 인물은 형제인 **Tarn Adams**(개발자 닉네임 "Toady One", 프로그래밍·디자인 전담)와 **Zach Adams**(닉네임 "Threetoe", 내러티브·세계관·스토리 담당)다. 2022년 Steam판의 퍼블리셔는 캐나다 몬트리올의 인디 퍼블리셔 **Kitfox Games**로, 2019년 3월에 협업을 발표하고 그래픽·음악 인재 섭외와 마케팅·퍼블리싱을 맡았다.

본 분석이 다루는 "2022 Steam판"(흔히 *Premium* 또는 *Steam edition*으로 불림)은 2022년 12월 6일 Steam과 itch.io에 동시 출시되었다. 가격은 약 29.99달러였다. 이는 16년 넘게 무료로 배포되던 클래식판(2006년 첫 공개)과 별개로 존재하는 유료 그래픽 버전이다.

### 디렉터·개발 규모

이 게임의 가장 비범한 점은 개발 규모다. Stack Overflow 개발자 블로그(2021년 12월)는 《Dwarf Fortress》를 두고 **"700,000 lines of code, 20 years, and one developer"**(70만 줄의 코드, 20년, 한 명의 개발자)라고 표현했다. 거의 모든 코드를 Tarn Adams가 단독으로 C++로 작성했다. 거대 스튜디오의 수백 명 인력, 수천만 달러 예산과는 정반대 극단에 있는, 가내 수공업적 평생 프로젝트다.

개발의 뿌리는 더 깊다. Tarn은 《Dwarf Fortress》 이전에 《Slaves to Armok: God of Blood》라는 RPG를 만들고 있었으나, 2004년경 코드 유지보수가 곤란해지자 새로운 프로젝트로 방향을 틀었다. 그렇게 탄생한 것이 《Dwarf Fortress》이며, 2006년 8월 처음 공개됐다. Tarn은 2011년 인터뷰에서 "버전 1.0은 최소 20년은 더 있어야 나올 것이고, 그 후에도 계속 작업할 것"이라고 밝힌 바 있다. 즉 이 게임은 본질적으로 **완성을 목표로 하지 않는 평생의 작업**이다.

### 엔진·기술 스택

자체 제작 엔진. 외부 게임 엔진을 일절 쓰지 않으며, 렌더링·시뮬레이션·세계 생성 모두 Tarn이 손수 짠 C++ 코드로 돌아간다. 클래식판은 텍스트 콘솔에 ASCII/CP437 문자를 찍는 방식이었고, 2022 Steam판은 그 위에 그래픽 타일 렌더링 레이어를 새로 얹었다.

---

## 2. 게임 설명: 이게 도대체 무슨 게임인가

### 컨셉

《Dwarf Fortress》를 한 문장으로 설명하기는 거의 불가능하지만, 가장 가까운 표현은 "**판타지 세계를 통째로 시뮬레이션하는, 콜로니 건설과 로그라이크 탐험이 결합된 게임**"이다. Wired는 이를 "난해하고 야심만만한 미완성작으로, 로그라이크의 잔혹한 던전 크롤링과 도시 건설 심의 디테일 집착적 창의성을 뒤섞은 것"(an obtuse, wildly ambitious work-in-progress that mashes the brutal dungeon crawling of roguelikes with the detail-oriented creativity of city-building sims)이라고 묘사했다.

게임은 먼저 **세계 하나를 통째로 생성**하는 것에서 시작한다. 단순히 지형 맵이 아니다. 고도, 강수량, 광물 분포, 배수, 온도 같은 기본 물리 요소를 절차적으로 깔고, 그 위에서 **수백~수천 년의 역사를 시뮬레이션**한다. 문명들이 흥망하고, 신화와 전설이 만들어지고, 전쟁이 벌어지고, 영웅과 괴물이 이름을 남긴다. 게임 개발 디렉터 Tarn의 표현을 빌리면 이는 "느슨한 턴 규칙과 형편없는 AI(하지만 수천 명의 에이전트)를 가진 0인용 전략 게임"이며, "역사란 그 게임의 기록일 뿐"이다. 플레이어가 본격적으로 플레이를 시작할 즈음, 발밑에는 이미 수백 년 치 역사가 깔려 있다.

### 두 가지 플레이 모드

- **Fortress Mode(요새 모드)**: 게임의 간판 모드. 플레이어는 일곱 명의 드워프를 이끌고 특정 지점에 정착(embark)한 뒤, 땅을 파고("Strike the Earth!") 요새를 건설하며 콜로니를 키운다. 드워프를 직접 조종하는 게 아니라 *간접 통제*한다 — 작업 우선순위와 명령을 내리면 드워프들이 각자의 성격과 욕구에 따라 알아서 움직인다. 좁은 공간에 콜로니를 압축해 넣고, 외부 문명과 괴물의 침공을 막아내는 것이 핵심이다.
- **Adventure Mode(모험 모드)**: 클래식판의 로그라이크 모드로, 단일 캐릭터 한 명을 직접 조종해 앞서 생성·시뮬레이션된 세계 전체를 자유롭게 탐험한다. 누구를 공격할지, 어디로 갈지 모두 플레이어 자유다. (단, 이 모드는 2022년 12월 Steam 최초 출시 시점에는 포함되지 않았고, 이후 베타로 추가됐다.)

### 무드·톤·아트 디렉션

원작의 미학은 순수한 ASCII였다. 드워프는 문자 ☺, 나무는 ♣, 물은 ≈로 표현됐고, 이 추상성이 오히려 플레이어의 상상력을 자극하는 장치로 기능했다. 2022 Steam판은 이를 따뜻하고 만화적인 픽셀 타일셋으로 교체했다. 커뮤니티에서 오랫동안 유명했던 비공식 타일셋 제작자들(Mayday, IronHand 등)이 공식 작업에 참여했다. 단, 그래픽이 입혀졌어도 화면을 가득 채우는 정보 밀도와 메뉴의 깊이는 그대로여서, 시각적 인상은 여전히 "친절한 스프레드시트" 같다는 평이 따른다.

### 사운드·음악

클래식판의 사운드는 Tarn이 직접 녹음한 어쿠스틱 기타 루프 한 곡이 사실상 전부였다. Steam판에서는 Kitfox가 작곡가를 섭외해 완전히 새로운 사운드스케이프와 음악을 추가했다. 드워프 광산의 분위기를 살리는 차분하고 민속적인 톤이 특징이다.

---

## 3. 핵심 시스템 / 메카닉

《Dwarf Fortress》의 진짜 정체성은 그 **시뮬레이션의 광기 어린 깊이**에 있다. 미국 매체 Reason은 2022년 리뷰에서 이를 "지금까지 만들어진 가장 깊고, 가장 불가해하며, 가장 어려운 시뮬레이션 게임"(the deepest, most inscrutable, and most difficult simulation game ever made)이라고 단언했다.

### 코어 게임플레이 루프 (요새 모드)

1. 세계를 생성한다(원하는 만큼 역사를 시뮬레이션).
2. 일곱 드워프와 보급품을 싣고 정착지를 고른다(embark).
3. 땅을 파 거주·작업 공간을 만들고, 가구·작업장·창고를 짓는다.
4. 식량과 술을 확보한다 — 드워프는 식량과 음료(주로 **술**)가 필요하며, 술이 떨어지면 사기와 작업 효율이 급락한다.
5. 인구가 늘고, 무역상·이주민·귀족이 오고, 동시에 고블린·포가튼 비스트·웨어크리처 같은 위협이 닥친다.
6. 방어·함정·군대를 갖추고, 콜로니의 사회·경제를 굴린다.
7. 거의 모든 요새는 결국 망한다 — 그리고 그것이 핵심이다.

### "Losing is !!FUN!!" — 패배의 철학

이 게임의 비공식 모토는 **"Losing is fun"**(지는 것이 재미다)이다. 공식 위키마저 "언제나 기억하라, 지는 것이 재미다(Always remember that losing is fun!). 진다는 것은 다음번에 어떻게 졌는지 기억하게 된다는 뜻"이라고 적는다. 《Dwarf Fortress》는 실패를 통한 학습을 게임 디자인의 중심에 놓는다. 홍수로 요새가 잠기고, 광기에 빠진 드워프가 동료를 학살하고, 끌어올린 마그마가 요새를 통째로 태우는 — 이 모든 파국이 결함이 아니라 *이야깃거리*다.

### 시뮬레이션 디테일 사례

이 게임이 전설이 된 것은 다음과 같은 비상식적 수준의 디테일 때문이다.

- **개성·심리 시뮬레이션**: 드워프 하나하나가 고유한 성격, 외모, 기술을 갖는다. 성격 모델링에는 실제 심리검사인 **NEO PI-R**(5요인 성격검사)이 참고됐다. 모든 드워프는 예술, 음식, 날씨, 사회적 상황에 대해 각자의 의견과 선호를 가지며, 정신 상태(스트레스, 분노, 슬픔)가 누적되면 발광·우울·기행으로 표출된다. 이는 길 잃은 **고양이 한 마리**에게도 적용된다.
- **신체·부상 시뮬레이션**: 신체 부위별 정밀 부상 시스템은 1990년 테이블탑 RPG 《Cyberpunk 2020》에서 영감을 받았다. 특정 손가락이 잘리거나, 신경이 끊겨 마비되거나, 폐가 찔려 질식하는 일이 개별적으로 추적된다.
- **그 유명한 "취한 고양이" 버그**: Tarn이 드워프 눈에 낀 이물을 닦아내기 위해 "눈꺼풀로 핥기" 기능을 추가하자, 술집 바닥의 알코올을 발에 묻힌 고양이들이 그루밍을 하다 발에 묻은 알코올을 핥아 **한 모금 분량의 술을 통째로 마신 것으로 계산되어 떼죽음**하는 버그가 생겼다. 이 일화는 게임의 비정상적 시뮬레이션 깊이를 상징하는 전설로 남았다.

이런 디테일이 70만 줄의 코드 안에서 서로 상호작용하며, 어느 누구도(개발자조차) 완전히 예측할 수 없는 **창발적 사건**을 끊임없이 만들어낸다.

### 난이도·접근성·UI/UX 철학

악명 높게 어렵다. GameSpot 유저 평을 빌리면 "신규 플레이어에게 믿기 힘들 만큼 적대적"이어서, "성공하기 전에 노는 법을 배우는 데 상당한 시간을 쏟아야 한다." 2022 Steam판의 가장 큰 디자인 목표가 바로 이 진입 장벽을 낮추는 것이었다 — 마우스 지원, 그래픽 타일, 정돈된 메뉴, 한눈에 보이는 정보가 추가됐다. IGN 리뷰는 이 점을 정확히 짚었다: "이미 전설이 된 게임을 위한 헌신적 리뉴얼로, 2022년판 《Dwarf Fortress》는 *casually interested*한 사람도 마침내 뛰어들어 'Strike the Earth!'를 외칠 수 있는 수준으로 끌어올렸다." 그럼에도 게임 자체의 본질적 복잡성은 줄어들지 않아서, 여전히 가장 어려운 게임 중 하나로 남아 있다.

---

## 4. 평가

### 평론 점수

- **Metacritic: 93 / 100**, "universal acclaim"(보편적 찬사), 12개 평론 기준. (출처: [Metacritic](https://www.metacritic.com/game/dwarf-fortress/))
- **OpenCritic: 90**, "Mighty" 등급, 13개 평론 기준. (출처: [OpenCritic](https://opencritic.com/game/14083/dwarf-fortress))
- **IGN: 10 / 10** — "이미 전설이 된 게임을 위한 헌신적 리뉴얼"이라 평하며 만점.
- **PC Gamer**(Steve Hogarty): "스스로를 예쁘게 꾸미는 데 단 1줄(joule)의 에너지도 쓰지 않으려는 《Dwarf Fortress》의 고집이, 경이로운 숨은 복잡성으로 귀결된다."(Dwarf Fortress's reluctance to expend even a joule of energy in prettying itself results in astonishing hidden complexity.)
- **Rock Paper Shotgun**(Quintin Smith, 원작 시절 평): "인터페이스가 원하는 대로 움직이게 만드는 건 마치 딱정벌레에게 요리를 가르치는 것 같다."(getting it to do what you want is like teaching a beetle to cook.) — 인터페이스의 난해함을 꼬집은 유명한 표현.
- **Wired**: "난해하고 야심만만한 미완성작."

### 유저 평가

- **Steam 유저 리뷰**: 약 94% 긍정(23,813개 리뷰 시점 기준). 이후 누적되며 "Overwhelmingly Positive"(압도적으로 긍정적)에 도달했다. Kitfox 포스트모템은 출시 초기 "Very Positive"를 빠르게 달성했고 "Overwhelmingly Positive"가 될 것이라 적었다.

### 수상

- **제26회 D.I.C.E. Awards(2023)**: AIAS(Academy of Interactive Arts & Sciences)가 수여하는 **Strategy/Simulation Game of the Year**(전략/시뮬레이션 부문 올해의 게임) 수상.
- 한편 **The Game Awards 2022**에서는 노미네이트되지 못해 커뮤니티가 불만을 표출하기도 했다.

### 평론-유저 괴리

이 게임은 평론과 유저 모두 극찬한 보기 드문 사례다. 다만 "괴리"라 부를 만한 지점이 있다면, **점수와 진입 난이도의 괴리**다. 93점·10점이라는 숫자만 보고 들어온 신규 유저가 첫 요새가 며칠 만에 전멸하는 경험을 하며 당황하는 경우가 많았다. 즉 "명작이지만 아무나 즐길 수 있는 명작은 아니"라는 합의가 평가의 저변에 깔려 있다.

---

## 5. 성공 요인 분석

### (1) 16년간 축적된 "전설"이라는 무형 자산

2022 Steam판의 성공은 마케팅의 승리라기보다 **16년간 쌓인 신화의 회수**였다. 이미 무료판으로 깊은 팬덤이 형성돼 있었고, 게임 업계 내부에서 "역사상 가장 깊은 시뮬레이션"이라는 컬트적 명성이 확고했다. Kitfox 포스트모템조차 이 극단적 성공이 "통상적인 퍼블리싱 전략이 아니라 게임의 전설적 위상과 고유한 조건"에서 비롯됐다고 인정했다. 즉 제품이 나오기 전부터 시장이 만들어져 있었다.

### (2) "의료보험을 위해 만든다"는 진정성 서사

Steam행의 동기 자체가 강력한 마케팅이었다. 형제는 16년간 게임을 **무료로 배포하며 기부금**(Steam 직전 월 약 1만 5천 달러)으로 생계를 이었다. 그러나 미국의 의료 시스템이 발목을 잡았다. Tarn은 "의료비가 사실상 (Steam행의) 전부"라며, "단 한 번의 건강 문제로 잘못된 본인부담금 상황에 빠지면 게임 풀타임 개발은 끝"이라고 말했다([Kotaku](https://kotaku.com/dwarf-fortress-is-coming-to-steam-because-its-developer-1833333064)). 실제로 동생 Zach는 코의 악성 종양 제거 수술을 받았고(보험이 1만 달러 수술의 대부분을 커버했으나 본인부담 1,500달러 발생), 재발까지 겪었다. "돈이 목적이 아니었던 개발자들이 이제 돈이 필요해졌다"(Vice)는 이 서사는 게이머들의 공감과 응원을 끌어냈고, 구매가 곧 후원이 되는 분위기를 만들었다.

### (3) 진입 장벽 제거라는 정확한 제품 개선

성공의 실질적 엔진은 **그래픽·UI 개편**이었다. 무료판이 있었음에도 유료판이 수십만 장 팔린 이유는, ASCII와 키보드 미로에 막혀 진입하지 못했던 거대한 잠재 수요를 그래픽판이 흡수했기 때문이다. "이제 마침내 들어가 볼 수 있겠다"는 IGN의 평가가 곧 구매 동기였다.

### (4) Kitfox의 절제된 퍼블리싱

Kitfox는 Bay 12의 기존 투명성 문화(개발 일지 공개 등)를 그대로 유지하고, 신뢰받는 커뮤니티 인사들(Clinodev, Mayday, IronHand 등)과 협업하며, Discord를 커뮤니티 허브로 운영했다. 출시일은 실현 가능성이 확실해질 때까지 발표를 미뤘고, 일부 기대 기능은 초기 출시에서 의도적으로 컷해 **모멘텀을 유지**했다. 거대 마케팅이 아니라, 까다로운 코어 팬덤을 적으로 돌리지 않는 신중한 관리가 핵심이었다.

### (5) 타이밍과 입소문

2022년 12월, 연말 시즌에 출시되어 "마침내 그래픽이 입혀진 전설"이라는 이야기가 게임 매체와 SNS를 도배했다. 동시기의 거대 작품들과 정면 경쟁하지 않는 독보적 위치 — "다른 어떤 게임과도 닮지 않은 게임"이라는 차별성 — 이 입소문을 폭발시켰다.

---

## 6. 비평적 시각 / 한계 / 논란

### 학습 곡선

가장 일관된 비판은 여전히 **진입 난이도**다. 그래픽판이 문턱을 낮췄다고는 하나, RimWorld나 Stardew Valley 같은 후예들과 비교하면 비교 불가능하게 어렵다. 메뉴의 깊이, 정보의 밀도, 기본적인 "무엇을 해야 하는지조차 알기 어려움"이 상존한다. 많은 신규 구매자가 튜토리얼만으로는 부족해 위키와 유튜브 가이드에 의존해야 했다.

### 미완성작이라는 본질

《Dwarf Fortress》는 정의상 **영원한 work-in-progress**다. Adventure Mode는 2022년 12월 Steam 출시 시점에 빠져 있었고(이후 베타로 추가), 클래식판이 가진 일부 기능도 초기 그래픽판에는 없었다. "30달러를 내고 미완성 게임을 산다"는 점은 일부에게 거부감을 줬다. 다만 16년의 전례를 아는 팬덤은 이를 결함이 아니라 지속적 무료 업데이트의 약속으로 받아들였다.

### 인터페이스의 잔재

RPS의 "딱정벌레에게 요리 가르치기" 비유가 상징하듯, 새 UI도 모든 거친 모서리를 다듬지는 못했다. 방대한 기능을 그래픽 메뉴 하나에 욱여넣은 결과, 일부 조작은 여전히 직관과 거리가 멀다.

### 콘텐츠 컷 논란

Kitfox가 모멘텀 유지를 위해 일부 기능을 초기 출시에서 뺀 결정은 합리적 퍼블리싱 판단이었으나, 일부 코어 팬은 클래식판 대비 기능 누락을 아쉬워했다.

---

## 7. 영향과 유산

### 하나의 장르를 낳다

《Dwarf Fortress》는 단순히 영향을 준 정도가 아니라 **"콜로니 심"이라는 장르 자체를 창시**했다. 적대적 환경에서 자율적으로 움직이는 소수의 캐릭터를 돌보며 사회를 키워나가는 모든 게임이 이 게임의 후예다.

- **《Minecraft》**: 창작자 Markus "Notch" Persson은 《Dwarf Fortress》의 영향을 직접 인정했고, 비평가들은 Minecraft를 "더 친근한 버전의 Dwarf Fortress"로 평가하곤 한다. 세계 최다 판매 게임이 이 무료 ASCII 게임에 빚을 지고 있다는 사실은 그 영향력의 척도다.
- **《RimWorld》**: 개발자 Tynan Sylvester는 "사람들이 이 게임에서 써낸 이야기들에 놀랐다. *Boatmurdered*와 *Gemclod* 같은 생성된 전설을 읽으며, 플레이어와 게임이 함께 실제로 작동하는 내러티브를 만들어내는 방식에 매료됐다. 나는 그것을 더 밀어붙이고 싶었다"고 밝혔다. RimWorld는 DF의 동적 스토리텔링을 보다 접근 가능하게 다듬은 정신적 후계작이다.
- 그 밖에 **《Prison Architect》, 《Project Zomboid》, 《Terraria》, 《Caves of Qud》** 등의 개발자들이 Steam 출시를 맞아 일제히 영향을 인정했다.

### 창발적 스토리텔링의 원형: Boatmurdered

게임의 문화적 유산을 압축하는 단어가 **Boatmurdered**다. 2006년 11월부터 2007년 3월까지 Something Awful 포럼의 14명이 한 요새를 릴레이로 이어 플레이하며 기록한 전설적 Let's Play로, 코끼리 떼의 습격과 마그마 함정, 광기와 파멸이 뒤엉킨 이 서사시는 "게임이 작가 없이도 위대한 이야기를 생성할 수 있다"는 증거로 회자된다. RimWorld 디자이너가 직접 언급할 만큼 게임 디자인계의 정전(canon)이 됐다.

### 산업적·문화적 의미

2012년 3월, **뉴욕 현대미술관(MoMA)**이 비디오게임의 역사를 보여주는 전시에 《Dwarf Fortress》를 선정·소장했다. 게다가 MoMA는 새 업데이트가 나올 때마다 이를 즉시 다운로드해 서버에 아카이브한다 — 끊임없이 진화하는 작품을 박물관이 박제하는 대신 *살아있는 채로* 보존하는 독특한 사례다. 산업적으로 이 게임은 "1인 개발자가 평생을 바친 비타협적 시뮬레이션도 100만 장을 팔 수 있다"는 가능성을 입증했고, 인디 개발의 한 극단적 이상향으로 남았다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 수치 | 출처 |
|---|---|---|
| Steam/itch.io 출시일 | 2022년 12월 6일 | Steam |
| 가격 | 약 $29.99 | Steam |
| 첫 24시간 판매 | 약 160,000장 (Kitfox의 2개월 목표를 하루에 달성) | Kitfox 포스트모템 |
| 첫 주 판매 | 약 300,000장 | PC Gamer |
| 첫 2개월 판매 | 정확히 606,342장 (itch.io 약 5,000장 포함) | Kitfox 포스트모템 |
| 1년차 누적 | 800,000장 이상 | gamedeveloper.com |
| 누적 판매 (2025년 4월) | 1,000,000장 돌파 | PC Gamer / gamedeveloper.com |
| 2023년 1월 매출 | $7.2M 이상 (Steam 이전 월 약 $15,000 대비 400배+) | Bay 12 포럼 |
| Metacritic | 93 / 100 (universal acclaim) | Metacritic |
| OpenCritic | 90 (Mighty) | OpenCritic |
| IGN | 10 / 10 | IGN |
| Steam 유저 평가 | 94% 긍정 → Overwhelmingly Positive | Steam |
| 코드 규모 | 약 700,000줄, 단독 개발 | Stack Overflow 블로그 |
| 수상 | D.I.C.E. 2023 Strategy/Simulation Game of the Year | AIAS |

### 주요 인터뷰·자료

- "Dwarf Fortress Is Coming To Steam Because Its Developer Needs Healthcare" — Kotaku, 2019 ([링크](https://kotaku.com/dwarf-fortress-is-coming-to-steam-because-its-developer-1833333064))
- "The 'Dwarf Fortress' Creators Weren't in It For Money, But Now They Need It" — Vice
- "700,000 lines of code, 20 years, and one developer: How Dwarf Fortress is built" — Stack Overflow 개발자 블로그, 2021 ([링크](https://stackoverflow.blog/2021/12/31/700000-lines-of-code-20-years-and-one-developer-how-dwarf-fortress-is-built/))
- "Dwarf Fortress: 2 Months Later — A post-partum and publishing retrospective" — Kitfox Games, Medium, 2023 ([링크](https://medium.com/kitfox-games-shenanigans/dwarf-fortress-2-months-later-648d1c4f34d2))
- "Dwarf Fortress: Figuring out how to simulate the universe, one step at a time" — Game Developer
- "Rimworld, Dwarf Fortress, and procedurally generated story telling" — Game Developer

### 참고 자료 목록 (영어권 매체 중심)

- [Wikipedia: Dwarf Fortress](https://en.wikipedia.org/wiki/Dwarf_Fortress)
- [Steam 스토어 페이지](https://store.steampowered.com/app/975370/Dwarf_Fortress/)
- [Metacritic](https://www.metacritic.com/game/dwarf-fortress/) / [OpenCritic](https://opencritic.com/game/14083/dwarf-fortress)
- [Reason: 'Dwarf Fortress,' the deepest, most insane computer simulation game ever](https://reason.com/2022/12/08/)
- [PC Gamer: Dwarf Fortress review](https://www.pcgamer.com/dwarf-fortress-review/)
- [PC Gamer: Dwarf Fortress sells 1 million copies on Steam](https://www.pcgamer.com/games/sim/dwarf-fortress-sells-1-million-copies-on-steam-so-now-bay-12-games-can-afford-that-little-party-it-planned/)
- [Boatmurdered (Wikipedia)](https://en.wikipedia.org/wiki/Boatmurdered)
- [Dwarf Fortress Wiki: Losing / World generation](https://dwarffortresswiki.org/)

---

*본 분석서는 2022년 12월 Steam판(Premium) 출시를 기준으로 작성되었으며, 모든 판매·매출 수치는 위 출처가 보도한 시점 기준이다.*
