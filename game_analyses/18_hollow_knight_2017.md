# Hollow Knight (2017) — 두 사람의 작은 게임 잼이 메트로배니아의 새 표준이 되기까지

> 호주 애들레이드의 무명 인디 스튜디오 Team Cherry가 만든 《Hollow Knight》는 "2시간짜리 작은 게임"으로 출발했지만, 결국 장르의 새로운 기준점이 되었다. 손으로 그린 멜랑콜리한 곤충 왕국 할로네스트(Hallownest), 정밀한 전투, 환경으로 서사를 풀어내는 절제된 스토리텔링. 이 분석서는 영어권 매체와 개발자 인터뷰를 바탕으로 이 게임이 무엇이며 왜 성공했는지를 추적한다.

---

## 1. 게임 개요

### 개발사 / 퍼블리셔 / 출시일

- **개발사 / 퍼블리셔**: Team Cherry (호주 남부 애들레이드 소재 인디 스튜디오, 자체 퍼블리싱)
- **장르**: 2D 사이드스크롤링 메트로배니아(Metroidvania) / 액션 어드벤처
- **엔진**: 초기 **Stencyl**로 프로토타이핑 → 이후 **Unity**로 전환 (Wikipedia)
- **플랫폼별 출시일** (Wikipedia 기준):
  | 플랫폼 | 출시일 |
  |---|---|
  | Windows (PC) | 2017년 2월 24일 |
  | Linux / macOS | 2017년 4월 11일 |
  | Nintendo Switch | 2018년 6월 12일 |
  | PlayStation 4 / Xbox One | 2018년 9월 25일 |
  | PS5 / Xbox Series X·S / Switch 2 (재발매) | 2026년 2월 5일 |

### 디렉터 / 주요 크레딧

Team Cherry는 사실상 핵심 인원 **두 명**으로 시작한 초소형 스튜디오였다. 후에 프로그래머 한 명이 합류하면서 3인 체제가 되었다.

- **Ari Gibson** — 디자이너 / 아티스트. 손으로 그린 비주얼 전체를 담당한 시각적 아이덴티티의 핵심.
- **William Pellen** — 디자이너 / 프로그래머. 게임 디자인과 코드 양쪽에 걸쳐 작업.
- **David Kazi** — 프로그래머(테크니컬 디렉터). Kickstarter 성공으로 추가 고용된 인력 (Wikipedia, MCV/DEVELOP).
- **Christopher Larkin** — 작곡가. Kickstarter 자금으로 합류한 외부 협력자.

### 개발 기간 / 개발 규모

- **착상**: 2013년 **Ludum Dare** 게임 잼에서 컨셉이 탄생했다 (Wikipedia).
- **Kickstarter**: 2014년 11월 캠페인 시작. 목표는 호주 달러 **A$35,000**.
- **모금 결과**: 2,158명의 후원자로부터 **A$57,000 이상**을 모금. 당초 "2시간 정도의 작은 게임"으로 기획했으나, 모금 초과 달성으로 스코프를 대폭 확장하고 추가 인력(David Kazi)과 작곡가(Christopher Larkin)를 고용할 수 있었다 (Wikipedia, GameRant, PledgeBox).
- **베타**: 2015년 9월 베타 상태 도달. 이후 스트레치 골(stretch goal)로 약속한 추가 콘텐츠를 계속 채워 넣으며 2017년 2월 정식 출시까지 약 2년여를 더 다듬었다.
- **개발 규모**: 핵심 2~3인 + 작곡가 외주. 인디 기준으로도 극도로 작은 팀이었다. "한 팀이 2명으로 1,350만 달러 이상의 매출을 만들어낸" 사례로 회자된다 (createleadsucceed.com).

### 기술 스택 (엔진 전환의 의미)

Stencyl(노코드/블록 기반 도구)에서 Unity로 옮긴 결정은 단순한 도구 교체 이상이었다. Team Cherry는 Unity의 내장 개발 도구와 Asset Store 확장 기능을 적극 활용해 기술적 부담을 덜고, 자신들이 가장 잘하는 것 — 즉 **아트** — 에 집중했다 (Made with Unity). 모든 비주얼은 Photoshop에서 손으로 그린 그림과 전통적 애니메이션 기법으로 제작되어 단순 PNG로 저장되었다. 즉, 화려한 기술 파이프라인이 아니라 "수공예적 그림 + 범용 엔진"이라는 조합이 이 게임의 핵심 미학을 가능하게 했다.

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 컨셉과 세계관

