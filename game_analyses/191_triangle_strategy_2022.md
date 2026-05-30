# Triangle Strategy (2022) 심층 분석

> 신념의 저울 위에 올라선 택틱스 RPG — 《Final Fantasy Tactics》의 망령을 HD-2D로 되살린 정치 드라마

---

## 1. 게임 개요

《Triangle Strategy》는 Square Enix가 퍼블리싱하고 Square Enix와 Artdink가 공동 개발한 택틱스(Tactical) RPG다. 2022년 3월 4일 Nintendo Switch로 전 세계 동시 출시되었고, 같은 해 10월 13일 PC(Steam)판이 발매되었다. 이후 IP의 롱테일을 노린 멀티플랫폼 확장이 이어져 2024년 10월 31일 Meta Quest 2·Pro·3용 VR 버전이, 2025년 8월 20일에는 PlayStation 5와 Xbox Series X|S판이 추가되었다. 장르는 그리드 기반 턴제 전략 시뮬레이션 RPG로, 분기형 멀티 엔딩 내러티브를 핵심에 둔 점이 특징이다.

이 게임의 정체성을 이해하려면 **개발 진영**부터 봐야 한다. 프로듀서는 Square Enix 내부의 이른바 "Team Asano"를 이끄는 **Tomoya Asano(아사노 토모야)**다. 그는 《Bravely Default》 시리즈와 《Octopath Traveler》를 프로듀싱하며 "고전 JRPG의 정신을 현대 기술로 되살린다"는 일관된 노선을 구축해 온 인물이다. 공동 프로듀서로는 **Yasuaki Arai(아라이 야스아키)**가 참여했다. 시나리오는 **Naoki Yamamoto**, 캐릭터 디자인은 **Naoki Ikushima**가 맡았고, 음악은 애니메이션·드라마 스코어로 명성이 높은 작곡가 **Akira Senju(千住明, 센주 아키라)**가 게임 사상 첫 풀 오리지널 사운드트랙으로 참여했다.

개발의 또 다른 축인 **Artdink**는 1988년부터 활동해 온 일본 개발사로, 의외로 깊은 SRPG 혈통을 지녔다. Artdink는 1993년 《Ogre Battle: The March of the Black Queen》과 1995년 《Tactics Ogre: Let Us Cling Together》의 개발에 협력한 이력이 있다. 이 두 작품은 후일 《Final Fantasy Tactics》(이하 《FFT》)에 직접적 영향을 준 마쓰노 야스미(Yasumi Matsuno) 계열의 정치 택틱스 명작들이다. 즉 《FFT》의 정신적 후속작을 만든다는 이 프로젝트에서, Artdink는 《FFT》가 참조한 원류를 만든 동시에 《FFT》를 참조하는, 이른바 "한 바퀴를 돌아 제자리로 온(full circle)" 위치에 서 있었다. Kotaku는 이를 두고 "픽셀 아트 노스탤지어보다 깊은(deeper than pixel art nostalgia)" 게임이라 평했다.

기술 스택은 Square Enix가 《Octopath Traveler》에서 정립한 **HD-2D** 아트 엔진이다. Unreal Engine 기반으로, SNES 시절의 도트 스프라이트를 고해상도로 렌더링하고 그 위에 실시간 라이팅·피사계 심도·파티클·3D 카메라를 입혀 "움직이는 디오라마" 같은 질감을 만들어 낸다. 본작은 이 HD-2D 양식을 택틱스 그리드 전장에 적용한 첫 사례에 가깝다.

게임의 전신은 2021년 공개된 데모 《Project Triangle Strategy》다. Square Enix는 이 데모를 단순 홍보가 아니라 **개발 피드백 수집 도구**로 활용했다. 데모 플레이어를 대상으로 설문을 돌려 공통적으로 제기된 불만을 정식판에 직접 반영했는데, 추가 난이도 모드·대체 카메라 조작·지난 대사 회고 기능 등이 그 산물이다.

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 세계관과 배경

