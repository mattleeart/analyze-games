# 《Samurai Shodown》 (2019) 심층 분석

> 한 번의 칼질이 곧 죽음이자 승리다. 11년의 공백을 끝내고 돌아온 SNK 검극(劍戟) 격투의 부활.

---

## 1. 게임 개요

《Samurai Shodown》(2019, 일본어 원제 《サムライスピリッツ / Samurai Spirits》)은 일본의 격투 게임 명가 **SNK**가 자사의 전통 무기 격투 시리즈를 11년 만에 되살린 리부트 작품이다. 시리즈의 정식 넘버링으로는 12번째 본편이며, 직전 본편이었던 2008년 《Samurai Shodown Sen》 이후 처음 나온 메인라인 신작이다. 단순한 속편이 아니라 시리즈 전체를 새로 출발시키는 의도로 만들어졌기에, 영어권 매체와 SNK 모두 이 작품을 일관되게 "reboot"로 칭한다.

- **개발사**: SNK (사내 KOF Studio 조직이 주도)
- **퍼블리셔**: SNK(일본) / Athlon Games(PS4·Xbox One 서구권) / Taito(아케이드) / Deep Silver(Nintendo Switch) / Netflix(모바일)
- **장르**: 2D(연출은 3D) 대전 격투 — 무기 기반(weapon-based) 격투
- **엔진**: Unreal Engine 4 (SNK 최초의 UE4 채택작)
- **플랫폼·출시일**:
  - PlayStation 4 / Xbox One — 2019년 6월 25일(전 세계), 6월 27일(일본)
  - 아케이드(Taito Type X 계열) — 2019년 10월 24일(일본)
  - Google Stadia — 2019년 11월 19일
  - Nintendo Switch — 2019년 12월 12일(일본), 2020년 2월 25일(전 세계)
  - Windows(PC) — 2020년 6월 11일(Epic Games Store), 2021년 6월 14일(Steam)
  - Xbox Series X|S — 2021년 3월 16일(120fps 지원)
  - 모바일(Netflix Games) — 2023년 8월 29일

**주요 크레딧**

- **디렉터**: Nobuyuki Kuroki(쿠로키 노부유키). 디렉터이자 아트 책임자로, 작품의 비주얼 톤과 게임 디자인 방향을 동시에 쥐었다.
- **프로듀서**: Yasuyuki Oda(오다 야스유키). 이후 《The King of Fighters XV》 등 SNK 격투 라인의 핵심 프로듀서로 시리즈 전체를 통할했다.
- **캐릭터 디자인**: Yumi Saji.
- **음악**: SNK Sound Team 명의. Hiroshi Yamazoe(야마조에 히로시)를 메인으로 Masato Horiuchi, Hideki "sha-v" Asanaka, Mayuko Hino, Naoki Kita, Kensuke Inage, Jun Hoshina, Minori Sasaki 등 다수가 참여.