《Hollow Knight》는 지하 깊은 곳에 묻힌 곤충들의 멸망한 왕국 **할로네스트(Hallownest)**를 탐험하는 2D 메트로배니아다. 플레이어는 말 없는 곤충형 전사 **The Knight(기사)**를 조작하며, 못(Nail)이라 불리는 검 형태의 무기로 적을 베고, 진행하면서 원거리 마법을 습득한다 (Wikipedia).

세계관의 톤은 한마디로 **멜랑콜리(melancholy)**다. 폐허가 된 왕국, 거의 텅 빈 통로, 정체와 기원을 알 수 없는 이름 없는 주인공 — 이 모든 요소가 외로움, 신비, 상실감을 불러일으키도록 설계되었다 (firstsummoner.com, lifelessgame.com).

### 줄거리 [스포일러 포함]

> ⚠️ **[스포일러]** 아래는 핵심 줄거리와 결말을 포함한다.

할로네스트는 한때 **Pale King(창백한 왕)**이 다스리던 번영한 곤충 왕국이었다. Pale King은 본래 거대한 벌레(Wyrm)였으나 스스로 몸을 작게 줄여 다른 벌레들과 비슷한 형태가 되었고, 왕국의 벌레들에게 지성·통찰·지식을 부여했다 (FextraLife, GameRant).

비극의 씨앗은 **The Radiance(빛의 여신, 광휘)**였다. 나방 부족(Moth tribe)이 할로네스트에 합류하면서 잊혀진 존재가 된 Radiance는, 자신을 다시 기억하게 하려고 주민들의 꿈에 나타나기 시작했다. 이것이 **The Infection(역병/감염)**의 정체다 — 꿈을 통해 벌레들의 정신을 지배하고 광기와 불사(undeath)로 몰아넣는 초자연적 질병이다 (GameRant).

Pale King의 해법은 **Vessel(그릇)**이었다. 그는 White Lady와 함께 공허(Void)로 빈 존재 — 감정도 의지도 없는 "텅 빈" 생명체 — 를 만들어 그 안에 Radiance를 봉인하고자 했다. 이것이 타이틀의 **Hollow Knight(텅 빈 기사)**다. 그리고 세 명의 봉인 수호자(Dreamers) — City of Tears의 감시자 **Lurien**, 학자 **Monomon**, Deepnest의 여왕 **Herrah** — 가 그 봉인을 떠받쳤다.

그러나 계획은 실패했다. Hollow Knight의 껍데기에는 작은 결함 — 자신을 길러준 아버지 Pale King에 대한 **감정적 애착** — 이 있었고, 그 균열로 인해 감염이 새어 나와 왕국 전체로 퍼졌다 (Villains Wiki, GameRant).

플레이어가 조작하는 **The Knight** 역시 Pale King이 만든 수많은 폐기된 Vessel 중 하나다. "실패작"으로 판정되어 형제들과 함께 어둠 속에 버려졌으나, 일부가 탈출했고 그중 하나가 바로 주인공이다. 주인공은 감염의 근원을 마주하기 위해 할로네스트로 돌아온다.

### 다중 엔딩

플레이어의 행동에 따라 여러 결말이 갈린다 (Wikipedia, GameRant):

1. **The Hollow Knight** — 세 Dreamers를 처치하고 Black Egg의 신전에서 부패한 Hollow Knight를 쓰러뜨린 뒤, 주인공이 그 자리를 대신해 Radiance를 봉인한다.
2. **Sealed Siblings** — Hornet의 도움을 받아 Hollow Knight를 봉인한다.
3. **Dream No More** — Void Heart 등 추가 조건을 충족하면 꿈의 영역에서 **Radiance 본체를 직접 처치**해 감염의 순환 자체를 끊는다.

### 캐릭터 / 주요 NPC

- **The Knight** — 무언의 주인공. 정체성과 감정의 부재가 곧 서사적 핵심.
- **Hornet** — 빠르고 민첩한 송곳(needle) 사용자. 주인공을 시험하는 라이벌이자 후반의 조력자. 후속작 《Silksong》의 주인공이 된다.
- **Quirrel, Cornifer(지도 상인), Iselda, Zote, Elderbug, Hornet, The Grimm** 등 폐허 곳곳에 흩어진 인상적인 조연들이 단편적 대사로 세계를 채운다.
- **Pale King, White Lady, The Radiance, The Hollow Knight** — 직접 등장은 적지만 세계관을 떠받치는 신화적 존재들.