무대는 가공의 대륙 **Norzelia(노르젤리아)**다. 이 대륙은 두 가지 희소 자원, **소금(salt)**과 **철(iron)**을 둘러싼 긴장 위에 세워져 있다. 세 세력이 자원과 교역로를 분점한다.

- **Glenbrook(글렌브룩) 왕국**: 대륙의 강과 주요 교역로를 장악한 입헌적 왕정. 균형추 역할.
- **Grand Duchy of Aesfrost(아에스프로스트 대공국)**: 북방의 혹한 지대를 근거로 **철**을 독점 생산하는 실력주의·무력 지향 국가.
- **Holy State of Hyzante(하이잔테 신정국)**: 여신 신앙을 국교로 삼아 **소금**을 독점하는 신권 체제. 표면의 성스러움 뒤에 로젤족(Roselle)을 노예·박해하는 어두운 구조를 숨기고 있다.

이 세 나라는 30년 전 자원을 두고 **Saltiron War(염철 전쟁)**를 벌였고, 그 휴전의 불안정한 균형 위에서 이야기가 시작된다. 갈등의 3축 구도가 게임 제목인 "Triangle(삼각)"의 일차적 의미이며, 동시에 후술할 신념 시스템의 3축과 이중으로 호응한다.

### 줄거리 [스포일러 포함]

주인공은 글렌브룩의 변경 명문가 **House Wolffort**의 후계자 **Serenoa Wolffort(세레노아 볼포트)**다. 그의 약혼녀는 아에스프로스트 대공의 서녀이자 박해받는 로젤족의 피를 이은 **Frederica Aesfrost(프레데리카)**, 죽마고우는 글렌브룩의 제2왕자 **Roland Glenbrook(롤랜드)**, 곁에는 냉철한 책략가 집사 **Benedict Pascal(베네딕트)**과 현실주의 힐러 **Geela(질라)** 등이 포진한다.

[스포일러] 이야기는 화해의 무드에서 출발한다. 글렌브룩과 아에스프로스트는 새로 발견된 거대 광산 **Grand Norzelian Mine**을 공동 개발하기로 합의하며 관계 개선을 시도한다. 그러나 아에스프로스트의 인물 Dragan이 암살당하고, 대공 **Gustadolph(구스타돌프)**는 이를 글렌브룩의 소행으로 몰아 응징 명목의 침공을 감행한다. Serenoa 일행이 손쓸 새도 없이 Gustadolph는 글렌브룩 수도를 함락하고 Regna 왕과 Frani 왕자를 살해하며 Cordelia 공주를 사로잡는다. 그 결과 Roland만이 글렌브룩 왕위의 유일한 계승자로 남는다. 여기서부터 Serenoa는 가문과 친구, 약혼녀, 그리고 대륙 전체의 운명 사이에서 끝없이 선택을 강요받는다.

표면적으로는 글렌브룩-아에스프로스트의 전쟁극이지만, 진짜 무게중심은 **Hyzante**다. 신정국은 소금 독점과 여신 숭배로 대륙의 도덕적 권위를 자처하지만, 그 번영은 로젤족에 대한 조직적 노예제 위에 서 있다. 이 "성스러운 위선" 구조가 후반부 도덕적 딜레마의 핵심으로 부상한다.

### 캐릭터와 톤

본작은 단일 영웅 서사가 아니라 **합의제 정치극**의 형식을 취한다. Serenoa는 압도적 카리스마의 영웅이 아니라, 서로 다른 가치를 가진 동료들을 설득하고 표를 모으는 "조정자"다. 각 동료는 뚜렷한 가치관을 갖는다. Frederica는 도덕(연민)을 우선하는 강한 의지의 귀족, Benedict는 "누가 무엇을 희생하든 House Wolffort가 최우선"인 실리주의 책략가, Geela는 "오늘 하루 더 살아남는 길"을 택하는 현실주의자로 그려진다. 이 가치관 분포가 그대로 게임 시스템의 표심으로 변환된다.

