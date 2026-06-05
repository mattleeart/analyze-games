# 《Rivals of Aether》 (2017) 심층 분석

> 한 명의 전직 Microsoft 게임 디자이너가 대학 시절 만든 《Super Smash Bros.》 데모(《Super Smash Land》)에서 출발해, "친근하지만 깊은(accessible but deep)" 플랫폼 파이터를 만들겠다는 목표 하나로 회사를 나와 인디로 완성한 작품. 방패와 잡기를 버리고 패링과 웨이브대시를 전면에 세운 공격 지향 설계, 16비트 픽셀아트의 원소 수인(獸人) 캐릭터, 그리고 무엇보다 Steam Workshop을 통해 누구나 캐릭터를 만들 수 있게 개방한 결정이 이 게임을 단순한 "스매시 클론"이 아니라 **플랫폼 파이터 장르의 독립적 표준 중 하나**로 끌어올렸다.

---

## 1. 게임 개요

### 기본 정보

| 항목 | 내용 |
|------|------|
| 제목 | 《Rivals of Aether》 |
| 장르 | 플랫폼 파이터(Platform Fighter) |
| 개발사 | Aether Studios (Dan Fornace 1인 스튜디오에서 출발) |
| 크리에이터·디렉터 | Dan Fornace |
| 엔진 | GameMaker (당시 GameMaker: Studio) |
| 출시 (PC, Early Access) | 2015년 (Steam 앞서 해보기) |
| 정식 출시 (Windows/Steam) | 2017년 3월 28일 |
| Xbox One | 2017년 8월 22일 |
| Nintendo Switch | 2020년 9월 24일 (Definitive Edition) |
| 모드 | 싱글플레이어, 로컬·온라인 멀티플레이어 |

### 디렉터와 핵심 크레딧

이 게임의 정체성은 곧 **Dan Fornace**라는 인물의 이력과 분리되지 않는다. Fornace는 대학 재학 중 독립 개발자로 시작해 2011년 《Super Smash Land》라는 팬메이드 작품을 내놓았다. 이는 닌텐도의 《Super Smash Bros.》를 게임보이 스타일의 흑백 데미크(demake)로 재해석한 작품으로, 당시 인디 신에서 화제가 되었다. 졸업 후 그는 Microsoft Studios에 입사해 약 2년 9개월간 게임 디자이너로 일하며 여러 XBLA(Xbox Live Arcade) 타이틀에 참여했다.