### 무드 / 톤 / 아트 디렉션

Ari Gibson의 손그림은 잉크 일러스트의 질감을 살린 2D 비주얼로, 각 지역이 뚜렷한 정체성을 가진다. 생기 넘치는 초록의 **Greenpath**, 끝없이 비가 내리는 우울한 **City of Tears**, 빛나는 **Crystal Peak**, 거미줄의 어둠 **Deepnest** 등 — 색채와 분위기의 대비가 곧 탐험의 동기가 된다 (lifelessgame.com, firstsummoner.com). 시각적 절제와 침묵, 멜랑콜리가 일관되게 흐른다.

### 사운드 / 음악

작곡가 **Christopher Larkin**(호주)이 만든 사운드트랙은 게임의 정체성을 결정짓는 핵심 요소다. Bandcamp Daily는 이를 "어둡고 우아하며 멜랑콜리한(dark elegance and melancholy)" 스코어로 평했다. 대부분 오케스트라 기반이며, 각 지역·캐릭터에 대응하는 **라이트모티프(leitmotif)**가 반복적으로 변주된다 (Bandcamp Daily, Wikipedia). 대표곡으로 메인 테마, "City of Tears", "Greenpath", "Resting Grounds", 그리고 Hornet 전투 테마 등이 꾸준히 회자된다. Larkin은 2017년 호주 ASSG(Australian Screen Sound Guild)에서 인터랙티브 미디어 부문 사운드상을 수상했다.

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

### 코어 게임플레이 루프 (모먼트-투-모먼트)

순간순간의 플레이는 **탐험 → 전투 → 발견(능력/지도/통화) → 더 넓은 영역 개방**의 메트로배니아 고리를 따른다. 그러나 Hollow Knight가 차별화되는 지점은 이 고리가 **명시적 안내 없이** 굴러간다는 데 있다. 새 지역에 처음 들어서면 지도가 없고, 방들의 외형이 유사해 길을 잃기 쉽다 — 이는 의도된 긴장감이다. 한 분석은 "새로운 지역에 처음 들어설 때 시각적 안내가 전혀 없어, 어둠 속으로 내딛는 한 걸음 한 걸음이 목숨을 건 도박처럼 느껴진다"고 표현했다 (paragraph.com/ludologist).

### 진행 구조 (맵 / 비선형)

할로네스트는 고유한 테마를 가진 여러 거대한 영역이 **상호 연결(interconnected)**된 단일 세계다. 비선형 디자인이라 한 가지 경로를 강요하지 않으며, 세계 전체를 다 탐험할 필요도 없다 (Wikipedia). 핵심은 영역들이 "레벨의 나열"이 아니라 **테마적·역사적 일관성을 가진 하나의 생태계**로 설계되었다는 점이다. 한 지역이 다른 지역의 존재 이유를 논리적으로 설명한다 (paragraph.com).

#### 지도(Map) 시스템

지도는 자동으로 채워지지 않는다. 각 영역에서 지도 상인 **Cornifer**를 먼저 찾아 지도를 구입해야 하고, 그마저도 벤치(저장 지점)에서 쉬어야 갱신된다. 위치를 표시하는 마커, 나침반(Wayward Compass 부적)조차 별도로 갖춰야 한다. 이 설계는 "탐험의 보상"을 강화하지만, 동시에 가장 큰 호불호 지점이기도 하다(6장 참조).

#### Fast Travel

**Stag Stations**(사슴벌레 역)을 통한 빠른 이동 시스템이 있어, 발견한 역들 사이를 오갈 수 있다 (Wikipedia).

### 전투 / 주요 메카닉의 정밀한 동작

#### 못(Nail)

기본 무기인 검 형태의 **Nail**로 상하좌우 4방향 공격이 가능하다. 특히 **아래 방향 공격(pogo/down-strike)**은 적이나 함정 위로 튕겨 오르는 데 사용되어, 전투와 플랫포밍이 결합되는 핵심 테크닉이다. Nail은 게임 진행에 따라 대장장이를 통해 업그레이드할 수 있다.

#### Soul(영혼) 시스템