전체 톤은 **"성숙한(mature) 정치 드라마"**다. Inverse와의 인터뷰에서 개발진은 본작이 단순 선악 구도가 아니라 "정답이 없는 선택"을 다루는 어른 대상의 이야기임을 강조했다. 배신·암살·노예제·난민·기근 같은 무거운 소재가 정면으로 다뤄지며, 어떤 선택도 누군가의 희생을 동반한다.

### 사운드와 음악

음악은 본작의 가장 일관된 호평 지점 중 하나다. 작곡가 **Akira Senju**는 1960년 도쿄 출생으로 도쿄예술대학에서 작곡을 전공해 최고 영예로 석사를 마쳤으며, 《강철의 연금술사 Brotherhood》 등 애니메이션·실사 드라마 스코어로 명성이 높다. 《Triangle Strategy》는 그의 **첫 전곡 게임 OST**였다. 60명 이상의 연주자가 참여한 풀 오케스트라 녹음으로, 4장 분량의 사운드트랙이 분기형 서사 곳곳에 배치되었다. 피아니스트 Haruki Mino 등이 참여한 이 스코어는 RPGFan 등 음악 전문 매체로부터 게임 음악으로서는 보기 드문 격조 높은 오케스트레이션이라는 평을 받았다.

---

## 3. 핵심 시스템과 메카닉

### Scales of Conviction — 신념의 저울 (가장 중요한 시스템)

본작을 다른 SRPG와 결정적으로 구분 짓는 것은 전투가 아니라 **Scales of Conviction(신념의 저울)** 투표 메카닉이다. 이야기의 중대 분기마다 Serenoa는 결정을 혼자 내리지 못한다. 7명의 핵심 동료가 각자 **동전(coin)** 한 닢씩을 들고 거대한 저울 앞에 모여 **투표**한다. 다수결의 결과가 그 챕터의 진로를 결정하고, 누적된 결과가 종국에는 엔딩 자체를 가른다.

이 시스템의 묘미는 투표 직전에 주어지는 **설득 단계**다. 투표 전 Serenoa는 마을을 돌며 정보를 수집하고, 그렇게 모은 정보나 자신의 강한 신념을 근거로 동료를 개별 설득해 표심을 바꿀 수 있다. Kotaku는 이를 "표를 얻고 사람을 움직이는(win votes and influence people)" 게임이라 표현했다. 캐릭터마다 설득 난도가 다르다. 가령 Benedict는 가문 이익에 반하는 선택이라면 거의 흔들리지 않는 반면, Geela는 "이 곤경에서 빠져나갈 그럴듯한 계획"만 제시하면 비교적 쉽게 원하는 쪽으로 표를 던진다. 즉 투표는 단순 선택지 클릭이 아니라, 각 동료의 가치관을 읽고 그에 맞는 논거를 준비하는 일종의 미니 협상 게임이다.

### 세 갈래 신념 — Utility / Morality / Liberty

저울의 배후에는 Serenoa 개인의 **Conviction(신념)** 수치가 작동한다. 신념은 세 축으로 나뉜다.

- **Utility(실리/실용)**: 효율과 결과를 중시하는 실용주의.
- **Morality(도덕/연민)**: 약자 보호와 윤리적 정당성을 중시하는 도덕주의.
- **Liberty(자유)**: 개인과 집단의 자유·자결을 중시하는 자유주의.

이 수치는 게임 내내 **비밀리에** 누적된다. 플레이어가 대사 선택이나 행동을 할 때마다 해당 축의 점수가 오르며, 신념 선택지를 고르면 관련 축에 50점이 더해진다. 중요한 것은 이 수치가 **화면에 명시되지 않는다**는 점이다(1회차 기준). 플레이어는 자신이 어떤 신념을 키워 왔는지 정확히 알지 못한 채 캐릭터를 연기하게 되고, 그 누적치가 어떤 동료를 영입할 수 있는지, 어떤 루트로 흐를지, 어떤 엔딩에 도달할지를 은밀히 좌우한다. 이 "보이지 않는 도덕 게이지"는 플레이어가 결과를 계산하기보다 캐릭터의 신념에 몰입하도록 유도하는 장치다. New Game Plus(NG+)에서는 비로소 각 대사 선택지가 Utility·Morality·Liberty 중 무엇을 얼마나 올리는지 수치가 공개되어, 2회차부터는 의도적 루트 설계가 가능해진다.