그러나 Fornace는 자신만의 플랫폼 파이터를 만들겠다는 목표로 2014년 4월 Microsoft를 퇴사했고, 같은 시기 작곡가 **flashygoodness**와 함께 《Rivals of Aether》 개발에 착수했다. 2014년 7월 프로젝트가 대중에 공개되면서 첫 두 캐릭터—Zetterburn(The Fire's Roar)과 Orcane(The Puddle Jumper)—가 함께 발표되었다.

주요 크레딧은 다음과 같다. 디자인·디렉션은 Dan Fornace, 프로그래밍은 Trevor Youngblood와 Ampersandbear, 아트는 Ellian과 Alex Mcdonald, 음악은 flashygoodness가 담당했다. 즉 이 게임은 전형적인 대형 스튜디오 작품이 아니라, **극소수 핵심 인력으로 운영된 인디 프로젝트**다. 운영 명의는 초기 Dan Fornace 개인 브랜드에서 점차 Aether Studios로 정리되었다.

### 엔진과 기술 스택

엔진은 YoYo Games의 **GameMaker(GameMaker: Studio)**다. 이 선택은 단순한 편의가 아니라 후일 게임의 핵심 강점—Steam Workshop을 통한 커스텀 캐릭터 제작—과 직결되는 전략적 결정이 된다. GameMaker는 진입 장벽이 낮은 게임 제작 도구였고, 《Rivals of Aether》의 Workshop은 바로 이 GameMaker: Studio 환경 위에서 유저들이 캐릭터·스테이지·버디(Buddy)를 직접 만들 수 있도록 개방되었다.

기술적으로 이 게임은 출시 후 수년에 걸친 가장 큰 도전 과제로 **롤백 넷코드(rollback netcode)** 도입을 안고 있었다. 본래 딜레이 기반(delay-based) 넷코드로 출시된 작품을 롤백 방식으로 전환하는 작업은 소규모 스튜디오에게 막대한 비용이었고, 팀(YellowAfterlife, Yosi, Zach Reedy, Juju 등이 참여)은 수년에 걸친 작업 끝에 Steam에서 롤백 넷코드 오픈 베타를 공개하기에 이른다.

---

## 2. 게임 설명

### 컨셉: "원소를 두른 동물 전사들의 플랫폼 파이터"

《Rivals of Aether》는 한마디로 **2~4인 난투형 플랫폼 파이터**다. 무대 위에서 상대를 점점 더 멀리 날려보내(knockback) 화면 밖으로 떨어뜨리는 것이 승리 조건이라는 점에서 《Super Smash Bros.》 계열의 기본 골격을 공유한다. 그러나 세계관과 캐릭터 디자인은 닌텐도의 IP 올스타가 아니라 **완전한 오리지널 세계 'Aether'**를 토대로 한다.

세계 'Aether'는 불(Fire), 물(Water), 공기(Air), 흙(Earth) 등 고전적 4원소를 중심으로 설계되었으며, 각 플레이 가능 캐릭터는 특정 원소에 정렬되어 그 원소가 곧 플레이 스타일의 핵심이 된다. 캐릭터들은 대부분 의인화된 동물(수인) 디자인으로, Rock, Paper, Shotgun은 그 캐릭터 디자인을 두고 "《Pokémon》을 연상시킨다"고 평했다.

### 세계관과 스토리 [스포일러 포함]

게임은 단순한 대전 모드에 그치지 않고 **Story Mode(스토리 모드)**를 통해 Aether의 서사를 전한다. 스토리 모드는 로컬 1~2인 협동 플레이를 지원하며, 7개의 메인 챕터로 구성되어 Maypul, Forsburn, Zetterburn, Orcane, Wrastor, Kragg 각 캐릭터의 이야기에 초점을 맞춘다. 그리고 마지막 챕터에서 Aether의 진정한 적대자인 **Gatekeepers(게이트키퍼)**의 정체가 드러난다.

[스포일러] 세계관의 정치적 음모는 Fire Empire(화염 제국)를 둘러싸고 전개된다. **Loxodont**(록소돈트)는 Fire Empire의 통상장관(Minister of Trade)이자 Fire Council의 일원으로, 겉으로는 Emperor Renburn의 친구로 행세했으나 실제로는 의회를 움직여 Renburn 황제를 살해하고 그 죄를 **Forsburn**에게 뒤집어씌운 인물이다. 캐릭터 **Clairen**은 Zetterburn과 Forsburn이 모두 사라져 영영 돌아오지 않은 먼 미래에서 온 노련한 전사로, 그녀의 시대에는 Loxodont가 강력한 황제로 성장해 Aether의 거의 전역을 지배하게 된다. 이러한 시간축을 가로지르는 서사는 단순 대전 게임으로서는 이례적으로 짜임새 있는 세계관을 부여했고, 후일 사실상 하나의 트랜스미디어 프랜차이즈(《Lovers of Aether》, 《Creatures of Aether》, 《Dungeons of Aether》, 코믹 《Tales of Aether》 등)로 확장되는 토대가 된다.

### 주요 캐릭터

기본 로스터의 핵심 캐릭터와 그 원소·콘셉트는 다음과 같다.

- **Zetterburn (불)** — "The Fire's Roar". 사자 형상의 캐릭터로, 게임 최초 설계 캐릭터. Fornace는 이를 Smash 플레이어가 곧바로 적응할 수 있는 "친근한 입문 캐릭터"로 의도했으며, 《Smash Bros.》의 Fox/Wolf와 유사한 손맛을 준다.
- **Orcane (물)** — "The Puddle Jumper". 물웅덩이를 만들고 그 웅덩이를 활용해 텔레포트·복귀·강타로 연결하는 자원 운용형 캐릭터.
- **Wrastor (공기)** — Air Armada의 'Aerial Ace'. 차지 강공격(Strong Attack)을 지상이 아닌 **공중에서** 수행하는, 장르 최초의 시도를 담은 캐릭터.
- **Maypul (흙/식물)** — 씨앗과 'Watcher's Dash'로 상대에게 표식을 남기고, 표식 대상을 식물 Lily로 속박해 추가타로 연결하는 마킹·콤보형 캐릭터.
- **Forsburn (불/연기)** — 연기로 전장을 가리고 그 안에 은신하거나, 자신의 연기 분신을 만들어 공격하며, 연기를 다시 흡수해 충전 후 폭발시키는 트릭스터.
- **Kragg (흙)** — 거대한 Aetherian Forest의 수호자. 땅에서 바위를 뽑아 던질 수 있고, 그 바위는 무대의 일부가 되어 Kragg 자신이나 다른 플레이어가 부술 수 있다.

이후 DLC와 Definitive Edition을 거치며 로스터는 크게 확장되었다(자세한 출시 일정은 5장과 7장 참조).

### 무드·톤·아트 디렉션

비주얼은 깔끔하고 채도 높은 **16비트 픽셀아트**다. 한 리뷰는 "16비트 아트 스타일이 각 캐릭터를, 특히 원소 공격을 통해 빛나게 한다"고 평했으며, Polygon은 단순히 "아름답다(beautiful)"고 표현했다. 픽셀 그래픽이 정적인 일러스트에 머무르지 않고 **모션에서 살아 움직인다**는 점이 자주 칭찬받았다—이는 빠른 대전 게임에서 캐릭터의 동작과 히트박스를 직관적으로 읽게 하는 가독성과도 직결된다.

사운드 측면에서는 작곡가 flashygoodness가 합류 초기부터 함께한 음악이 게임의 정체성에 크게 기여했다. 강렬하고 에너지 넘치는 칩튠/일렉트로닉 사운드트랙은 게임의 빠른 템포와 어울리며, 사운드트랙 자체가 팬덤에서 별도로 사랑받는 콘텐츠가 되었다.

---

## 3. 핵심 시스템 / 메카닉

《Rivals of Aether》의 설계 철학은 한 문장으로 요약된다: **"방어 옵션을 줄이고 공격을 보상하라."** Dan Fornace는 이 게임의 엔진 설계 대부분을 "공격적 전투(offensive combat)에 초점을 맞춰" 결정했다고 밝혔으며, 그 결과 《Smash Bros.》에 있던 방어 옵션들이 의도적으로 축소되었다.

### 코어 루프와 승리 조건

기본 루프는 플랫폼 파이터의 정석을 따른다. 상대를 타격하면 데미지가 누적되고, 데미지가 높을수록 넉백이 커진다. 상대를 무대 경계 밖(블래스트 존)으로 날려 보내거나, 무대로 복귀(recovery)하려는 시도를 차단(edge-guarding)해 떨어뜨리면 스톡(목숨)을 빼앗는다. 여기까지는 《Smash》 계열과 동일하지만, 세부 룰에서 결정적 차이가 갈린다.

### 방패·잡기 폐지, 그리고 패링(Parry)

《Rivals of Aether》는 《Smash Bros.》와 달리 **아이템이 없고, 가장자리(ledge)를 잡을 수 없으며, 방패(shield)와 잡기(grab)가 존재하지 않는다.** 그 자리를 대체하는 것이 바로 **패링(Parry)** 시스템이다.

패링은 상대의 다음 공격을 정확한 타이밍에 예측해 막아내면, 상대를 **스턴**시키고 자신에게는 일시적 무적을 부여하는 기술이다. 이는 《Street Fighter III: 3rd Strike》의 패링처럼 "정확한 타이밍"을 핵심으로 삼아, 수비를 그저 버티는 행위가 아니라 **고위험·고보상의 능동적 공격 기회**로 바꾼다. 방패처럼 무한정 막을 수 있는 안전망이 없으므로, 플레이어는 끊임없이 공격을 강요받고, 상대의 패턴을 읽어 패링으로 역공할지 회피로 빠질지를 매 순간 결정해야 한다. 이 단 하나의 설계 결정이 게임 전체의 템포를 끌어올리고 공격적 플레이를 구조적으로 보상한다.

### 웨이브대시(Wavedashing)

《Smash Bros. Melee》의 상징적 고급 테크닉이었던 **웨이브대시**가 《Rivals of Aether》에서는 **숨겨진 버그가 아니라 정식으로 완비된 메카닉**으로 들어가 있고, 게임플레이 자체가 이를 중심으로 밸런싱되어 있다. 웨이브대시란 공중에서 지면 방향으로 에어닷지(air-dodge)를 입력해 캐릭터를 지상에서 미끄러뜨리는 동작으로, 이동을 빠르고 예측 불가능하게 만들어 공방의 핵심 무브먼트가 된다. 《Melee》에서는 우연히 발견된 비공식 테크였던 것을, 《Rivals》는 설계 단계에서 1급 기능으로 끌어안아 누구나 배울 수 있는 정식 기술로 만든 것이다.

### 복귀(Recovery)와 월점프

가장자리 잡기가 없는 대신, 《Rivals of Aether》는 특유의 **월점프(wall jump) 메카닉**을 둔다. 벽에 닿아 점프하면 복귀기(up-special 등)를 착지 전 **한 번 더** 사용할 수 있어, 무대 밖으로 날아갔을 때 복귀 루트를 다채롭게 만든다. 가장자리에 매달려 무적 시간을 버는 "ledge camping"이 불가능하므로, 복귀하는 쪽과 막는 쪽(edge-guarder) 모두 더 공격적이고 읽기 싸움 중심의 교전을 하게 된다.

### 원소 자원 시스템

각 캐릭터는 자신의 원소를 **자원처럼 운용**한다. 이는 단순 콤보를 넘어 게임에 전략적 깊이를 더한다. 몇 가지 예:

- **Zetterburn**은 상대를 "불태운(burning)" 상태로 만들고, 상대가 불타는 동안 Strong Attack으로 그 화염을 흡수하면 넉백을 **두 배**로 키워 결정타로 삼는다.
- **Orcane**은 웅덩이 위에 설 때 그 물을 소비해 사거리와 넉백이 크게 강화된 Strong Attack을 쓴다. 웅덩이는 텔레포트 복귀, 함정(bubble pillar), 강타의 기점이 모두 된다.
- **Forsburn**은 연기 구름을 세 번 흡수해 충전한 뒤 Down Special을 다시 써서 상대를 고속으로 날려보내는 폭발을 일으킨다.
- **Maypul**은 마킹→속박→추가타라는 자원 사이클로 콤보를 설계한다.

즉 단순히 "원소 테마 스킨"이 아니라, 각 캐릭터의 **고유 자원 관리 루프**가 곧 그 캐릭터의 정체성이 되도록 설계되어 있다. Fornace는 무브셋 영감을 격투/Smash뿐 아니라 《League of Legends》, 《Full Metal Alchemist》 같은 다양한 출처에서 가져왔다고 밝힌 바 있다.

### 싱글플레이어 모드: Story Mode와 Abyss

대전 게임이면서도 싱글·협동 콘텐츠가 비교적 충실하다.

- **Story Mode** — 로컬 1~2인 협동. 7개 메인 챕터로 각 캐릭터의 서사를 풀어내고, Gatekeepers라는 진 적대자를 드러낸다.
- **Abyss (Abyss Endless)** — 로컬 싱글 또는 협동 모드. 점점 어려워지는 웨이브를 돌파하며, **룬(rune)**을 구매·장착해 캐릭터를 강화하거나 특수 능력을 부여하는 **로그라이트형** 모드. 반복 플레이성과 빌드 구성의 재미를 더한다.

### 접근성과 UI/UX 철학

이 게임은 "쉽게 입문하되 천장은 매우 높게"라는 균형을 명시적으로 추구한다. 신규 플레이어는 단순한 조작과 친절한 튜토리얼로 곧바로 진입할 수 있다. 동시에 튜토리얼은 "프레임(frames)", "히트박스(hitboxes)" 같은 내부 전문 용어까지 깊이 파고들며(트레이닝 모드에서 히트박스 시각화를 켤 수 있다), 캐릭터별 권장 전략까지 제시한다. 이는 격투 게임 입문자에게 가장 큰 장벽인 "보이지 않는 규칙"을 가시화하려는 시도로, 단순한 친절을 넘어 **경쟁 격투 게임의 학습 곡선 자체를 설계 대상으로 삼은** 접근이다.

---

## 4. 평가

### 평론 반응

《Rivals of Aether》는 평단에서 전반적으로 긍정적인 평가를 받았다. 핵심 평가는 "《Smash Bros.》 공식을 단순 모방하지 않고, 그 위에 추가적 깊이를 쌓아올린 본격 격투 게임"이라는 것이다.

- **Destructoid** (Nick Valdez): "추가적 깊이를 더한 완전히 다듬어진(fully fleshed out) 파이터"라고 평하며, 《Super Smash Bros.》 공식에 깊이를 더했다고 호평했다.
- **Polygon**: "《Super Smash Bros.》에 대한 인디의 답(the indie answer to Super Smash Bros.)"이라 표현하고, 비주얼을 "아름답다(beautiful)"고 칭했다.
- **Rock, Paper, Shotgun**: 캐릭터 디자인을 "《Pokémon》을 연상시킨다"며 호평했다.

리뷰들이 공통적으로 짚은 강점은 (1) 깔끔하고 표현력 있는 픽셀아트, (2) 입문은 쉽지만 극도로 높은 스킬 천장, (3) 패링·웨이브대시·원소 자원으로 차별화된 메카닉의 깊이였다. "고급 무브먼트, 콤보, 캐릭터 테크를 배우기 시작하면 어마어마한 깊이가 열린다"는 평이 대표적이다.

### 상업 지표

서드파티 추정치 기준, 《Rivals of Aether》는 Steam에서 약 **140만~160만 장**이 판매된 것으로 추정되며(Video Game Insights 등 추정), 2017년 3월 출시 이후 약 **2,800만 달러**의 총매출(gross revenue)을 올린 것으로 추정된다. 인디 격투/플랫폼 파이터로서는 매우 견고한 상업적 성공이며, 이는 후속작 개발과 트랜스미디어 확장을 가능케 한 토대가 되었다. (이 수치들은 서드파티 추정치이므로 [추정]으로 이해해야 한다.)

참고로 후속작 《Rivals of Aether II》는 2024년 10월 23일 정식 출시 후 **약 일주일 만에 10만 장**을 돌파하며, 원작이 구축한 팬덤의 규모를 입증했다.

### 출시 경로: Early Access의 성공 사례

이 게임은 2017년 정식 출시 이전에 **Steam 앞서 해보기(Early Access)** 및 Xbox의 **Game Preview** 프로그램을 거쳤다. 즉 커뮤니티와 함께 수년간 밸런스를 다듬으며 완성도를 높여간 사례로, 출시 시점에 이미 탄탄한 팬덤과 검증된 메카닉을 갖춘 채 나왔다는 점이 상업적·평론적 안정성의 배경이 되었다.

### 유저 평가와 커뮤니티

Steam과 커뮤니티에서 이 게임은 오랜 기간 꾸준한 호평을 유지했다. 특히 경쟁 격투 커뮤니티(FGC) 일부와 Smash 디아스포라(공식 룰셋·넷코드에 불만을 가진 Melee/플랫폼 파이터 플레이어들)에게 "닌텐도 IP에 묶이지 않은, 정식으로 토너먼트 운영이 가능한 플랫폼 파이터"라는 가치를 인정받았다. 게임은 자체적으로 경쟁 룰(Competitive Rules)과 'Rivals Top 50' 같은 랭킹·방법론을 운영하며 경쟁 신을 적극 육성했다.

---

## 5. 성공 요인 분석

### (1) "친근하지만 깊은"이라는 명확한 설계 목표

Fornace는 처음부터 **"accessible but deep(친근하지만 깊은)"** 파이터라는 단 하나의 목표를 일관되게 추구했다. 그는 《Killer Instinct》가 달성한 "쉬운 입문 + 깊은 숙련"의 균형을 명시적으로 존경했고, 이를 플랫폼 파이터에 이식하려 했다. 첫 캐릭터 Zetterburn을 Smash 플레이어가 즉시 적응할 수 있는 입문형으로 설계하되, 나머지 캐릭터는 Smash 캐릭터를 흉내 내기보다 각자의 **원소와 자원 메카닉**을 중심으로 설계함으로써, "익숙함으로 끌어들이고 독창성으로 붙잡는" 구조를 만들었다.

### (2) 방어를 깎고 공격을 보상한 메카닉 차별화

방패·잡기·가장자리 잡기를 제거하고 패링을 도입한 결정은 단순한 "Smash 클론 회피용 변형"이 아니라, **게임 전체의 정체성을 규정하는 핵심 차별점**이었다. 그 결과 《Rivals》는 《Melee》의 속도감과 《Street Fighter III: 3rd Strike》식 타이밍 패링을 결합한 고유의 공격적 메타를 갖게 되었고, "더 빠르고 더 콤보 지향적인 플랫폼 파이터"라는 명확한 포지션을 확보했다. 이는 원작 《Super Smash Land》 시절부터 Fornace가 추구한 "더 빠르고 콤보 중심" 방향성의 연장선이다.

### (3) Steam Workshop — 커뮤니티를 개발 파이프라인으로 끌어들인 전략

이 게임의 가장 결정적이고 모범적인 성공 요인은 **Steam Workshop 개방**이다. 2019년 9월 18일부터 정식 지원된 Workshop은, 유저가 GameMaker: Studio를 활용해 **커스텀 캐릭터·스테이지·버디(Buddy)**를 직접 만들고 공유하게 했다.

이는 단순한 모드 지원을 넘어 **무한 콘텐츠 공급원이자 인재 발굴 파이프라인**이 되었다. 대표적으로, 팬이 만든 캐릭터 **Mollo**가 공식 Rivals of Aether Direct에서 소개되었고, 그 제작자 **Giik**은 이후 향후 Workshop 기능 개발을 돕도록 **정식 채용**되었다. 더 나아가 Workshop 출신 캐릭터 네 명—**Mollo, Hodan, Pomme, Olympia**—이 기본 캐스트로 편입되기에 이른다. 즉 커뮤니티 창작물이 공식 게임에 역으로 통합되는 선순환이 실제로 작동했다. 이는 게임의 수명을 사실상 무한히 연장하고, 충성도 높은 크리에이터 커뮤니티를 게임의 일부로 묶어두는 효과를 냈다.

### (4) Early Access를 통한 커뮤니티 공동 개발

수년간의 Steam Early Access / Xbox Game Preview를 거치며 커뮤니티 피드백으로 밸런스를 다듬은 점은, 출시 시점의 완성도와 신뢰를 동시에 확보하게 했다. 인디 격투 게임이 흔히 겪는 "출시 후 텅 빈 온라인" 문제를 출시 전부터 쌓아온 팬덤으로 상당 부분 회피했다.

### (5) 오리지널 IP와 트랜스미디어 확장 잠재력

닌텐도 IP에 의존하지 않는 오리지널 세계관 'Aether'는, 토너먼트 운영의 법적 자유(저작권 분쟁 위험 없음)뿐 아니라 후속 확장의 토대가 되었다. 실제로 이 IP는 데이팅 시뮬레이션 《Lovers of Aether》(2019), 덱빌딩 《Creatures of Aether》(2020), 로그라이크 《Dungeons of Aether》(2023), 코믹 《Tales of Aether》(2021), 그리고 정식 후속작 《Rivals of Aether II》(2024)로 뻗어나갔다.

### (6) 동시기 경쟁작 대비 차별점

2017년 전후 플랫폼 파이터 시장에는 《Brawlhalla》(부분유료·무기 기반), 《Brawlout》 등이 있었다. 《Rivals of Aether》는 이들과 달리 **《Melee》식 하드코어 무브먼트(웨이브대시)와 패링 중심의 공격적 메타**를 정면으로 끌어안아, "진지한 경쟁 플랫폼 파이터를 원하지만 닌텐도 생태계를 벗어나고 싶은" 플레이어층을 정확히 겨냥했다. 무료화·캐주얼 노선으로 폭을 넓힌 《Brawlhalla》와는 정반대 지점에서 자기 시장을 확보한 셈이다.

---

## 6. 비평적 시각 / 한계 / 논란

### (1) 넷코드 — 가장 오래 끌었던 약점

가장 자주 지적된 한계는 **온라인 넷코드**였다. 게임은 본래 딜레이 기반 넷코드로 출시되었는데, 빠른 템포의 플랫폼 파이터에서 입력 지연은 경쟁 플레이의 치명적 결함이 된다. 개발팀은 이를 **롤백 넷코드**로 전환하려 수년간 노력했으나, 완성된 게임을 사후에 롤백으로 바꾸는 작업은 소규모 스튜디오에게 막대한 비용이었고 "너무 비싸서 일단 접어야 했던" 시기도 있었다. 결국 YellowAfterlife, Yosi, Zach Reedy, Juju 등의 기여로 롤백 넷코드 오픈 베타를 출시하기에 이르렀지만, 이 과정의 길이와 어려움 자체가 "딜레이 기반으로 먼저 출시한 결정"의 비용을 보여주는 사례로 남았다.

### (2) "Smash 클론" 프레임의 양날

이 게임은 본질적으로 《Super Smash Bros.》, 특히 《Melee》의 유산을 자랑스럽게 계승한다. 이는 강점인 동시에, 일부에게는 "결국 Smash의 변주"라는 한계로 읽혔다. 닌텐도 캐릭터의 친숙함이 없는 오리지널 로스터는 진입 동기 면에서 IP 매력이 약하다는 평도 있었다(이는 픽셀아트 동물 캐릭터의 매력으로 상당 부분 상쇄되었지만, 닌텐도 올스타의 흡인력과 직접 비교하면 불리한 출발이다).

### (3) 높은 스킬 천장의 양면성

웨이브대시·패링·원소 자원 운용이 결합된 깊은 메카닉은 숙련자에게는 매력이지만, 캐주얼 유저와 하드코어 경쟁층 사이의 간극을 크게 만든다. 친절한 튜토리얼에도 불구하고 《Melee》 계열 무브먼트는 본질적으로 손에 익히기 어려우며, 이 "익히면 천국, 못 익히면 벽"의 구조는 플레이어 이탈 요인이 될 수 있다.

### (4) 플랫폼 파이터 시장의 본질적 한계

플랫폼 파이터는 닌텐도의 《Smash Bros.》라는 절대 강자가 시장을 지배하는 장르다. 오리지널 IP·인디 규모의 작품이 닌텐도의 브랜드·예산·캐릭터 풀과 정면 경쟁하는 것은 구조적으로 불리하다. 《Rivals》의 성공은 인상적이지만, 그 천장은 어디까지나 "닌텐도가 점유하지 않은 틈새(진지한 경쟁 + 토너먼트 자유 + 모드 개방)"를 정밀하게 공략한 결과라는 점에서 한계와 성취가 동전의 양면을 이룬다.

### (5) 개발자의 방향성 발언 논란

Fornace는 이후(후속작 맥락에서) "초심자를 위한 격투 게임을 만드는 일을 그만두겠다(done with making fighting games for newcomers)"는 취지의 발언으로 일부 논의를 불러왔다(NME 보도). 이는 "친근함"을 핵심 가치로 내세웠던 원작의 정체성과 대비되어, 시리즈의 타깃층이 점차 경쟁·코어 지향으로 이동하고 있음을 시사하는 신호로 읽혔다.

---

## 7. 영향과 유산

### (1) 플랫폼 파이터 장르에서의 위상

《Rivals of Aether》는 **닌텐도 밖에서도 진지한 경쟁 플랫폼 파이터가 성립할 수 있음을 증명한 대표작** 중 하나가 되었다. 《Melee》식 깊이를 정식 기능으로 끌어안고(웨이브대시), 패링이라는 독자적 차별점을 더하며, 오리지널 IP로 토너먼트 자유를 확보한 모델은 이후 플랫폼 파이터 설계의 한 참고점이 되었다. 게임은 자체 경쟁 룰셋과 랭킹(Rivals Top 50)을 운영하며 독립적 경쟁 신을 유지했다.

### (2) Steam Workshop 모델의 모범 사례

커뮤니티 창작물을 공식 캐스트로 흡수하는(Mollo·Hodan·Pomme·Olympia, 그리고 제작자 Giik의 정식 채용) 선순환은, "유저 생성 콘텐츠를 개발 파이프라인의 일부로 제도화한" 보기 드문 성공 사례로 자주 인용된다. 이는 게임의 수명을 비약적으로 늘렸을 뿐 아니라, 인디 게임이 적은 인력으로 방대한 콘텐츠를 지속 공급하는 한 가지 해법을 제시했다.

### (3) Definitive Edition과 후속작

게임은 2020년 1월(이후 Switch판은 9월 24일) **Definitive Edition**으로 모든 DLC 캐릭터를 포함한 완성판을 내놓았다. DLC 라인업 일정은 다음과 같았다.

| DLC | 캐릭터 | 출시일 | 비고 |
|------|--------|--------|------|
| 게스트 1 | Ori & Sein | 2017년 8월 22일 | 《Ori and the Blind Forest》 콜라보 |
| DLC | Ranno & Clairen | 2017년 10월 17일 | 물 / 불 |
| DLC | Sylvanos & Elliana | 2018년 4월 2일 | 흙 / 공기 |
| 게스트 2 | Shovel Knight | 2018년 9월 14일 | 마지막 플레이어블, 《Shovel Knight》 콜라보 |

그리고 2024년 10월 23일, 정식 후속작 **《Rivals of Aether II》**가 2D 픽셀아트에서 3D로 전환한 새 작품으로 출시되어, 출시 약 일주일 만에 10만 장을 돌파했다. 후속작은 Aether Studios(이후 운영 구조 변화 포함)와 그 IP가 인디 격투 프랜차이즈로 자리 잡았음을 보여준다.

### (4) 산업적·문화적 의미

《Rivals of Aether》의 궤적은 인디 게임 개발의 한 이상적 서사를 보여준다. 한 개인이 팬게임(《Super Smash Land》)으로 실력을 입증하고, 대기업(Microsoft)에서 경험을 쌓은 뒤, 자기 비전을 위해 독립해 오리지널 IP를 구축하고, 커뮤니티를 개발의 동반자로 끌어들여 그 IP를 멀티미디어 프랜차이즈로 확장한 것이다. 이는 "팬게임 → 정식 오리지널 IP → 트랜스미디어"라는 경로가 실현 가능함을 보여준 사례이자, GameMaker 같은 접근성 높은 도구와 Steam Workshop 같은 플랫폼이 결합될 때 소규모 팀이 어디까지 갈 수 있는지를 보여주는 산업적 레퍼런스다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 수치 / 내용 | 비고·출처 |
|------|------------|-----------|
| 정식 출시 (Windows) | 2017년 3월 28일 | Wikipedia |
| Xbox One | 2017년 8월 22일 | Wikipedia |
| Nintendo Switch | 2020년 9월 24일 | Definitive Edition, Wikipedia |
| 엔진 | GameMaker (GameMaker: Studio) | Wikipedia |
| Steam 추정 판매량 | 약 140만~160만 장 [추정] | Video Game Insights 등 서드파티 추정 |
| 추정 총매출 | 약 2,800만 달러 [추정] | 서드파티 추정 |
| Steam Workshop 정식 지원 | 2019년 9월 18일 | Workshop/Wikipedia |
| 후속작 《Rivals of Aether II》 | 2024년 10월 23일 출시, ~1주 만에 10만 장 | offbrand games 발표, DashFight |

### 주요 인물·크레딧

- **Dan Fornace** — 크리에이터·디렉터 (전 Microsoft Studios 게임 디자이너, 《Super Smash Land》(2011) 제작자)
- **flashygoodness** — 작곡
- **Trevor Youngblood, Ampersandbear** — 프로그래밍
- **Ellian, Alex Mcdonald** — 아트
- 롤백 넷코드 기여: YellowAfterlife, Yosi, Zach Reedy, Juju
- Workshop 출신 정식 합류: Giik(Mollo 제작자, 후 정식 채용)

### 주요 인터뷰·자료

- Dan Fornace, "Rivals of Aether: 2017 Developer Recap - 2018 Developer Preview" (Medium, fornace.medium.com) — 연간 개발 회고
- Dan Fornace, "Fighting Game Design with Dan Fornace: The Power of Silhouettes" (Medium) — 캐릭터 실루엣·가독성 설계론
- "Interview: Dan Fornace talks 'Rivals of Aether'" (Gameverse, 2015) — "accessible but deep" 설계 목표
- "VGU Interviews: Rivals of Aether" (Video Games Uncovered, 2014) — 초기 비전
- "Rivals of Aether's creator details his Smash Bros. inspirations" (GamesBeat) — Smash·Killer Instinct 영감
- "Rivals of Aether's Dan Fornace talks ID@Xbox, Game Preview, and indie development" (Windows Central) — Xbox Game Preview·인디 개발
- "Rivals of Aether with Dan Fornace" (Software Engineering Daily, 2025) — 기술·운영 회고

### 참고 자료 목록 (영어권 매체 중심)

- Wikipedia — "Rivals of Aether" / "Rivals of Aether II" / "GGPO"
- Metacritic — Rivals of Aether (critic & user reviews)
- Destructoid — "Review: Rivals of Aether" (Nick Valdez)
- Polygon — Rivals of Aether 리뷰 ("the indie answer to Super Smash Bros.", "beautiful")
- Rock, Paper, Shotgun — 캐릭터 디자인 평("reminiscent of Pokémon")
- Rivals of Aether Wiki (Fandom) — Parrying, Story Mode, Abyss Endless, Workshop, Definitive Edition, Loxodont
- TV Tropes — VideoGame/RivalsOfAether, Characters/RivalsOfAether
- 공식 사이트 rivalsofaether.com — Characters, Rollback Netcode Open Beta, "Making the Jump from Early Access to Full Launch", Rivals Top 50 Methodology
- NME — "Rivals of Aether creator Dan Fornace is done with making fighting games for newcomers"
- DashFight / offbrand games — 《Rivals of Aether II》 10만 장 돌파 발표
- Video Game Insights / games-stats — Steam 판매·매출 추정치

---

*본 분석서는 영어권 매체·공식 자료·개발자 인터뷰를 바탕으로 작성되었다. 판매량·매출 등 일부 상업 지표는 서드파티 추정치이므로 [추정]으로 표기했으며, 정확한 수치는 출처 보고서 갱신에 따라 달라질 수 있다.*