적을 베면 **Soul**이 쌓여 **Soul Vessel**에 저장된다. 초기에는 Soul을 **Focus(집중)**에 써서 체력(마스크)을 회복하는 것이 전부지만, 진행하면서 Soul을 소모하는 **공격 마법**(Vengeful Spirit/Shade Soul, Desolate Dive 등)을 습득한다 (Wikipedia). 핵심 긴장은 여기서 발생한다 — Soul은 회복에도, 공격에도 쓰이므로, 전투 중 "지금 치유할 것인가, 더 공격할 것인가"를 끊임없이 저울질해야 한다. 또한 Focus는 즉시 발동되지 않고 충전 동작이 필요해, 안전하게 회복할 틈을 만드는 것 자체가 실력의 영역이 된다 (blog.rwittmann.com 전투 분석).

#### 체력(Masks)

체력은 **마스크(masks)**로 표현되며, 처음에는 5칸으로 시작한다. 지역에 흩어진 **Mask Shard**를 4개 모으면 마스크 1칸이 추가된다. 마찬가지로 **Vessel Fragment**를 모으면 Soul 저장 용량이 늘어난다.

#### Geo와 죽음 패널티 (Dark Souls식 Shade)

게임의 주 통화는 **Geo**다. 마스크를 모두 잃으면 죽고, 죽은 위치 근처에 **Shade(그림자)**가 생성되어 지도에 표시된다. 이때 보유한 Geo를 모두 잃고 Soul 저장 용량도 일시적으로 감소한다. 잃은 Geo와 용량을 되찾으려면 그 Shade를 처치해야 한다 (Wikipedia). 명백히 Dark Souls의 회수(corpse run) 시스템에서 영감을 받은 구조다.

### 부적(Charms) — 빌드 커스터마이징

**Charms(부적)**는 이 게임의 빌드/커스터마이징 축이다. Nail의 사거리 증가, Soul 획득 효율, 추가 체력, Shade 소환, 마법 강화 등 다양한 효과를 제공한다. 부적 장착은 한정된 **Charm Notch(부적 슬롯)** 자원을 소모하며, 강력한 부적일수록 더 많은 슬롯을 차지한다 (Wikipedia, NoobFeed). 슬롯이 제한적이므로 플레이어는 자신의 플레이 스타일에 맞춰 부적 조합을 끊임없이 재구성하게 된다 — 이것이 사실상 클래스/스킬트리 부재를 대체하는 핵심 진척 시스템이다.

### 자원 관리 / 진척도 시스템 정리

- **Geo**: 주 통화 — 상점 구매, 능력 잠금 해제.
- **Soul**: 치유와 마법의 공유 자원 — 전투의 핵심 긴장.
- **Mask Shard / Vessel Fragment**: 체력·Soul 용량 영구 확장 수집물.
- **Charm Notch**: 부적 빌드의 제약 자원.
- **Pale Ore**: Nail 업그레이드 재료.

업그레이드 페이싱은 의도적으로 후반에 무게를 둔다 — 한 비평가는 "Metroid에 비해 체력·Soul 업그레이드를 게임 후반부까지 별로 찾을 수 없다"고 지적했다 (gamecritics.com).

### 멀티 / 협력 시스템

해당 없음 — 순수 싱글플레이 게임이다.

### 라이브 운영 대신: 무료 DLC 4종

Hollow Knight는 시즌 패스나 MTX(소액결제)가 없다. 대신 출시 후 약 1년 반에 걸쳐 **네 개의 대형 무료 콘텐츠 팩**을 제공해, 사실상 정식판을 계속 확장했다 (Wikipedia):

1. **Hidden Dreams** (2017년 8월 3일) — 신규 보스 전투, 사운드트랙 추가.
2. **The Grimm Troupe** (2017년 10월 26일) — 퀘스트, 부적, 그리고 러시아어·포르투갈어·일본어 등 다국어 지원.
3. **Lifeblood** (2018년 4월 20일) — 최적화, 색 팔레트 개선, 신규 보스.
4. **Godmaster** (2018년 8월 23일) — 보스 러시 모드(Pantheons), Hall of Gods, 최고 난도 도전 콘텐츠.

이 무료 DLC 전략은 평단과 유저 모두에게 강력한 호평을 받았다. GameSpot 리뷰는 "긴 핵심 서사와 여러 무료 DLC 패키지에 걸친 막대한 양의 훌륭한 콘텐츠"를 장점으로 꼽았다.

### 난이도 / 접근성

기본 난이도가 상당히 높은 편이며, 별도 난이도 옵션은 없다. 대신 도전을 늘리는 방향의 **Steel Soul 모드(영구 사망, permadeath)**가 존재한다 (Wikipedia). 부적 조합을 통해 사실상 플레이어가 스스로 난이도를 조절(체력 부적 등)할 수 있는 여지가 있다.