### 전투 시스템 — 타일 기반 정밀 택틱스

전투는 정통 그리드 기반 턴제 SRPG다. 다만 디테일이 촘촘하다.

- **행동 순서**: 유닛의 **속도(speed)** 스탯에 따라 턴이 결정된다.
- **TP(Tactical Points)**: 기본 공격을 제외한 모든 스킬은 TP를 소비한다. 매 턴 1 TP가 차오르고, 마법 사용자는 주력기에 보통 2 TP가 필요해 자원 관리 압박이 크다. TP 운용이 곧 화력 배분 전략이 된다.
- **지형과 고저차**: 전장은 입체적이다. 고지대에서 내려치는 공격은 명중률과 데미지가 상승하고, 저지대에서 올려치는 공격은 불리하다. 단순 평면 체스가 아니라 높이를 활용한 진형 설계가 승패를 가른다.
- **속성·환경 상호작용**: 환경을 무기로 쓰는 설계가 깊다. 눈 위에서 화염 스킬을 쓰면 타일이 진창(bogged)으로 변하고, 얼어붙은 타일이 화염과, 불타는 타일이 얼음과 만나도 진창이 된다. 전기는 **물을 통해 전파**되어 물에 잠긴 적 다수를 한 번에 감전시킬 수 있다. 화공·빙결·감전의 연쇄를 짜는 것이 고난도 전투의 핵심이다.
- **협공과 배후**: 적을 두 유닛이 양옆에서 끼면 자동으로 **추격타(follow-up)**가 발동해 한 번에 두 번 때린다. 배후에서의 공격은 **자동 크리티컬**이다. 따라서 적을 둘러싸는 포지셔닝이 데미지 효율을 극대화한다.
- **Quietus(퀴에투스)**: 전투당 1회 사용 가능한 특수 행동으로, **턴을 소모하지 않는다**. 야영지의 Eagle-Eyed Elder에게 kudos(전공 포인트)를 지불해 추가 퀴에투스를 해금할 수 있다. 위기 순간을 뒤집는 "비장의 카드"로 기능한다.

흥미롭게도 본작에는 **영구사망(permadeath)이 없다**. Fire Emblem이나 일부 클래식 SRPG와 달리, 전투에서 쓰러진 유닛은 다음 전투에 복귀한다. 개발진은 Destructoid 인터뷰에서 이는 플레이어가 서사적 선택에 집중하도록 전투 페널티의 가혹함을 의도적으로 낮춘 결정이라고 설명했다.

### 진행 구조와 야영지

게임은 17개 안팎의 챕터로 구성되며, 전투-탐색-투표-컷신이 교차한다. 전투 사이에는 **야영지(encampment)**가 허브 역할을 한다. 여기서 무기 강화, 신규 캐릭터 영입, 정보 열람, 퀴에투스 구매가 이뤄진다. 영입 캐릭터의 해금에는 **Mental Mock Battle(가상 모의전)**이라는 별도 전투가 쓰이며, NG+에서는 이들의 하드 버전과 추가 모의전이 열린다.

### 멀티 엔딩과 리플레이 구조

본작은 **4종의 엔딩**을 갖는다. 게임 내내 어떤 신념(Utility·Morality·Liberty)을 강화했는지에 따라 세 갈래 루트 엔딩이 갈리고, 여기에 특정 분기 플래그를 모두 충족했을 때만 열리는 **Golden Route(True Ending)**가 더해진다. Golden Route는 "신념의 저울 자체를 거부하고, 누구도 잃지 않는 제3의 길을 찾는" 결말로, Serenoa의 가장 가까운 세 동료가 누구도 이탈하지 않는다.