엔진 선택은 이 작품을 이해하는 첫 단추다. SNK 회장 Zhihui Ge(거 즈후이)는 향후 SNK 격투 게임이 Unreal Engine 4를 표준으로 쓸 것이라고 밝혔고, 《Samurai Shodown》은 그 첫 실현이었다. SNK는 그동안 자체 스프라이트·렌더링 파이프라인에 의존해 왔으나, UE4로 전환하면서 멀티 플랫폼 포팅의 용이함과 셰이더·라이팅 표현력의 큰 도약을 한꺼번에 얻었다. 쿠로키 디렉터는 Unreal Engine 공식 개발자 인터뷰에서 "전통 일본 회화를 현대 애니메이션·만화 감각과 결합해 지금 플레이할 수 있는 《Samurai Shodown》의 스타일에 도달했다"라고 밝혔고, 고품질 그래픽 에셋 제작이 "극도로 쉬웠으며, 내가 하고 싶은 것에 대한 완전한 통제권을 가진 느낌"이었다고 회고했다. ([Unreal Engine 개발자 인터뷰](https://www.unrealengine.com/en-US/developer-interviews/unreal-engine-provided-robust-artistic-tools-that-empowered-snk-to-make-the-most-beautiful-samurai-shodown-yet), [PCGamesN](https://www.pcgamesn.com/samurai-shodown/making-it-in-unreal-samurai-shodown))

---

## 2. 게임 설명 — 이 게임이 무엇인가

### 컨셉과 정체성

《Samurai Shodown》은 1993년 첫 작품으로 격투 게임 장르에 충격을 준 시리즈의 정통 후예다. 당시 《Street Fighter II》가 정의한 "맨주먹 콤보" 격투의 시대에, SNK는 **칼·창·도끼 같은 무기를 든 사무라이들이 단 몇 합으로 승부를 가르는** 전혀 다른 결의 격투를 제시했다. 작은 실수 하나가 치명상으로 직결되는 긴장감, 베일 때 튀는 핏물과 효과음, 결정타 한 방의 무게가 이 시리즈의 정체성이다. 2019년 리부트는 바로 이 "검극의 무게"를 현대 하드웨어와 UE4의 표현력으로 복원하는 것을 목표로 삼았다.

### 세계관과 줄거리 [일부 스포일러 포함]

배경은 **1787년, 일본 에도 시대 후기 덴메이(天明) 시대**다. 시리즈 연표상으로는 《Samurai Shodown V》와 오리지널 1993년작 사이에 위치하는 "프리퀄/사이 시기" 이야기로, 익숙한 캐릭터들의 조금 더 젊은 시절을 그린다. 덴메이 시대는 실제로 대기근과 화산 분화(아사마산 분화), 사회 불안이 겹친 격동기였고, 게임은 이 음울한 시대상을 배경으로 초자연적 위협을 얹는다.

[스포일러] 최종 보스는 **Shizuka Gozen(시즈카 고젠)**으로, 요미(게임 내에서는 "Eternity/영원"으로 표기)에 사로잡힌 채 무언가에 빙의된 죽은 여인의 영혼이다. 그녀는 일본 전토를 파멸로 몰아넣으려 하며, 각 캐릭터의 스토리 모드는 이 위협을 둘러싼 개별 동기로 수렴한다. 시즈카 고젠이라는 이름 자체가 일본 역사·전설 속 시라뵤시(白拍子, 무희) 시즈카 고젠에서 따온 것으로, 시대극적 분위기를 강화한다.

### 캐릭터

기본 출시 로스터는 **16명**으로, 시리즈 베테랑 13명과 신규 3명, 그리고 신규 최종 보스로 구성됐다.

- **귀환 베테랑**: Haohmaru(하오마루, 시리즈 간판 사무라이), Nakoruru(나코루루, 아이누 소녀 검사), Genjuro Kibagami, Ukyo Tachibana, Yoshitora Tokugawa, Earthquake(거구의 도적), Jubei Yagyu, Galford(닌자견 Poppy 동반), Charlotte(프랑스 검사), Hanzo Hattori, Tam Tam, Kyoshiro Senryo, Shiki.
- **신규 캐릭터**: **Darli Dagger**(거대한 톱검을 휘두르는 여성 조선공/뱃사람으로 강렬한 개성), **Wu-Ruixiang**(중국 도교 소녀), **Yashamaru Kurama**(이번 작의 신규 미남 사무라이).

이후 DLC로 로스터가 크게 확장됐다. **시즌 1**은 Rimururu, Basara, Kazuki Kazama, Wan-Fu, Mina Majikina, Sogetsu Kazama, Iroha, Shizumaru Hisame 등 시리즈 베테랑과 더불어, 외부 IP 게스트로 《For Honor》의 **Warden**과 《Honor of Kings(왕자영요)》의 **Gongsun Li(공손리)**가 참전했다. **시즌 2**에는 Cham Cham, Hibiki Takane, Shiro Tokisada Amakusa, 그리고 《Guilty Gear》의 인기 캐릭터 **Baiken(바이켄)**이 게스트로 합류했다. 게스트 캐릭터 비중이 높은 점은 이 시기 SNK가 글로벌 협업과 IP 교류에 적극적이었음을 보여준다.

### 무드·아트 디렉션·사운드

비주얼은 한 폭의 우키요에·수묵화를 움직이는 것 같은 인상을 노린다. UE4 기반의 3D 모델을 쓰되, 외곽선과 색조를 회화적으로 다듬어 "움직이는 일본화"라는 평을 얻었다. 캐릭터가 베일 때의 거친 붓 터치 같은 핏자국 연출, 결정타가 들어갈 때 화면이 멎으며 클로즈업되는 연출은 한 합 한 합의 무게를 시각적으로 증폭한다.

음악(SNK Sound Team)은 일본 전통 악기(샤쿠하치, 고토, 타이코 등)의 음색을 현대적 편곡과 섞어 시대극 무드를 진하게 깐다. 사운드 디자인에서 특히 칼이 맞부딪치는 금속음, 베기와 막기의 타격감은 이 시리즈가 자랑하는 "베는 손맛"을 청각적으로 떠받친다. 사운드트랙은 별도 CD·바이닐로도 발매됐다.

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

《Samurai Shodown》(2019)의 설계 철학은 한 문장으로 요약된다. **"플레이어는 늘 죽음에서 한 칼, 승리에서 한 칼 떨어져 있다(one strike away from death, one strike away from victory)."** 이는 단순한 마케팅 문구가 아니라 모든 시스템을 관통하는 디자인 원리다.

### 코어 게임플레이 루프 — 콤보가 아니라 뉴트럴

현대 격투 게임 다수가 긴 콤보, 화려한 연계, 자원 폭발 위주로 흘러간 데 반해, 이 작품은 **의도적으로 콤보 중심이 아니다**. 대신 "뉴트럴 게임(neutral game)" — 즉 서로의 간격을 재고 상대의 행동을 읽으며 결정타를 노리는 풋시(footsies)가 절대적으로 중요하다. 이동은 느리고 신중하며, 그 느린 호흡을 보상하듯 **한 방의 데미지가 막대하다**. 강베기 한두 방이면 라운드가 끝날 수 있어, 한 라운드가 단 서너 번의 유효타로 종결되는 경우가 흔하다. EventHubs는 이를 "기본기는 단순하지만 깊이로 가득 찬(basic yet brimming with depth) 뉴트럴 중심 격투 게임"이라 요약했다. ([EventHubs 리뷰](https://www.eventhubs.com/news/2019/jun/24/samurai-shodown-review-neutral-focused-fighting-game-s-basic-yet-brimming-depth/))

공격 체계는 **약·중·강 베기(slash) + 발차기(kick)**의 4버튼 골격을 따른다. 약공은 빠르지만 데미지가 작고, 강베기는 느리지만 막히지 않고 들어가면 체력의 큰 덩어리를 가져간다. 이 위험-보상 곡선이 모든 교전을 "지를 것인가, 읽을 것인가"의 심리전으로 바꾼다.

### Rage(분노) 게이지 — 작품의 심장

체력 게이지 아래에 위치한 Rage(분노) 게이지가 시스템의 중심이다. 피격을 당할수록(특히 데미지를 입을수록) Rage가 차오르며, 이는 "역전의 자원"으로 기능한다. Rage가 일정 수준(MAX)에 이르면 다음의 강력한 옵션들이 열린다.

- **Rage Explosion(분노 폭발)**: 한 경기에 단 한 번, 원하는 타이밍에 발동할 수 있는 강화 상태다. 발동하면 Rage 게이지를 통째로 소모하지만, 지속 시간 동안 **모든 공격 데미지가 40% 증가**하고 가드 캔슬 등 부가 이점을 얻는다. 핵심 디테일은 **발동 시 체력이 낮을수록 지속 시간이 길어진다**는 점으로, 이는 코너에 몰린 약자에게 역전의 창을 의도적으로 더 크게 열어주는 "고무줄(rubber-band)" 설계다. 단, 한 번 쓰고 나면 그 라운드 내내 Rage 관련 자원을 다시 쓸 수 없다는 대가가 따른다.

- **Super Special Move(초필살기) / 무기 날리기 기술(Weapon-Flipping Technique)**: Rage가 MAX이거나 Rage Explosion이 활성화된 동안 1회 발동 가능한 초강력 기술이다. 명중 시 막대한 데미지를 주거나, 무기 날리기 버전(예: 236B+C)이 명중하면 **상대의 무기를 떨어뜨려(disarm)** 일정 시간 맨손 상태로 만든다. 무기를 잃은 쪽은 데미지·리치가 급감해 사실상 절체절명에 몰린다. 이 역시 한 경기 1회 제한이 걸려 있어, 언제 칼을 던질지의 판단 자체가 거대한 전략적 도박이 된다.

- **Lightning Blade(번개 칼날, 일본판 "이센/잇센")**: Rage Explosion 도중에만 발동할 수 있는 돌진 일격기로, 발동 시점에 남아 있는 게이지 양에 비례해 데미지가 결정된다. 게이지를 거의 다 남긴 채 초반에 성공시키면 한 방으로 라운드를 끝낼 수 있는 즉사급 위력을 낸다. 이는 "한 칼의 무게"라는 철학을 극단까지 밀어붙인 장치다.

이 세 가지 분노 옵션은 모두 "1회성"이라는 공통점을 가진다. 즉 게임은 자원을 풍부하게 쥐여주고 반복 사용하게 만드는 대신, **단 한 번의 결단**으로 판을 뒤집게 설계됐다. 패배 직전의 플레이어가 Rage Explosion + 무기 날리기 + Lightning Blade로 순식간에 역전하는 그림은 이 게임의 시그니처 드라마다.

### 방어·심리전 시스템

- **칼 막기·받아치기(Parry/Deflect)**: 절묘한 타이밍에 상대의 베기를 받아넘기면 빈틈을 강제해 반격 기회를 잡는다. 콤보가 없는 만큼, 한 합의 공방에서 "막고 되갚는" 정확도가 승패를 가른다.
- **무기 부딪힘(Weapon Clash)**: 같은 세기의 베기가 맞부딪치면 버튼 연타로 힘겨루기를 벌이고, 패한 쪽이 무기를 놓치는 연출이 발생한다. 이는 한 합의 정면 충돌에 도박성과 긴장을 더한다.
- **회피·구르기·뒤로 도약** 등 기동 옵션이 있으나, 전반적으로 느린 템포 위에서 신중하게 쓰이도록 설계됐다.

### Dojo(도장) 모드와 "Ghost" AI — 기계 학습의 실험

이 작품의 가장 야심찬 시스템은 단연 **Dojo 모드의 "Ghost"** 기능이다. SNK는 딥러닝 기반 AI 기술을 도입해, 플레이어가 오프라인 모드(스토리·대전·서바이벌 등)에서 싸우는 동안 그 행동 패턴·전술을 관찰·학습·계산·매핑한다고 밝혔다. 이렇게 만들어진 "Ghost(고스트)" 아바타는 플레이어의 버릇을 모사한 AI 대전 상대가 되며, **온라인을 통해 다른 플레이어의 고스트를 내려받아 대결**할 수도 있다. 100명의 AI를 연속으로 상대하는 "Ironman Challenge(아이언맨 챌린지)" 같은 변형 모드도 제공됐다. ([GameSpot — 딥러닝 AI 기사](https://www.gamespot.com/articles/samurai-shodown-uses-deep-machine-learning-to-crea/1100-6465815/))

이는 2019년 격투 게임으로서는 매우 앞선 시도였고 발표 당시 큰 화제를 모았다. 다만 실제 체감 완성도는 기대에 못 미쳤다(6장 참조).

### 게임 모드·UI·접근성

싱글 콘텐츠로는 캐릭터별 스토리 모드, 서바이벌, 시간 공격, 도장(Ghost) 등이 제공된다. 다만 출시 시점의 모드 구성은 동시기 대형 격투 게임에 비해 빈약하다는 지적을 받았다. UI는 시대극 무드에 맞춰 절제됐으며, 콤보 의존도가 낮은 만큼 입력 난이도 진입 장벽이 비교적 낮아 초심자도 "한 방의 손맛"을 빨리 체험할 수 있다는 접근성상의 장점이 있었다.

### 온라인·넷코드 (출시 시점의 한계)

출시 당시 온라인 대전은 **딜레이 기반(delay-based) 넷코드**를 채택했는데, 반응 속도가 승패를 좌우하는 이 게임 특성상 치명적이었다. 입력 지연이 풋시와 받아치기를 망가뜨려 온라인 경험이 크게 손상됐다. SNK는 수년 뒤 **GGPO 기반 롤백 넷코드**를 도입했는데, PC(Steam)에는 2023년 12월 14일, 콘솔에는 2024년 5월 22일에 적용됐다. 2023년 초 롤백 베타는 디싱크·버그로 출발이 순탄치 않았으나, 최종적으로 온라인 환경은 크게 개선됐다. ([EventHubs — 롤백 베타](https://www.eventhubs.com/news/2023/feb/10/samurai-shodown-rollback-beta-bugs/))

---

## 4. 평가

### 평론 점수 (Metacritic / OpenCritic)

플랫폼별 Metacritic 점수는 다음과 같다.

| 플랫폼 | Metacritic 점수 |
|---|---|
| PlayStation 4 | 81/100 |
| Xbox One | 78/100 |
| PC(Windows) | 76/100 |
| Nintendo Switch | 75/100 |

PS4 기준 81점은 "generally favorable(대체로 우호적)" 구간으로, 11년 만의 시리즈 부활로서는 매우 성공적인 점수다.

### 주요 매체 인용

- **IGN — 8.2/10** (리뷰어 Mitchell Saltzman): "현재의 격투 게임 풍토에서 거의 유일무이하게 극도로 긴장감 넘치는 싸움(extraordinarily tense style of fighting unlike just about anything else in the genre)"이라며 전투 메카닉을 극찬했다.
- **GameSpot — 8/10**: "훌륭한 리부트(a great reboot)"로, 원작을 재미있고 독특하게 만들었던 핵심을 잘 포착했다고 평했다. 다만 싱글플레이 경험이 다소 빈약하다는 점을 함께 지적했다.
- **Eurogamer — 4/5** (리뷰어 Martin Robinson): "SNK의 상징적 시리즈가 기능(콘텐츠)은 부족하지만 시스템은 풍부한 리부트로 돌아왔다(short on features but rich in systems)."
- **Game Informer — 7.75/10**: "거친 모서리가 있는 강렬한 귀환(An Intense Return With Rough Edges)"이라는 제목으로, 전투의 긴장감을 높이 사면서도 콘텐츠·온라인의 미흡함을 한계로 짚었다.

평론의 공통 패턴은 명확하다. **전투 핵심(긴장감 있는 검극, 한 방의 무게, 뉴트럴 깊이)은 격찬, 주변부(싱글 모드 분량, 캐릭터 수, 온라인 넷코드, 로딩 시간, 스토리 모드)는 비판**이라는 구도다.

### 수상·노미네이트

- **The Game Awards 2019** — Best Fighting Game 후보.
- **23rd D.I.C.E. Awards** — Fighting Game of the Year 후보.
- **NAVGTR Awards** — Game, Franchise Fighting 수상.
- **EventHubs 커뮤니티 투표** — 2019년 "올해의 격투 게임"에 선정되며 격투 게임 코어 팬덤의 높은 지지를 입증했다. ([EventHubs](https://www.eventhubs.com/news/2019/dec/26/what-best-fighting-game-2019/))

### 상업 지표

- 일본 PS4 첫 주: 실판매 16,662장으로 주간 4위(2019년 6월 24~30일 차트).
- 첫 주 출하+디지털 합산: **40,606장**(피지컬 30,179 + 디지털 10,427, 2019년 7월 4일 집계). 이는 같은 시기 일본 첫 주 기준으로 《The King of Fighters XIV》(2016, 20,655장)의 **약 두 배**, 《Soulcalibur VI》(24,049장)·《Dead or Alive 6》(26,442장)를 웃돌며 《Street Fighter V》 일본 첫 주(41,990장)에 근접하는 수치였다. ([Gematsu](https://www.gematsu.com/2019/07/samurai-shodown-ps4-shipments-and-digital-sales-top-40606-in-japan), [EventHubs](https://www.eventhubs.com/news/2019/jul/05/samurai-shodowns-launch-sales-japan-doubled-king-fighters-14-its-first-week/))
- SNK는 2019년 투자자 미팅에서 강한 사전 예약 덕에 《Samurai Shodown》이 이미 **흑자 전환**했다고 보고했다. 디렉터는 PC 독점 계약(판매를 제한할 수 있는)을 거절하면서 "이 게임은 100만 장 이상 팔릴 것"이라는 자신감을 내비쳤다.

### 유저 평가와 평론-유저 괴리

격투 게임 코어 커뮤니티(EVO 참가자, FGC)에서의 지지는 뜨거웠다. **EVO 2019에서 약 1,700명이 참가 등록**해 같은 해 《Mortal Kombat 11》의 엔트리를 능가했고, SNK 타이틀로서는 기록적인 규모였다. 반면 라이트 유저층에서는 빈약한 싱글 콘텐츠와 열악한 출시 넷코드 탓에 체감 만족도가 갈렸다. "전투는 최고지만 패키지는 미완성"이라는 평가가 평론과 유저 모두에서 반복됐다.

---

## 5. 성공 요인 분석 (핵심)

### (1) "콤보의 시대"에 대한 역행이라는 차별화

2019년 격투 게임 시장은 점점 더 복잡한 콤보, 자원 시스템, 가드 게이지로 무거워지고 있었다. 《Samurai Shodown》은 그 흐름을 정면으로 거슬러 **"단순하지만 깊은" 뉴트럴 중심 격투**를 제시했다. 콤보 암기 부담이 적어 신규·복귀 유저가 진입하기 쉬우면서도, 풋시·심리전의 천장이 매우 높아 코어 유저가 파고들 깊이가 충분했다. 이 "낮은 진입 장벽 + 높은 숙련 천장"의 조합은 격투 게임 디자인의 이상적 형태로 평가받았고, 시장 내에서 명확한 정체성을 확보했다.

### (2) 시리즈 정체성의 정확한 복원

리부트의 가장 큰 함정은 "원작의 무엇을 지키고 무엇을 바꿀지"의 판단이다. SNK는 시리즈의 핵심 — **한 합의 무게, 베는 손맛, 한 방 역전의 드라마** — 을 명확히 식별하고 그것을 디자인의 중심에 두었다. 동시에 Rage Explosion·Dojo Ghost 같은 신규 레이어를 얹어 현대적 신선함을 더했다. "바꾸지 말아야 할 것을 정확히 알았다"는 점이 평론의 호의를 끌어낸 결정적 요인이다.

### (3) Unreal Engine 4로의 전환 — 비주얼 도약과 멀티플랫폼

UE4 채택은 두 가지 실리를 동시에 얻게 했다. 첫째, "움직이는 일본화"라 불릴 만큼 진일보한 비주얼로 발표 시점부터 시각적 화제를 만들었다. 둘째, 멀티 플랫폼 이식이 쉬워져 PS4·Xbox One을 시작으로 Stadia, Switch, PC(Epic·Steam), Xbox Series, 모바일(Netflix)까지 장기간에 걸쳐 폭넓게 출시될 수 있었다. 플랫폼 확장은 곧 판매 채널의 확장이었다.

### (4) 타이밍 — 11년의 갈증과 SNK 부활 서사

직전 본편으로부터 11년이라는 긴 공백은 오히려 강력한 마케팅 동력이 됐다. "전설적 시리즈의 귀환"이라는 서사는 노스탤지어 수요를 자극했고, SNK 자체의 부활 스토리(《The King of Fighters XIV》로 3D 전환을 시작한 흐름의 연장)와 맞물려 격투 게임 팬덤의 주목을 모았다. 사전 예약만으로 흑자를 낸 사실이 이 노스탤지어·기대 수요의 강도를 증명한다.

### (5) FGC(격투 게임 커뮤니티) 중심 마케팅

SNK는 EVO 등 메이저 토너먼트를 핵심 마케팅 채널로 활용했다. EVO 2019에서의 1,700명 규모 엔트리는 단순한 흥행 지표를 넘어, e스포츠·스트리밍을 통한 자연 확산을 일으켰다. 코어 커뮤니티가 먼저 게임을 "증명"하고 그 열기가 바깥으로 퍼지는 전형적인 격투 게임 흥행 구조를 정확히 탔다.

### (6) 동시기 경쟁작 대비 차별점

《Street Fighter V》, 《Tekken 7》, 《Mortal Kombat 11》, 《Dragon Ball FighterZ》 등 동시기 강자들이 콤보·연계·플래시한 연출로 경쟁하던 시기에, 《Samurai Shodown》은 "느리고 무겁고 한 방이 치명적인" 정반대의 결을 택해 시장에서 고유의 자리를 만들었다. 같은 장르 안에서 직접 충돌하지 않는 포지셔닝을 확보한 것이 생존·성공의 토대였다.

---

## 6. 비평적 시각 / 한계 / 논란

### (1) 빈약한 출시 콘텐츠

가장 일관된 비판은 **싱글플레이·전체 콘텐츠 분량의 부족**이다. 스토리 모드는 짧고 빈약했으며, 출시 모드 구성이 동시기 대형 격투 게임(특히 풍부한 싱글 캠페인을 갖춘 《Mortal Kombat 11》)에 비해 초라했다. 기본 16명이라는 로스터도 출시 시점 기준으로는 적은 편이어서, "전투는 훌륭하나 패키지는 미완성"이라는 인상을 남겼다.

### (2) 열악한 출시 넷코드

반응 속도가 핵심인 게임에서 딜레이 기반 넷코드는 치명적이었다. 온라인 대전에서의 입력 지연은 풋시·받아치기 같은 핵심 메카닉을 무너뜨렸고, 이는 라이트 유저의 장기 잔존을 가로막았다. 롤백 넷코드가 도입된 것은 출시로부터 4~5년이 지난 2023~2024년이었다. SNK는 이 교훈을 흡수해 후속 《The King of Fighters XV》(2022)는 처음부터 롤백 넷코드를 탑재했다.

### (3) Dojo "Ghost" AI의 기대 미달

야심차게 홍보한 딥러닝 Ghost 기능은 실제로는 실망스러웠다. Siliconera 등은 이 모드가 "거의 무용지물"에 가까웠다고 평했는데, AI가 플레이어 스타일을 어느 정도 흉내 내는 듯하다가 이내 무차별적으로 잡기·회피·약베기를 남발하는 비일관적 행동으로 무너졌기 때문이다. 마케팅이 약속한 "나를 닮은 AI"라는 환상에는 크게 못 미쳤다. ([Siliconera](https://www.siliconera.com/samurai-shodowns-dojo-mode-is-pretty-useless/))

### (4) 평가가 갈리는 지점 — 게임플레이 템포

"느리고 신중한" 템포는 시리즈 정체성이자 양날의 검이다. 풋시와 심리전을 사랑하는 코어 유저에게는 더없는 매력이지만, 빠르고 화려한 액션을 기대한 일부 유저에게는 "지루하다"는 인상을 줄 수 있었다. 한 방 데미지가 큰 만큼 운·심리에 따른 변수가 크다는 점도 호불호가 갈렸다.

### (5) 출시 타이밍의 불운

격투 게임 매체들은 후일 회고에서, 이 작품이 "위험한 결정과 어려운 타이밍, 예측 불가능한 외부 상황의 피해자"였다고 평가하기도 했다. 뛰어난 코어를 가졌음에도 출시 넷코드 문제와 콘텐츠 부족, 그리고 이후의 시장 환경이 겹쳐 장기 흥행으로 충분히 이어지지 못한 측면이 있다. ([EventHubs 회고](https://www.eventhubs.com/news/2025/mar/04/2019-samurai-shodown-victim-circumstances/))

---

## 7. 영향과 유산

### 장르·산업적 의미

《Samurai Shodown》(2019)은 "콤보 중심이 아닌, 뉴트럴·한 방 중심의 격투 게임도 현대 시장에서 충분히 통한다"는 것을 입증했다. 점점 복잡해지던 격투 게임 흐름 속에서, 단순하고 무거운 전투 철학의 가치를 재확인시킨 사례로 남는다. 격투 게임 디자인 담론에서 "낮은 진입 장벽 + 높은 숙련 천장"의 모범 사례로 자주 인용된다.

### SNK 부활 서사의 한 축

이 작품은 SNK가 《The King of Fighters XIV》(2016)로 시작한 부활·현대화 흐름을 이어받아 **UE4 표준화**를 본격화한 분기점이다. 비주얼·멀티플랫폼 전략의 성공은 이후 SNK 라인업(《KOF XV》 등)의 토대가 됐고, 출시 넷코드 실패의 교훈은 후속작의 롤백 기본 탑재로 직결됐다. 즉 《Samurai Shodown》은 성공과 실패 양쪽 모두에서 SNK의 다음 행보에 직접적인 교훈을 남겼다.

### 라이브 운영과 IP 교류

장기간에 걸친 시즌제 DLC(베테랑 복귀 + 외부 게스트)는 격투 게임의 라이브 운영 모델을 충실히 따랐다. 특히 《For Honor》의 Warden, 《Guilty Gear》의 Baiken, 《Honor of Kings》의 Gongsun Li 등 타사·타 IP 게스트 영입은 글로벌 협업의 적극성을 보여주며, 팬덤 교차 유입을 노린 전형적 전략이었다.

### 문화적 의미

11년 만의 귀환은 시리즈를 다시 격투 게임 담론의 중심으로 불러왔다. EVO 종목 채택과 1,700명 규모 엔트리는 이 IP가 여전히 코어 커뮤니티에서 강한 생명력을 지님을 증명했다. 또한 우키요에·시대극 미학을 현대 게임으로 번역한 비주얼은, 일본 전통 미학과 게임 아트의 결합 사례로도 의미가 있다. 그 결과 시리즈는 명맥을 유지하며, SNK 격투 포트폴리오의 핵심 기둥 중 하나로 자리매김했다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
|---|---|
| 개발사 / 퍼블리셔 | SNK / SNK·Athlon Games·Deep Silver·Taito·Netflix |
| 디렉터 / 프로듀서 | Nobuyuki Kuroki / Yasuyuki Oda |
| 엔진 | Unreal Engine 4 (SNK 최초) |
| 최초 출시 | 2019년 6월 25일 (PS4 / Xbox One) |
| 장르 | 무기 기반 2D 대전 격투 |
| 시대 배경 | 1787년, 덴메이 시대 일본 |
| 기본 로스터 | 16명 (베테랑 13 + 신규 3) + 최종 보스 |
| 신규 캐릭터 | Darli Dagger, Wu-Ruixiang, Yashamaru Kurama |
| 최종 보스 | Shizuka Gozen |
| Metacritic | PS4 81 / XBO 78 / PC 76 / Switch 75 |
| 주요 평점 | IGN 8.2, GameSpot 8.0, Eurogamer 4/5, Game Informer 7.75 |
| 일본 첫 주(출하+디지털) | 40,606장 |
| EVO 2019 엔트리 | 약 1,700명 |
| 롤백 넷코드 적용 | PC 2023.12.14 / 콘솔 2024.5.22 |
| 주요 수상 | NAVGTR Game, Franchise Fighting 수상 / TGA·DICE 후보 |

### 핵심 시스템 요약

- **설계 철학**: "죽음에서 한 칼, 승리에서 한 칼" — 콤보 아닌 뉴트럴 중심, 한 방의 막대한 데미지.
- **Rage Explosion**: 경기당 1회, 데미지 +40%, 체력 낮을수록 지속 시간 증가.
- **Super Special / Weapon-Flipping**: 1회성 초필살기, 명중 시 무기 탈락(disarm) 가능.
- **Lightning Blade**: Rage Explosion 중에만, 남은 게이지 비례 데미지(즉사급).
- **Dojo Ghost AI**: 딥러닝으로 플레이어 패턴 학습한 AI 고스트 생성·공유(실제 완성도는 미흡).

### 주요 인터뷰·자료

- Unreal Engine 공식 개발자 인터뷰 — "Unreal Engine provided robust artistic tools that empowered SNK to make the most beautiful Samurai Shodown yet" ([unrealengine.com](https://www.unrealengine.com/en-US/developer-interviews/unreal-engine-provided-robust-artistic-tools-that-empowered-snk-to-make-the-most-beautiful-samurai-shodown-yet))
- Unreal Engine — "Why SNK shifted to Unreal Engine for its latest fighting games" ([unrealengine.com](https://www.unrealengine.com/developer-interviews/why-snk-shifted-to-unreal-engine-for-its-latest-fighting-games))
- PCGamesN — "Making it in Unreal: why now is the perfect time for Samurai Shodown" ([pcgamesn.com](https://www.pcgamesn.com/samurai-shodown/making-it-in-unreal-samurai-shodown))
- Siliconera — 디렉터 Kuroki 인터뷰(포팅·신규 캐릭터) ([siliconera.com](https://www.siliconera.com/samurai-shodowns-director-talks-about-the-game-its-ports-and-creating-new-characters/))
- GameSpot — "Samurai Shodown Uses Deep Machine Learning To Create Opponents" ([gamespot.com](https://www.gamespot.com/articles/samurai-shodown-uses-deep-machine-learning-to-crea/1100-6465815/))
- Variety — "'90s Fighting Series 'Samurai Shodown' Returns This June" ([variety.com](https://variety.com/2019/gaming/news/snk-announces-samurai-shodown-reboot-1203171293/))

### 참고 자료 목록

- Wikipedia — Samurai Shodown (2019 video game): https://en.wikipedia.org/wiki/Samurai_Shodown_(2019_video_game)
- Metacritic — Samurai Shodown: https://www.metacritic.com/game/samurai-shodown/
- OpenCritic — Samurai Shodown: https://opencritic.com/game/7854/samurai-shodown
- IGN / GameSpot / Eurogamer / Game Informer 리뷰 (4장 인용)
- Gematsu — 일본 첫 주 판매 집계: https://www.gematsu.com/2019/07/samurai-shodown-ps4-shipments-and-digital-sales-top-40606-in-japan
- EventHubs — 리뷰 라운드업·2019 올해의 격투 게임·롤백 베타·회고: https://www.eventhubs.com/
- Mizuumi Wiki — Samurai Shodown Mechanics: http://wiki.mizuumi.net/w/Samurai_Shodown/Mechanics
- Liquipedia Fighting Games — Samurai Shodown (2019): https://liquipedia.net/fighters/Samurai_Shodown_(2019)
- Esports Earnings — EVO 2019 Samurai Shodown: https://www.esportsearnings.com/tournaments/36585-evo-2019-samurai-shodown

---

*본 분석서는 영어권 매체·공식 개발자 인터뷰·격투 게임 커뮤니티 자료를 기반으로 작성했다. 판매·점수 수치는 각 출처 집계 기준이며, 시점에 따라 갱신될 수 있다.*