### UI/UX 디자인 철학

인터페이스는 극도로 미니멀하다. HUD는 좌상단의 마스크와 Soul 게이지로 거의 전부이며, 화면 대부분을 비워 분위기를 살린다. "정보를 최소한으로 제시하고 세계 자체에 집중하게 한다"는 철학이 일관된다 (champicky.com 인터페이스 분석).

---

## 4. 평가

### Metacritic / OpenCritic

- **Metacritic** (Wikipedia 집계 기준): PC **87/100**, Nintendo Switch **90/100**("universal acclaim"), Xbox One **89/100**, PS4 **85/100**. Switch판이 가장 높은 점수를 받았다.
- **OpenCritic**: "Mighty" 등급, 평론가 73명 기준 평균 약 **89점**, 상위 **1%**, 평론가 **97%**가 추천 (Metacritic, OpenCritic).

### 주요 평론 인용

- **IGN — 9.4/10**: 분위기를 구축하는 "수백만 가지 디테일"을 극찬.
- **PC Gamer — 92/100**: "새로운 클래식(new classic)".
- **Eurogamer — "Recommended"**: "플레이어의 손을 잡아주지 않겠다는 점을 분명히 하는, 준엄하면서도 눈부신 2D 어드벤처(a stern yet scintillating 2D adventure that makes a point of not holding your hand)".
- **GameSpot — "An Exceptional Adventure"**: 탐험, 강렬한 전투, 아름다운 비주얼 디자인과 막대한 콘텐츠 분량을 호평.
- **Destructoid**: "올해 최고의 게임일 뿐 아니라, 현존하는 최고의 메트로배니아일지도 모른다… 진정한 게임의 걸작(masterpiece of gaming)".
- **Nintendo Life (Switch판)**: "Metroid도 Castlevania도 아니면서 최고의 메트로배니아 중 하나".

### 수상 이력

- **The Game Awards 2017** — Best Debut Indie Game **노미네이트**.
- **BAFTA Games Awards 2018** — Debut Game **노미네이트**.
- **Golden Joystick 2018** — Nintendo Game of the Year **노미네이트**.
- **Australian Games Awards 2018** — Independent Game of the Year, Developed Game of the Year **수상**.
- **NAVGTR (2019)** — Game Design, New IP 등 부문 **수상** 및 다수 노미네이트(Art Direction, Character Design, Original Action 등).
- **ASSG 2017** — Christopher Larkin, 인터랙티브 미디어 사운드 부문 **수상**.

(출처: Wikipedia, IMDb Awards)

### 상업 지표 (판매량 추이)

영어권 보도에 근거한 누적 판매 추이는 다음과 같다 (Wikipedia, Nintendo Life, LEVVVEL):

| 시점 | 누적 판매 |
|---|---|
| 2017년 11월 | 50만 장 이상 |
| 2018년 6월 (PC) | 100만 장 (Switch 출시 직전) |
| Switch 출시 후 2주 | Switch에서만 25만 장 이상 |
| 2018년 7월 | 120만 장 |
| 2019년 2월 | 280만 장 |
| 2025년 8월 | **1,500만 장 이상** |

매출 측면에서 Steam 단일 플랫폼만으로도 약 **$64M** 수준으로 추정되며, Godmaster·The Grimm Troupe 등 무료 DLC와 굿즈 판매까지 더하면 전체 재무 성과는 훨씬 크다 (LEVVVEL). 1,500만 장이라는 수치는 Castlevania나 Metroid **시리즈 전체 누적 판매**에 근접하는 규모로, 단일 인디 타이틀로서 비범한 성취다 (PC Gamer).

### 유저 평가

Steam에서 Hollow Knight는 "Metroidvania" 태그에서 평점 기준 1위(약 **96.08% 긍정**)를 기록하며 사실상 장르의 상징이 되었다 (PC Gamer). Reddit·Steam 커뮤니티의 장기적 평가도 압도적으로 호의적이며, "역사상 최고의 메트로배니아"라는 평가가 흔하다.

### 평론-유저 괴리

평론과 유저 평가 사이의 큰 괴리는 없다 — 양쪽 모두 매우 높다. 다만 **개별 디자인 요소(특히 지도 시스템과 안내 부재)**를 둘러싼 유저 내부의 호불호는 분명히 존재한다(6장 참조).

---

## 5. 성공 요인 분석 (핵심)

### 디자인 측면 성공 요인