Golden Route 해금 조건은 까다롭다. 보고된 분기 선택은 다음과 같다 — 7장에서 Roland 보호, 9장에서 밀수 소금 운반, 10a장에서 Roland 정체 공개, 11장에서 Roselle 방어, 15장에서 Wolffort 귀환, 17장에서 "다른 길 찾기" 선택. 게다가 **30명의 플레이어블 캐릭터를 1회차에 모두 모으는 것은 불가능**하다. 일부 캐릭터는 특정 엔딩 루트에 묶여 있어 사실상 게임을 네 번 클리어해야 전원 영입이 가능하다. 가령 강력한 캐릭터 **Avlora**는 Golden Route에서만 영입된다. NG+는 영입 유닛·레벨·강화를 인계해 반복 플레이의 부담을 덜어 준다. 이 구조는 단편적 분기를 넘어 게임 전체를 4회 순회하게 만드는, 강력한 리플레이 설계다.

### UI/UX와 접근성

데모 피드백을 반영한 접근성 개선이 두드러진다. **Easy / Normal / Hard 세 난이도**가 제공되며(데모판은 난이도 선택이 제한적이었다), 대체 카메라 조작과 지난 대사 회고(backlog) 기능이 추가되었다. 방대한 텍스트 분량을 고려하면 대사 회고는 사실상 필수 기능이었고, 이는 플레이어 의견을 직접 반영한 대표 사례로 자주 인용된다.

---

## 4. 평가

### 평론 점수

《Triangle Strategy》는 평론 집계 사이트 Metacritic에서 Nintendo Switch 기준 "generally favorable(대체로 호평)" 등급을, OpenCritic에서도 양호한 평가를 받았다. 주요 매체 점수는 다음과 같다.

| 매체 | 점수/평가 |
|------|-----------|
| IGN | 8 / 10 |
| GameSpot | 8 / 10 |
| Eurogamer | Recommended (추천) |
| Metacritic (Switch) | Generally Favorable |

평론가들이 공통적으로 칭찬한 지점은 **전투의 전략적 깊이**, **정치 서사의 복잡성과 성숙함**, **Akira Senju의 오케스트라 스코어**, 그리고 **HD-2D 아트 디렉션**이었다. 동시에 거의 모든 리뷰가 한 가지 약점을 공통으로 지적했는데, 바로 **컷신·대사량의 과다함**이다(6장에서 상술).

### 상업 성적

상업적으로는 견조한 성공을 거뒀다. 출시 약 2주 만에 전 세계 출하량(디지털 포함)이 **약 800,000장**에 도달했고, 이 중 일본·아시아 지역에서만 20만 장 이상이 팔렸다(VGChartz, Gamereactor 보도). 이후 2022년 12월, Square Enix는 **전 세계 출하량과 디지털 판매 합계가 100만 장을 돌파**했다고 발표했다(Gematsu, RPG Site). 이 수치는 2022년 3월 4일 Switch 출시와 10월 13일 PC(Steam) 출시를 합산한 것이다.

니치 장르인 정통 택틱스 RPG로서, 그리고 초기엔 사실상 Switch 단일 플랫폼으로 출발한 작품으로서 100만 돌파는 상당한 성과다. 이후 2025년 PS5·Xbox 멀티플랫폼 확장과 VR판 출시는 이 IP의 장기 수익화를 노린 행보로 읽힌다.

### 수상

The Game Awards 2022에서 **Best Role-Playing Game(최우수 RPG) 부문에 노미네이트**되었으나, 그해 최강자 《Elden Ring》에 밀려 수상에는 이르지 못했다. 시대를 압도한 거대 RPG와 같은 부문에서 경합했다는 사실 자체가 본작의 평단 입지를 방증한다.

### 유저 평가와 평론-유저 괴리