1. **세계로서의 공간 설계** — Team Cherry는 환경을 "레벨의 연속"이 아니라 "세계와 공간"으로 사고했다. Pellen은 "세계와 공간으로 생각하면 그 안에 무엇을 넣을지 떠올리기가 훨씬 쉽다"고 말했다 (PC Gamer). 이 접근이 할로네스트의 유기적 상호연결성을 만들었다.
2. **환경 서사(Environmental storytelling)** — 직접 설명 대신, 폐허·대사·아이템 묘사를 통해 플레이어가 스스로 이야기를 짜맞추게 한다. 이는 "직접 추론해 얻은 성취감"을 준다 (firstsummoner.com).
3. **정밀한 컨트롤과 전투** — Soul의 이중 용도(치유/공격)가 만드는 긴장, pogo 점프의 손맛, 부적 빌드의 자유도가 결합되어 반복 플레이를 견디는 깊이를 만들었다.
4. **압도적 가성비** — 출시가가 매우 저렴($15 내외)했고, 네 개의 무료 DLC로 콘텐츠 분량이 비대해졌다. "가격 대비 콘텐츠"의 인식이 입소문을 가속했다.

### 마케팅 / 출시 전략

- **Kickstarter를 통한 초기 커뮤니티 형성** — 2,158명의 후원자가 초기 전도사가 되었다.
- **Switch 깜짝 출시** — 2018년 6월 E3 Nintendo Direct에서 발표 즉시 당일 eShop 출시. 이 "shadow drop"은 큰 화제를 만들었고, Switch에서 2주 만에 25만 장을 팔며 Nindies 프로그램 출범 이래 가장 성공적인 인디 중 하나가 되었다 (Wikipedia, Nintendo Life, Bleeding Cool).

### 타이밍 / 시장 환경

- **메트로배니아 르네상스의 한가운데** — Steam에 Hollow Knight 이전에도 150개 이상의 메트로배니아 태그 게임이 있었으나, 이후 1,350개 이상이 쏟아졌다. Hollow Knight는 이 흐름의 **변곡점**이 되었다 (PC Gamer).
- **Switch의 휴대형 인디 친화 생태계**와 맞물려, 짧은 세션으로 즐기기 좋은 탐험형 게임이 폭발적으로 확산됐다.

### 개발 / 운영 방법론

- **소규모·아트 집중 파이프라인** — Unity + Asset Store로 기술 부담을 덜고 손그림 아트에 자원을 집중한 전략적 선택.
- **출시 후 무료 확장** — 유료 시즌 패스 대신 무료 DLC로 신뢰와 호평을 쌓는 운영.

### 커뮤니티 / IP 효과

입소문(word of mouth)이 핵심 성장 동력이었다. 출시 초기 메가히트는 아니었으나, 평단의 극찬과 유저 추천이 누적되며 **롱테일**로 폭발적으로 성장했다(50만 → 1,500만). 후속작 《Silksong》에 대한 비정상적일 정도의 기대감 자체가 원작이 구축한 IP 충성도의 증거다.

### 동시기 작품 대비 차별점

- **Ori and the Blind Forest(2015)** 대비: Ori가 화려한 비주얼·감정 서사에 집중했다면, Hollow Knight는 **더 큰 비선형 세계, 더 어려운 전투, 더 절제된 멜랑콜리한 스토리텔링**으로 차별화했다.
- **Dead Cells(2018), Bloodstained(2019)** 등 동시기 메트로배니아 대비: Hollow Knight는 **분위기와 세계의 깊이**에서 독보적이라는 평가를 얻으며 사실상 "기준점"이 되었다.

---

## 6. 비평적 시각 / 한계 / 논란

### 디자인적 약점

1. **지도·길안내 시스템** — 가장 큰 호불호 지점. 비판자들은 "거대한 미로 같은 게임에서 지도가 전혀 도움이 안 되는 반대 극단으로 치우쳤다"고 지적한다. 많은 방의 외형이 비슷해 길을 잃기 쉽고, 각 영역마다 지도 상인 Cornifer를 먼저 찾아야 한다는 점이 탐험의 보상감보다 짜증을 더한다는 의견이 있다 (ResetEra, Steam Community, NeoGAF, LevelUpTalk).
2. **방향성 부재** — "어디로 가야 할지 전혀 알 수 없어 엉뚱한 방향으로 몇 시간을 헤맸다"는 호소가 흔하다. 의도된 모호함이 누군가에겐 몰입을, 누군가에겐 좌절을 준다.
3. **후반 백트래킹** — 후반부로 갈수록 백트래킹이 많아지는데, 새 능력을 어디에 써야 할지 알려주는 맵 마커가 부족하다는 비판이 있다 (gamecritics.com).
4. **업그레이드 페이싱** — 체력·Soul 강화가 후반에 몰려 있어 초반 진입 장벽이 가파르다는 지적 (gamecritics.com).