유저 평가도 대체로 긍정적이었으나, 평론과 유사하게 "스토리 분량 대비 전투 비중"을 두고 의견이 갈렸다. Steam 커뮤니티에서는 "리뷰어들이 게임의 75%가 대사고 25%가 전투라고 하는데 정말 그런가?"라는 토론이 활발했고, 일부 유저는 본작을 "긴 스토리텔링 때문에 SRPG 요소가 끼인 비주얼 노벨처럼 느껴진다"고 평했다. 즉 평론과 유저 모두 게임의 품질 자체는 인정하되, **택틱스 게임으로서의 정체성**에 대한 기대치 차이에서 호불호가 갈렸다.

---

## 5. 성공 요인 분석

### 디자인 측면 — 시스템과 서사의 이중 삼각구조

본작 최대의 디자인 성취는 **세계관의 3국 구도**와 **신념의 3축(Utility·Morality·Liberty)**, 그리고 **투표 메카닉**을 하나의 일관된 테마로 묶어낸 점이다. 제목 "Triangle"이 정치 구도이자 도덕 시스템이자 게임플레이 루프를 동시에 지시한다. 서사적 선택이 단순 분기 대사로 끝나지 않고 동료 영입·전투 자원·엔딩까지 기계적으로 연결되므로, 플레이어의 도덕적 고민이 곧 시스템적 결과로 환산된다. 이 "내러티브-메카닉 일체화"가 본작을 단순한 비주얼 노벨이나 단순한 SRPG가 아닌, 둘의 진지한 결합으로 만든다.

### 브랜드와 계보 — Team Asano + FFT 혈통

상업적·평단적 신뢰의 상당 부분은 **Team Asano** 브랜드에서 왔다. 《Octopath Traveler》와 《Bravely Default》로 "고전 JRPG를 현대 기술로 정성껏 복원한다"는 신뢰를 쌓은 팀이 만든 신작이라는 사실 자체가 강력한 마케팅 자산이었다. 여기에 Artdink의 SRPG 혈통(《Tactics Ogre》 개발 협력)이 더해지며, 본작은 자연스럽게 **《Final Fantasy Tactics》의 정신적 후속작**으로 포지셔닝되었다. 《FFT》 정식 후속작이 수십 년째 부재한 상황에서, 그 갈증을 정조준한 것이다.

### 시장 타이밍

2022년 초 Switch 진영에는 정통 택틱스 RPG의 공백이 컸다. Fire Emblem 신작과 신작 사이의 간극, 그리고 《FFT》 부재 속에서, 본작은 "깊이 있는 정치 택틱스를 갈망하던 코어 SRPG 팬덤"이라는 명확한 타깃에 정확히 안착했다. 거대 AAA들과 직접 경쟁하기보다 니치를 독점하는 전략이 주효했다.

### 개발 방법론 — 데모 주도 개발

데모 《Project Triangle Strategy》를 통한 피드백 수집·반영은 본작 성공의 숨은 요인이다. 난이도 추가, 카메라 개선, 대사 회고 같은 변경이 모두 실제 플레이어 데이터에 기반했다. 출시 전부터 "개발사가 우리 의견을 듣는다"는 신뢰를 형성했고, 동시에 출시판의 완성도와 접근성을 끌어올렸다. 이는 Team Asano가 《Bravely Default》 시절부터 이어온 데모-피드백 문화의 연장선이다.

### 동시기 작품 대비 차별점

같은 HD-2D 형제작 《Octopath Traveler》가 8인 옴니버스 RPG였다면, 본작은 **단일하고 응집된 정치 대하 드라마 + 택틱스**라는 정반대 방향을 택해 HD-2D 라인업 내에서 차별화에 성공했다. Fire Emblem 대비로는 영구사망을 제거하고 투표·분기를 전면화해, 전술보다 서사적 선택의 무게에 방점을 찍었다.

---

## 6. 비평적 시각 — 한계와 논란

### 압도적 대사량, 절뚝거리는 페이싱