### 운영 / 논란 이슈

원작 자체에는 큰 운영 논란이 없었다. 다만 산업적 맥락에서 가장 큰 "논란"은 후속작 **《Silksong》의 극단적인 개발 지연**이었다. 2019년 발표 후 수년간 침묵이 이어지며 커뮤니티의 밈과 좌절이 누적됐다(2025년 9월 출시로 마침내 해소). Kotaku 인터뷰에서 개발진 스스로 "이렇게 오래 걸릴 줄 몰랐다"고 인정했다 (Kotaku).

### 평가가 갈리는 지점

- "의도된 길 잃음"을 디자인의 미덕으로 보는 측 vs. 불친절·시간 낭비로 보는 측.
- 높은 난이도와 가혹한 죽음 패널티(Shade 회수)를 "긴장과 성취"로 보는 측 vs. 진입 장벽으로 보는 측.
- 절제된(모호한) 서사를 "깊이"로 보는 측 vs. "현학적이고 혼란스럽다(pretentious and confusing)"고 보는 측 (Steam Community 토론).

---

## 7. 영향과 유산

### 장르에 미친 영향

Hollow Knight는 메트로배니아의 **사실상의 새로운 템플릿**이 되었다. Steam의 메트로배니아 태그에서 평점 1위를 유지하며, 후속작 Silksong이 2위에 자리한다 (PC Gamer). 1,500만 장이라는 누적 판매는 단일 인디가 도달한 보기 드문 수준으로, Castlevania·Metroid 시리즈 전체 누적에 근접한다.

흥미롭게도 Team Cherry는 처음부터 "메트로배니아"라는 라벨을 의도적으로 **피했다**. 2017년 인터뷰에서 Pellen은 그 명칭에서 "완전히 거리를 뒀다"고 했고, Gibson은 "장르가 우리의 디자인 결정을 좌우하게 두고 싶지 않았다"고 말했다. 그럼에도 불구하고 — PC Gamer의 표현을 빌리면 — 그들은 "**우연히, 이후 모든 게임이(심지어 Silksong조차) 마주해야 할 기준을 세워버렸다**" (PC Gamer).

### 후속작 / 모방작 / 장르 확장

- **Hollow Knight: Silksong (2025년 9월 4일 출시)** — Hornet을 주인공으로, 새로운 왕국 Pharloom을 무대로 한 후속작. 출시 직후 막대한 판매와 평단 호평을 기록했다(Steam Awards 2025 올해의 게임 등). Sea of Sorrow 확장도 예고됐다 (Wikipedia, PC Gamer).
- 이후 출시된 수많은 메트로배니아가 Hollow Knight의 세계 설계·환경 서사·전투 페이싱을 명시적으로 참고했다.

### 산업적 의미

- **인디의 가능성 증명** — 핵심 2~3인 팀이 Kickstarter A$57,000에서 출발해 1,500만 장·수천만 달러 매출에 도달한 것은, "작은 팀 + 명확한 비전 + 장기 입소문"이 메가히트로 이어질 수 있음을 보여준 상징적 사례다.
- **무료 DLC 운영의 모범** — 시즌 패스 없이 무료 확장으로 신뢰를 쌓는 모델의 성공 사례.

### 문화적 의미

할로네스트의 멜랑콜리한 분위기, Hornet, City of Tears 음악 등은 인디 게임 문화의 아이콘이 되었다. Silksong을 둘러싼 수년간의 커뮤니티 밈은 이 IP가 단순한 게임을 넘어 하나의 문화 현상이 되었음을 방증한다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
|---|---|
| 개발사 | Team Cherry (호주 애들레이드) |
| 핵심 인원 | Ari Gibson, William Pellen, David Kazi (+작곡 Christopher Larkin) |
| 엔진 | Stencyl → Unity |
| Kickstarter | 2014.11, 목표 A$35,000 / 모금 A$57,000+ (후원자 2,158명) |
| PC 출시 | 2017.2.24 |
| Switch 출시 | 2018.6.12 (E3 깜짝 출시) |
| Metacritic | Switch 90 / Xbox One 89 / PC 87 / PS4 85 |
| OpenCritic | "Mighty", 평균 ~89, 추천율 97% |
| 누적 판매 | 50만(2017.11) → 280만(2019.2) → 1,500만+(2025.8) |
| Steam 추정 매출 | 약 $64M (LEVVVEL) |
| 무료 DLC | Hidden Dreams, The Grimm Troupe, Lifeblood, Godmaster |
| 후속작 | Hollow Knight: Silksong (2025.9.4) |

### 주요 인터뷰 / 자료

- MCV/DEVELOP, "When We Made… Hollow Knight" — 개발 회고.
- ACMI, "From Ludum Dare to Pharloom" — Team Cherry 인터뷰.
- Source Gaming(2025.4), "Straight from the Source: Ari Gibson & William Pellen".
- Kotaku — Silksong 개발 지연에 대한 Team Cherry 인터뷰.
- Bandcamp Daily — Christopher Larkin 사운드트랙 분석.
- Limelight Arts — Larkin, "On scoring Hollow Knight".

### 게임 디자인 분석 자료

- Game Developer(Gamasutra), "The Surreal Philosophy of Hollow Knight".
- paragraph.com/ludologist, "Architecture of Silence and Melancholy" — 메트로배니아 패러다임 분석.
- blog.rwittmann.com, "The Combat of Hollow Knight" — 전투 시스템 정밀 분석.

### 참고 자료 목록 (영어권 매체 중심)

- [Hollow Knight — Wikipedia](https://en.wikipedia.org/wiki/Hollow_Knight)
- [Hollow Knight — Metacritic](https://www.metacritic.com/game/hollow-knight/)
- [Hollow Knight — OpenCritic](https://opencritic.com/game/4002/hollow-knight)
- [Hollow Knight Review — GameSpot](https://www.gamespot.com/reviews/hollow-knight-review-an-exceptional-adventure/1900-6416972/)
- [Review: Hollow Knight — Destructoid](https://www.destructoid.com/reviews/review-hollow-knight/)
- [Hollow Knight Review (Switch) — Nintendo Life](https://www.nintendolife.com/reviews/switch-eshop/hollow-knight)
- [Hollow Knight sold 250k on Switch in two weeks — Nintendo Life](https://www.nintendolife.com/news/2018/06/hollow_knight_sold_over_a_quarter_of_a_million_copies_on_switch_in_two_weeks)
- [When We Made… Hollow Knight — MCV/DEVELOP](https://mcvuk.com/development-news/when-we-made-hollow-knight/)
- [Hollow Knight — Made with Unity](https://unity.com/made-with-unity/hollow-knight)
- [Hollow Knight statistics — LEVVVEL](https://levvvel.com/hollow-knight-statistics/)
- [Team Cherry didn't want the 'metroidvania' label — PC Gamer](https://www.pcgamer.com/gaming-industry/hollow-knights-creators-didnt-want-to-be-constrained-by-the-metroidvania-label-but-they-accidentally-set-a-standard-that-every-game-since-even-silksong-has-to-reckon-with/)
- [Hollow Knight's Story and Lore Explained — GameRant](https://gamerant.com/hollow-knight-story-lore-void-radiance-pale-king-hornet-explained/)
- [The Pale King — Hollow Knight Wiki (FextraLife)](https://hollowknight.wiki.fextralife.com/The+Pale+King)
- [Inside Christopher Larkin's Score — Bandcamp Daily](https://daily.bandcamp.com/features/christopher-larkin-review)
- [Christopher Larkin — Wikipedia](https://en.wikipedia.org/wiki/Christopher_Larkin_(composer))
- [The Surreal Philosophy of Hollow Knight — Game Developer](https://www.gamedeveloper.com/design/the-surreal-philosophy-of-hollow-knight)
- [Hollow Knight: Silksong — Wikipedia](https://en.wikipedia.org/wiki/Hollow_Knight:_Silksong)
- [Silksong devs interview — Kotaku](https://kotaku.com/silksong-interview-delay-hollow-knight-team-cherry-2000619168)
- [Is the map system really that troublesome? — ResetEra](https://www.resetera.com/threads/lttp-hollow-knight-is-this-map-system-really-that-troublesome-for-some-people.150423/)

---

*본 분석서는 영어권 매체·공식 인터뷰·개발자 발언을 바탕으로 작성되었으며, 판매·점수 등 모든 수치는 본문에 출처를 명시했다. 일부 매출 추정치(예: Steam $64M)는 제3자 통계 사이트 추정값임을 밝힌다.*