본작의 거의 유일하면서도 치명적인 약점은 **컷신과 대사의 과부하**다. Eurogamer는 페이싱, 특히 대사 시퀀스를 강하게 비판하며 "전투 한 번을 치르고 나면 한 시간이 넘는 컷신이 이어지곤 한다"고 지적했다. 어떤 리뷰어는 단일 컷신 시퀀스가 **30분 넘게 어떤 상호작용 기회도 없이** 지속되는 것을 측정해 보고하기도 했다. 다수 매체가 본작을 "가끔 전투를 허용하는 비주얼 노벨"에 비유했고, "전투보다 읽기가 많은 게임"이라는 인상은 택틱스 팬 일부에게 진입 장벽으로 작용했다. CogConnected는 PS5판 리뷰에서 이를 "뛰어난 전투, 분열적인 페이싱(Brilliant Combat, Divisive Pacing)"이라고 압축했다.

### 진짜 결말로 가는 길의 불친절함

멀티 엔딩 구조는 강점이자 약점이다. **Golden Route(True Ending)** 해금 조건이 직관적이지 않아, 무계획적인 1회차로는 도달하기 어렵다. 게다가 30명 전원 영입에 4회차가 필요한 설계는 헌신적인 팬에게는 보상이지만, 라이트 유저에게는 부담이다. 많은 플레이어가 결국 가이드에 의존하게 되는데, 이는 "보이지 않는 신념 수치"라는 디자인 철학과 실용적으로 충돌하는 지점이다.

### 전투 시스템이 서사에 묻힌다는 지적

역설적으로, 본작의 전투는 깊이 있고 잘 만들어졌음에도 **전투 횟수 자체가 적다**는 비판이 있다. 방대한 컷신 사이사이에 전투가 드문드문 배치되어, 전술 시스템의 잠재력을 충분히 즐기기 전에 다시 긴 대사 구간으로 돌아가야 한다. 깊은 시스템이 충분한 플레이 기회를 얻지 못한다는 아쉬움이다.

### 평가가 갈리는 지점

요컨대 본작의 호불호는 거의 전적으로 **"이것을 택틱스 게임으로 볼 것인가, 인터랙티브 정치 소설로 볼 것인가"**라는 기대치 문제로 수렴한다. 후자로 받아들이는 플레이어에게는 걸작에 가깝고, 전자를 기대한 플레이어에게는 "전투가 너무 적은 SRPG"가 된다.

---

## 7. 영향과 유산

### HD-2D 라인업의 확장

《Triangle Strategy》는 Square Enix의 **HD-2D 브랜드**를 단일 장르(《Octopath》의 정통 JRPG)에서 **택틱스 RPG로 확장**한 작품이다. 도트 그래픽이 단순 노스탤지어 마케팅을 넘어 전략 전장의 입체적 표현에도 통한다는 것을 입증했다. 이는 이후 Square Enix가 HD-2D를 다양한 장르에 적용하는 흐름의 한 분기점이 되었다.

### 클래식 SRPG 부흥의 한 축

본작의 상업적·평단적 성공은 "정통 정치 택틱스 RPG에 시장이 살아 있다"는 것을 증명했다. 이는 《Final Fantasy Tactics》 계열 명작을 재조명하는 분위기와 맞물렸고, 장르 부흥의 기대를 키웠다. 본작 스스로가 《FFT》의 정신적 후속작을 자임하며 그 공백을 메운 것은 산업적으로도 의미가 컸다.

### 멀티플랫폼 확장과 롱테일

초기 Switch 단독에 가깝던 출시 전략은 2022년 PC, 2024년 VR, 2025년 PS5·Xbox로 단계적으로 확장되었다. 단일 플랫폼 니치 작품으로 출발해 점진적 멀티플랫폼으로 수명을 늘리는 이 행보는, 중규모 IP를 장기 수익화하는 Square Enix의 전형적 패턴을 보여 준다.

### 문화적 의미

"선택에는 정답이 없고 모든 결정이 누군가의 희생을 동반한다"는 본작의 성숙한 도덕관, 그리고 그것을 **투표라는 집단 의사결정 메카닉**으로 게임화한 시도는, 도덕적 선택 시스템의 디자인 사례로 자주 언급된다. 단순 선악 슬라이더(예: Paragon/Renegade)를 넘어, 동료 설득과 다수결이라는 정치 과정 자체를 플레이로 만든 점에서 디자인적 참신함을 인정받았다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
|------|------|
| 개발 | Square Enix + Artdink |
| 퍼블리셔 | Square Enix |
| 프로듀서 | Tomoya Asano, Yasuaki Arai (Team Asano) |
| 시나리오 | Naoki Yamamoto |
| 캐릭터 디자인 | Naoki Ikushima |
| 음악 | Akira Senju (첫 전곡 게임 OST, 4 디스크) |
| 엔진/그래픽 | HD-2D (Unreal Engine 기반) |
| 장르 | 택틱스(턴제 전략) RPG |
| 출시 (Switch) | 2022-03-04 (전 세계) |
| 출시 (PC/Steam) | 2022-10-13 |
| 출시 (VR/Meta Quest) | 2024-10-31 |
| 출시 (PS5/Xbox) | 2025-08-20 |
| 엔딩 수 | 4종 (Utility/Morality/Liberty + Golden) |
| 플레이어블 캐릭터 | 약 30명 (1회차 전원 영입 불가) |
| 평론 점수 | IGN 8/10, GameSpot 8/10, Eurogamer 추천 |
| 판매 (2주) | 약 800,000장 출하(디지털 포함) |
| 판매 (2022-12) | 100만 장 돌파 (출하+디지털) |
| 수상 | TGA 2022 Best RPG 노미네이트 |

### 주요 인터뷰 및 자료

- Destructoid, "Triangle Strategy producers talk HD-2D, storytelling, and no permadeath" (Asano·Arai 인터뷰): https://www.destructoid.com/triangle-strategy-interview-producers-asano-arai-square-enix-hd-2d-tactics-rpg/
- Inverse, "Triangle Strategy Devs On Creating a 'Mature' Story": https://www.inverse.com/gaming/triangle-strategy-interview-hd-2d
- Kotaku, "Square Enix's New Tactical RPG Is Deeper Than Pixel Art Nostalgia": https://kotaku.com/triangle-strategy-octopath-traveler-final-fantasy-tacti-1848637430
- Kotaku, "How To Win Votes And Influence People In Triangle Strategy": https://kotaku.com/triangle-strategy-square-enix-scales-of-conviction-vote-1848657909

### 참고 자료 목록 (영어권 매체 중심)

- Wikipedia — Triangle Strategy: https://en.wikipedia.org/wiki/Triangle_Strategy
- Metacritic (Switch): https://www.metacritic.com/game/switch/triangle-strategy
- OpenCritic: https://opencritic.com/game/12840/triangle-strategy
- Gematsu — 100만 돌파 보도: https://www.gematsu.com/2022/12/triangle-strategy-shipments-and-digital-sales-top-one-million
- RPG Site — 100만 돌파: https://www.rpgsite.net/news/13632-triangle-strategy-surpasses-1-million-units-worldwide
- VGChartz — 약 80만 출하: https://www.vgchartz.com/article/452956/triangle-strategy-ships-nearly-800000-units-worldwide/
- Nintendo Life — 전투 시스템 가이드(TP·Quietus·Kudos): https://www.nintendolife.com/guides/triangle-strategy-tips-and-battle-tactics-walkthrough-tactical-points-phases-kudos-quietuses-guide
- Game Rant — Convictions and Choices Guide: https://gamerant.com/triangle-strategy-convictions-choices-scale-morality-utility-liberty/
- Game8 — Golden Route/Endings Guide: https://game8.co/games/Triangle-Strategy/archives/370301
- RPGFan — Original Soundtrack Music Review: https://www.rpgfan.com/music-review/triangle-strategy-original-soundtrack/
- CogConnected — PS5 Review (Brilliant Combat, Divisive Pacing): https://cogconnected.com/review/triangle-strategy-ps5-review/

---

*본 분석서는 영어권 매체·위키·개발자 인터뷰를 기반으로 작성되었으며, 판매·점수 수치는 각 출처 발표 기준이다.*
