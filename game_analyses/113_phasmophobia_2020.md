# Phasmophobia (2020) 심층 분석

> 한 명의 영국 인디 개발자가 만든 4인 협동 공포 게임이, COVID-19 봉쇄와 트위치 스트리밍 붐을 등에 업고 출시 한 달 만에 글로벌 현상이 되었다. 《Phasmophobia》는 "유령 사냥"이라는 익숙한 소재를 증거 수집·유령 식별이라는 정밀한 추리 게임플레이로 재발명했고, 출시 5년이 넘은 지금도 여전히 얼리 액세스 상태이면서 누적 2,500만 장 이상을 판 기록적인 성공작이다. 이 글은 영어권 매체와 개발사 인터뷰를 바탕으로 이 게임의 모든 것을 해부한다.

---

## 1. 게임 개요

### 기본 정보

| 항목 | 내용 |
|------|------|
| 제목 | 《Phasmophobia》 |
| 개발사 | Kinetic Games (영국 사우샘프턴 소재 인디 스튜디오) |
| 퍼블리셔 | Kinetic Games (자체 자금·자체 퍼블리싱) |
| 장르 | 심리 공포, 협동(co-op) 유령 사냥/조사 시뮬레이션 |
| 엔진 | Unity |
| 얼리 액세스 출시 | 2020년 9월 18일 (Microsoft Windows, Steam, 14달러) |
| 콘솔 출시 | 2024년 10월 29일 (PS5, PlayStation VR2, Xbox Series X/S) |
| Nintendo Switch 2 | 2026년 출시 예정 (The Game Awards 2025에서 발표) |
| 플레이 인원 | 1~4인 온라인 협동 |
| VR 지원 | 출시 시점부터 네이티브 VR 지원 |

(출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)), [Steam](https://store.steampowered.com/app/739630/Phasmophobia/), [Gematsu](https://www.gematsu.com/2024/10/phasmophobia-early-access-for-ps5-ps-vr2-and-xbox-series-launches-october-29))

### 디렉터와 크레딧

이 게임의 핵심 인물은 사실상 단 한 사람, **Daniel Knight**(닉네임 Dknighter)다. 그는 Kinetic Games의 리드 개발자이자 CEO이며, 《Phasmophobia》의 디자이너·프로그래머·디렉터 역할을 출시 초기에 혼자 도맡았다. Knight는 이르면 2018년경부터 이 프로젝트를 시작한 것으로 알려져 있으며, 초기 작업명은 《Spectrophobia》였다. 확인 가능한 가장 오래된 얼리-알파 체인지로그는 2019년 12월로 거슬러 올라간다. 2020년 3월 3일, 게임명은 《Phasmophobia》로, 회사명은 Kinetic Games로 변경되었다. (출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)), [Phasmophobia Wiki - Kinetic Games](https://phasmophobia.fandom.com/wiki/Kinetic_Games))

### 개발 규모

이 게임의 가장 극적인 서사 중 하나는 "1인 개발자에서 정식 스튜디오로"의 성장이다. 출시 시점에 Knight는 사실상 혼자였고, 출시 후 7~8개월간 매일 그리고 주말까지 주 60시간 이상을 일했다. 그는 GameSpot 등과의 인터뷰에서 "이 속도를 몇 년이고 유지할 수는 없었다"고 회고하며, 결국 "삶을 되찾기 위해" 사람을 고용하기 시작했다고 밝혔다. Kinetic Games는 이후 1인 운영에서 약 32명 규모의 스튜디오로 성장했다. (출처: [PCGamesN](https://www.pcgamesn.com/phasmophobia/developer-update), [GameSpot](https://www.gamespot.com/articles/phasmophobia-dev-is-preparing-to-shake-things-up-again/1100-6535210/))

특기할 점은 자금 조달 방식이다. Knight는 PCGamesN 인터뷰에서 "우리는 자체 자금·자체 퍼블리싱이라는 매우 운 좋은 위치에 있다. 그래서 우리만의 마일스톤과 타임라인을 직접 정한다"고 말했다. 외부 투자나 퍼블리셔의 압박 없이 개발 일정을 통제할 수 있었던 점이 이 게임의 독특한 운영 철학으로 이어진다.

---

## 2. 게임 설명: 이 게임이 정확히 무엇인가

### 컨셉

《Phasmophobia》는 플레이어가 "유령 사냥꾼(paranormal investigator)" 팀의 일원이 되어, 귀신 들린 장소에 진입해 어떤 종류의 유령이 그곳을 떠도는지 증거를 수집해 식별하는 1인칭 공포 조사 게임이다. 핵심은 "전투"가 아니라 "조사"다. 플레이어는 유령과 싸워 이길 수 없다. 대신 EMF 리더, 스피릿 박스, 온도계, 야간 투시 카메라 같은 실제 심령 조사 장비를 본뜬 도구로 단서를 모아, 세 가지 증거를 조합해 유령의 정체를 추론한 뒤 무사히 빠져나오는 것이 목표다. (출처: [Steam](https://store.steampowered.com/app/739630/Phasmophobia/), [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)))

게임에는 전통적인 의미의 줄거리나 컷신이 없다. 세계관은 "현대 사회에 실재하는 초자연적 현상을 조사하는 민간 조사단"이라는 미니멀한 설정 위에 세워져 있고, 서사는 전적으로 각 조사 세션에서 플레이어가 직접 만들어낸다. 이 "이머전트 호러(emergent horror)" 구조 — 정해진 무서운 순간이 아니라, 예측 불가능한 유령의 행동에서 공포가 자연 발생하는 구조 — 가 이 게임의 정체성이다.

### 영감의 기원: 《The Witcher 3》가 살린 게임

이 게임의 핵심 메카닉이 어디서 왔는지에 관한 일화는 인디 게임사에서 손꼽히는 사례다. Knight는 솔로 개발자로서 첫 게임을 만들던 중, 성공 보장이 전혀 없다는 압박감에 프로젝트를 거의 포기할 뻔했다. 그러던 중 《The Witcher 3: Wild Hunt》의 프롤로그 사이드 퀘스트 "Devil by the Well(우물 속 악마)"을 플레이하다 돌파구를 찾았다. 이 퀘스트에서 게롤트는 정령을 퇴치하기 전에 먼저 그것이 어떤 종류의 정령인지 단서를 모아 식별해야 한다. Knight는 여기서 "유령의 이름이 아니라 유령의 '유형'을 찾는 게임이라면 어떨까, 그리고 친구들과 함께 집 안을 돌며 증거를 모아 어떤 유형의 유령이 들렸는지 정확히 짚어내는 게임이라면 어떨까"라는 발상을 떠올렸다. 이 "유령 유형 식별" 메카닉이 게임 전체의 근간이 되었다. 여러 영어권 매체가 이를 두고 "《The Witcher 3》가 《Phasmophobia》를 살렸다"고 표현했다. (출처: [TheGamer](https://www.thegamer.com/phasmophobia-the-witcher-3-prologue-quest-saved/), [GameRant](https://gamerant.com/witcher-3-quest-phasmophobia-inspiration/), [vgtimes](https://vgtimes.com/news/129952-how-the-witcher-3-saved-phasmophobias-development-and-inspired-its-core-mechanic-according-to-the-creator.html))

Knight 본인의 동기 역시 단순했다. 그는 "이런 게임이 없었고, 내가 그걸 플레이하고 싶었기 때문에 직접 만들었다"고 밝혔다. 협동 공포 퍼즐 게임을 찾아 Steam을 뒤지다 지친 끝에 스스로 만들기로 한 것이다. (출처: [Yahoo/AT&T 재인용 PC Gamer](https://currently.att.yahoo.com/att/didnt-exist-wanted-play-phasmophobias-142037740.html))

### 유령(캐릭터)

전통적 의미의 "캐릭터"는 없지만, 게임의 진짜 주인공은 유령들이다. 출시 후 지속적으로 추가되어 현재 **27종의 유령**이 존재하며, 이들은 일본·게르만·켈트·이슬람·인도·파키스탄·인도네시아·말레이·헝가리·루마니아·스칸디나비아·중앙아프리카·버마·벨기에·그리스·기독교 전통 등 다양한 문화권의 민속에서 가져온 존재들이다. 각 유령은 고유한 행동 패턴과 약점을 지닌다. 몇 가지 예를 들면 (출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)), [Phasmophobia Wiki - Ghost](https://phasmophobia.fandom.com/wiki/Ghost), [GINX TV](https://www.ginx.tv/en/video-games/phasmophobia-all-ghost-types-and-evidence-to-identify)):

- **Banshee(밴시)**: 한 번에 한 명의 대상만 노리며, 항상 여성이고, 크루시픽스(십자가)를 두려워한다.
- **Demon(데몬)**: 가장 공격적인 유령 중 하나로, 식별 시 주의해야 할 위험한 예외로 분류된다.
- **Mare(메어)**: 조명과 더 자주 상호작용하고 어둠을 선호한다.
- **Spirit(스피릿)**: 가장 기본적이고 위험도가 낮은 유령.
- **Oni**, **Obake** 등: 활동성이 높거나 특수 능력을 지닌 변종들.

### 무드·톤·아트 디렉션

게임의 톤은 "값싼 점프 스케어"가 아니라 "지속적인 긴장과 예측 불가능성"에 기반한다. 어두운 집 안을 손전등 하나에 의지해 돌아다니며, 언제 유령이 발현할지 모르는 불확실성이 공포의 핵심이다. 흥미로운 아트 디렉션 비화도 있다. Knight는 초기에 Unity 스토어의 기성 에셋(stock assets)을 사용해 게임을 만들었는데, 같은 에셋이 다른 게임에도 쓰여 있다 보니 정체성 확립을 위해 출시 이후 그래픽 충실도(graphical fidelity) 개선에 큰 노력을 기울였다고 밝혔다. (출처: [Phasmophobia Wiki - Kinetic Games](https://phasmophobia.fandom.com/wiki/Kinetic_Games))

### 사운드와 음악

사운드 디자인은 이 게임에서 단순한 분위기 장치가 아니라 핵심 게임 메카닉이다. 공간 음향(spatial sound)과 환경음을 통해 유령의 위치와 행동을 추론하고, 마이크를 통한 음성 인식으로 유령과 "대화"한다. 평론가들은 영리한 공간 음향과 환경 음향 효과가 몰입감 있는 세계를 만들어낸다고 일관되게 호평했다. (출처: [Analog Stick Gaming](https://www.analogstickgaming.com/game-reviews/2024/10/27/phasmophobia), [Movies Games and Tech](https://moviesgamesandtech.com/2024/10/28/review-phasmophobia/))

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

### 코어 게임플레이 루프

매 세션(계약, contract)의 기본 흐름은 다음과 같다.

1. **로비/장비 준비**: 트럭(차량) 안에서 조사 장비를 선택하고 맵에 진입한다.
2. **초기 정찰**: 집에 들어가 유령의 활동 방(ghost room)을 찾는다. 온도 저하, 소리, EMF 반응 등으로 위치를 좁힌다.
3. **증거 수집**: 장비를 배치·사용해 일곱 가지 증거 유형 중 해당 유령이 주는 세 가지를 찾아낸다.
4. **유령 식별**: 수집한 증거를 저널에 기록하고 소거법으로 27종 중 정체를 추론한다.
5. **목표 수행**: 추가 부수 목표(특정 행동 유도, 사진 촬영 등)를 완료한다.
6. **탈출**: 완료 후 차량으로 돌아가 세션을 종료한다. 사냥(hunt) 중에는 출입문이 잠기므로 도망치거나 숨어야 한다.

### 증거 시스템

게임에는 일곱 가지 고유 증거가 있고, 기본적으로 각 유령은 그중 세 가지를 제공한다. 주요 장비와 증거는 다음과 같다 (출처: [Phasmophobia Wiki - Evidence](https://phasmophobia.fandom.com/wiki/Evidence), [Steam Guide](https://steamcommunity.com/sharedfiles/filedetails/?id=3044514296)):

- **EMF Reader(EMF 리더)**: 유령 상호작용 시 전자기장 수치를 측정. "EMF 5" 반응이 증거가 된다.
- **Spirit Box(스피릿 박스)**: 여러 라디오 주파수를 순환시켜 백색소음을 만들고, 이를 통해 유령이 음성으로 응답하게 한다. 활성화된 스피릿 박스를 같은 층 7.5미터 이내에서 들고 있으면 사냥 중 유령을 끌어들인다.
- **Thermometer(온도계)**: 영하로 떨어지는 "결빙 온도(freezing temperatures)" 탐지.
- **UV Flashlight/Light(자외선)**: 지문, 발자국 등 흔적 탐지.
- **Ghost Writing Book(고스트 라이팅 북)**: 유령이 직접 글씨를 쓰게 유도.
- **Video Camera/Night Vision(야간 투시 카메라)**: D.O.T.S. 프로젝터를 통해 유령의 실루엣을 포착하거나 유령 구체(ghost orbs)를 탐지.
- **Parabolic/Sound Recorder(음향 녹음 장비)**: 유령 음성 등 청각 증거를 녹음.

### 음성 인식 — 이 게임의 시그니처 메카닉

《Phasmophobia》를 다른 모든 유령 게임과 구별짓는 결정적 기능은 마이크 음성 인식이다. 플레이어가 실제로 입으로 유령에게 말을 걸면, 게임이 그 구절을 인식해 유령이 스피릿 박스로 응답하거나, 화가 나서 물건을 움직이고 조명을 깜빡이게 만든다. 이 기능 때문에 스트리머들이 "유령에게 욕을 했다가 사냥을 유발하고 비명을 지르는" 장면이 트위치에서 대량으로 양산되며 바이럴의 핵심 원동력이 되었다. (출처: [Phasmophobia Wiki - Voice chat](https://phasmophobia.fandom.com/wiki/Voice_chat), [Kotaku](https://kotaku.com/twitchs-latest-horror-sensation-phasmophobia-has-stre-1845362213))

음성 인식 시스템은 두 가지("Voice"와 "System Voice")를 선택할 수 있다. "Voice"는 게임에 존재하는 모든 언어를 지원하고, "System Voice"는 영어·프랑스어·독일어·일본어·중국어·스페인어만 지원한다. 콘솔 버전에서는 VOSK 음성 인식이 구현되어 PS5(DualSense 내장 마이크), PS VR2(헤드셋 내장 마이크), Xbox Series X/S에서 작동한다. (출처: [Kinetic Games](https://www.kineticgames.co.uk/news/phasmophobia-voice-recognition-update), [Phasmophobia Wiki - Voice chat](https://phasmophobia.fandom.com/wiki/Voice_chat))

### 근접 음성 채팅(Proximity Voice)

협동 플레이의 또 다른 핵심은 거리 기반 음성 채팅이다. 로컬/근접 음성은 약 20미터 이내에서 들리며(실제로는 볼륨 감쇠로 더 짧게 느껴진다), 멀리 떨어진 동료와는 라디오(글로벌 채팅)로 소통해야 한다. VR에서는 로컬 음성이 기본적으로 항상 켜져 있고, 라디오로 글로벌 대화를 한다. 이 구조는 팀이 흩어졌을 때의 고립감과 공포를 극대화한다. (출처: [Phasmophobia Wiki - Voice chat](https://phasmophobia.fandom.com/wiki/Voice_chat), [Steam Community](https://steamcommunity.com/app/739630/discussions/0/2998800559182227866/))

### 정신력(Sanity) 시스템

정신력(sanity)은 게임플레이의 여러 요소를 좌우하는 핵심 자원이다. 게임 시작 시 100%에서 출발하며, 어두운 곳을 돌아다닐수록 수동적으로 감소한다. 유령 이벤트나 특정 유령의 능력은 정신력을 더 빠르게 깎는다. 팀의 평균 정신력이 낮을수록 유령이 이벤트·상호작용·사냥 같은 행동을 벌일 확률이 높아진다. 정신력이 충분히 낮아지면 유령이 사냥(hunt)을 시작해 플레이어를 죽이려 든다. 사냥 페이즈 동안 모든 출입문이 잠기므로 플레이어는 사냥이 끝날 때까지 도망치거나 숨어야 한다. 정신력은 진정제(sanity pills)나 일부 저주받은 물건으로 회복할 수 있다. (출처: [Steam Guide](https://steamcommunity.com/sharedfiles/filedetails/?id=3044514296), [GameRant](https://gamerant.com/phasmophobia-ghosts-combat-defense-design-helpless-players/))

이 "무력함의 디자인"은 의도된 것이다. GameRant는 이 게임이 "플레이어를 가능한 한 무력하게 만들고 싶어 한다"고 분석했다. 유령을 공격할 수단이 거의 없고, 십자가로 사냥을 예방하거나 도망치는 것이 전부다.

### 저주받은 물건(Cursed Possessions)

7종의 저주받은 물건은 강력한 효과와 위험을 동시에 안기는 하이리스크-하이리워드 요소다. Ouija Board(위자 보드, 원조), Music Box(뮤직 박스), Haunted Mirror(저주받은 거울), Tarot Cards(타로 카드), Summoning Circle(소환진), Voodoo Doll(부두 인형), Monkey Paw(원숭이 손, 2023년 2월 27일 0.8.1.0 업데이트로 추가). 각 물건은 맵당 1/7 확률로 등장하며, 표준 미션에서는 하나만 스폰된다. (출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)), [MSN/GameRant](https://www.msn.com/en-us/news/technology/all-cursed-object-locations-in-phasmophobia/ar-AA1LZRgf))

### 맵 / 진행 구조

현재 총 14개의 맵이 존재하며, 소형 7개·중형 5개·대형 2개로 구성된다. 대표적인 맵은 다음과 같다 (출처: [Phasmophobia Wiki - Map](https://phasmophobia.fandom.com/wiki/Map), [TheGamer](https://www.thegamer.com/phasmophobia-location-maps-ranked/), [KeenGamer](https://www.keengamer.com/articles/guides/phasmophobia-all-maps-guide-breaker-locations-best-looping-spots-and-many-more/)):

- **6 Tanglewood Drive**: 입문용 소형 주택 맵. 2층 11개 방.
- **Grafton Farmhouse**: 마지막 소형 맵으로 분류되는 농가. 넓은 방 때문에 사냥 중 탈출이 어렵다.
- **Prison(교도소)**: Sunny Meadows의 축소판 격. 29개 방, 2층의 복잡한 구조.
- **Sunny Meadows Mental Institution**: 69개 방의 거대한 정신병원 맵. 예배당·시체안치소·제한구역 등으로 구성된 가장 상세하고 무서운 대형 맵.
- **Sunny Meadows Restricted**: 위 맵을 무작위로 축소한 버전. 매번 세 구역만 개방된다.
- **Asylum(구버전)**: 출시 당시 유일한 대형 맵으로 119개 방을 가졌으나, 2022년 9월 27일 더 정교한 Sunny Meadows로 대체되며 제거되었다.

### 난이도 / 진척도 / 경제 시스템

다섯 가지 주 난이도가 있다: **Amateur, Intermediate(레벨 10 해금), Professional(레벨 15 해금), Nightmare(레벨 20 해금), Insanity**. 난이도가 올라갈수록 정신력 감소 속도가 빨라지고(Professional은 200% 비율), 사망 시 장비 가치를 잃으며, 도구 일부가 손상되는 등 페널티가 커지지만 보상 배수도 함께 늘어난다(Professional 3배, Nightmare 4배, Insanity 6배). (출처: [Phasmophobia Wiki - Difficulty](https://phasmophobia.fandom.com/wiki/Difficulty), [GINX TV](https://www.ginx.tv/en/phasmophobia/difficulty-levels-differences-explained))

경제는 계약 보상금(money)으로 돌아간다. 플레이어는 목표 완수와 부수 증거 발견에 따라 돈을 벌고, 이를 장비 구매·업그레이드에 쓴다. 정확한 유령 식별, 3개 목표 완수, 뼈(bone) 수집, 고유 미디어로만 저널을 채우면 50달러의 "완벽한 조사 보너스(Perfect Investigation Bonus)"를 받는다. 이론상 단일 계약 최대 수익은 특정 조건(Blood Moon 날씨, 대형 맵, Obake 상대 완벽 게임)에서 14,261달러, 특수 이벤트일의 데일리·위클리 과제까지 더하면 22,861달러에 이른다. (출처: [Phasmophobia Wiki - Money](https://phasmophobia.fandom.com/wiki/Money), [Phasmophobia Wiki - Experience](https://phasmophobia.fandom.com/wiki/Experience))

### 진척도 철학: 라이브 서비스의 거부

여기서 이 게임의 가장 독특한 운영 철학이 드러난다. Knight는 PCGamesN 인터뷰에서 라이브 서비스 모델을 명시적으로 거부한다.

- "우리는 절대 우리 자신을 라이브 서비스라고 부르지 않을 것이다. 그 길로 가고 싶지 않다." ("We'll never call ourselves a live service. We don't want to go down that route.")
- "우리는 마이크로트랜잭션이나 DLC 같은 게 없다. 오직 최초 판매만 있다." ("We don't have microtransactions or DLCs or anything like that. We only have the initial sale.")
- "라이브 서비스 게임은 격월로 업데이트가 나온다. 우리는 그런 압박을 우리 자신에게 가하고 싶지 않다."
- "우리에게 진척도란 곧 지식이다. 모든 유령에 대해 배울 것이 너무나 많다." ("The progression for us is knowledge.")

즉, 인위적 보상 트레드밀이 아니라 "재미있어서 플레이하는 게임"을 만드는 것이 목표라는 것이다. (출처: [PCGamesN](https://www.pcgamesn.com/phasmophobia/live-service-interview))

### 접근성 / 멀티플레이

게임은 1인 솔로도 가능하지만, 본질적으로 4인 협동 경험으로 설계되었다. 평론가들은 "솔로로도 할 수 있지만, 그것은 협동/경쟁 스포츠를 혼자 하는 것과 같아서 가능하긴 하나 만족스럽지 않다"고 평했다. 콘솔 출시 이후에는 PC·PS5·Xbox 간 완전한 크로스플레이를 지원한다. (출처: [Niche Gamer](https://nichegamer.com/reviews/phasmophobia-early-access-review/), [DayOne](https://playday.one/2024/10/18/phasmophobia-comes-to-consoles-ps-vr2-29th-october-full-crossplay-support/))

---

## 4. 평가

### 평론 점수와 인용

《Phasmophobia》는 얼리 액세스 상태로 출시되어 전통적인 Metacritic 메타스코어 집계는 제한적이지만, 영어권 매체에서 일관되게 높은 평가를 받았다. 주요 인용은 다음과 같다 (출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game))):

- **PC Gamer (Rich Stanton)**: "지금까지 만들어진 최고의 유령 게임(the best ghost game ever made)"
- **IGN**: 2023년 8월 이후 "PC 최고의 공포 게임 12선"에 포함
- **GameRant**: "Steam에서 즐길 수 있는 최고의 공포 게임"
- **CBR**: "할로윈 시즌을 위한 완벽한 게임"
- **Jeuxvideo.com**: 20점 만점에 16점, 독창성과 진척도 페이싱을 호평

PC Gamer는 또한 2020년 자체 선정에서 《Phasmophobia》를 **Best Co-op Game 2020(2020 최고의 협동 게임)**으로 뽑았다. (출처: [PC Gamer](https://www.pcgamer.com/best-co-op-game-2020-phasmophobia/))

### 수상 이력

| 시상식 | 일자 | 부문 | 결과 |
|--------|------|------|------|
| The Game Awards 2020 | 2020년 12월 10일 | Best Debut Game (최우수 데뷔 게임) | **수상** |
| Steam Awards 2020 | 2021년 1월 3일 | VR Game of the Year | 후보 |
| Game Developers Choice Awards | 2021년 7월 21일 | Best Debut Developer (최우수 데뷔 개발사) | **수상** |

(출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)), [The Game Awards](https://thegameawards.com/winners/best-debut-indie-game), [Screen Rant](https://screenrant.com/phasmophobia-best-debut-game-awards/))

The Game Awards 2020에서는 같은 부문 후보였던 《Carrion》 등을 제치고 수상했다. 이는 출시 약 3개월 만에 거둔 성과로, 1인 개발 인디 게임으로서는 이례적이었다.

### 상업 지표

상업적 성공은 폭발적이었다 (출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)), [Game Developer](https://www.gamedeveloper.com/business/phasmophobia-sales-1-million-console-copies), [Rely on Horror](https://www.relyonhorror.com/latest-news/phasmophobia-surpasses-20-million-copies-sold/), [LEVVVEL](https://levvvel.com/phasmophobia-statistics/)):

- **2020년 10월**: 동시 접속자 약 86,000명 돌파(약 10월 10일경). 트위치 시청 순위 5위 안에 진입하며 《Among Us》, 《Fortnite》, 《FIFA 21》, 《Genshin Impact》를 추월. 10월 한 달 트위치에서 여섯 번째로 많이 시청된 게임.
- **2020년 10~11월**: 3주 연속 Steam 글로벌 판매 1위. 10월 말 시점 《Fall Guys》와 《Cyberpunk 2077》(예약 구매)까지 앞섰다.
- **Steam 역대 최고 동접**: 약 112,717명.
- **2024년 11월**: 누적 판매 약 2,000만 장 돌파.
- **2024년 12월**: 콘솔 판매 100만 장 돌파, 총 판매 약 2,200만 장.
- **2025년 2월**: PS5·PS VR2·Xbox 콘솔 합산 200만 장 돌파(출시 104일 만).
- **2025년 7월**: 누적 2,500만 장 돌파.
- **2025년 6월(영화화 발표 시점)**: 글로벌 누적 2,300만 장 이상으로 보도.
- **2026년 4월 기준**: 전 세계에서 50번째로 많이 팔린 비디오 게임으로 집계.

### 유저 평가

Steam 유저 평가는 출시 이후 오랫동안 "압도적으로 긍정적(Overwhelmingly Positive)"을 유지했다. 약 80만 건 이상의 평가에서 약 95~96%의 긍정 비율을 기록했다(예: 817,604건 기준 96/100, 또는 804,386건 기준 95.67% 긍정). 이는 인디 게임으로서 극히 이례적인 수치다. (출처: [Steambase](https://steambase.io/games/phasmophobia/reviews), [SteamDB](https://steamdb.info/app/739630/charts/))

다만 2026년 5월 캐릭터 업데이트 이후 일시적으로 평가가 75% 수준까지 하락하는 변동을 겪었다(아래 6장 참조).

### 평론-유저 괴리

본 게임은 평론(거의 만장일치 호평)과 유저 평가(장기간 압도적 긍정)가 대체로 일치한 드문 사례다. 괴리가 발생한 것은 평론이 아니라 특정 업데이트에 대한 기존 팬층의 반발(리뷰 폭탄) 국면에서였다.

---

## 5. 성공 요인 분석 (핵심)

### 디자인 측면

1. **재발명된 코어 루프**: "유령 사냥"은 새로운 소재가 아니지만, 《Phasmophobia》는 그것을 "증거를 모아 27종 중 정체를 추리한다"는 정밀한 연역 게임으로 바꿨다. 《The Witcher 3》의 "Devil by the Well" 퀘스트에서 가져온 이 "유형 식별" 메카닉이 반복 플레이의 깊이를 만들었다.

2. **음성 인식이라는 시그니처**: 마이크로 유령에게 직접 말을 거는 기능은 다른 어떤 게임에도 없던 차별점이었고, 동시에 스트리밍에 완벽하게 최적화된 "콘텐츠 생성기"였다.

3. **무력함의 공포**: 플레이어가 유령을 이길 수 없게 만든 디자인이 진정한 공포를 만들었다. 점프 스케어 대신 예측 불가능성과 긴장에 의존한 점을 평론가들이 일관되게 호평했다.

4. **협동의 사회적 공포**: 근접 음성 채팅으로 동료와 떨어졌을 때의 고립감, 그리고 함께 비명 지르는 공유 경험이 솔로 공포 게임과 다른 매력을 만들었다.

### 마케팅/출시 전략과 타이밍

이 게임의 성공에서 마케팅 예산이 차지한 비중은 거의 없다. 1인 개발자에게 마케팅 자금이 있을 리 없었다. 대신 결정적이었던 것은 **타이밍과 인플루언서 효과**다.

- **COVID-19 봉쇄**: 2020년 9월 출시는 팬데믹 봉쇄 한가운데였다. 멀리 떨어진 친구들이 함께 즐길 수 있는 협동 공포 게임이라는 점이 격리된 사람들에게 완벽하게 맞았다.
- **할로윈 시즌**: 9월 출시 후 10월 할로윈 시즌과 맞물려 공포 게임 수요가 폭발했다.
- **트위치/유튜브 바이럴**: 음성 인식과 4인 협동의 비명-코미디가 스트리밍에 최적이었다. 2020년 10월 다수의 대형 스트리머·유튜버가 플레이하며 트위치 시청 5위권에 진입했고, 이것이 판매로 직결되어 3주 연속 Steam 1위를 만들었다. Kotaku는 이를 "트위치 최신 공포 센세이션"이라 보도했다.

(출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)), [Kotaku](https://kotaku.com/twitchs-latest-horror-sensation-phasmophobia-has-stre-1845362213), [GameRant](https://gamerant.com/phasmophobia-indie-horror-ghost-hunting-games-genre-influence/))

### 개발/운영 방법론

- **자체 자금·자체 퍼블리싱**: 외부 압박 없이 자체 마일스톤을 정하는 구조가, 빠른 성공 후에도 장기적·지속 가능한 운영을 가능케 했다.
- **라이브 서비스 거부**: MTX·DLC 없이 최초 판매만으로 운영하면서, "격월 업데이트"의 압박을 거부하고 무료 콘텐츠 업데이트로 신뢰를 쌓았다.
- **얼리 액세스의 장기 활용**: 출시 후 3년 이상에 걸쳐 여러 대형 콘텐츠 업데이트를 무료로 제공하며 커뮤니티를 유지했다.

### 동시기 작품 대비 차별점

2020년에는 《Among Us》, 《Fall Guys》 같은 소셜·협동 게임들이 팬데믹 호황을 누렸다. 《Phasmophobia》는 이들과 같은 "친구와 함께하는 가벼운 소셜 경험"의 흐름을 타면서도, 공포라는 강렬한 감정과 음성 인식이라는 독자적 메카닉으로 차별화했다. 다른 협동 게임이 웃음을 줬다면, 《Phasmophobia》는 비명을 줬다.

---

## 6. 비평적 시각 / 한계 / 논란

### 디자인적 약점

1. **얼리 액세스의 거친 부분**: 초기 평론들은 애니메이션 불일치, 일부 UI의 투박함을 지적했다(이후 업데이트로 다수 개선). (출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)))
2. **솔로 플레이의 한계**: 본질적으로 협동 게임이라 혼자 하면 재미가 크게 반감된다는 점이 거의 모든 평론에서 언급되었다.
3. **장기 반복성**: 코어 루프가 강력하지만 본질적으로 반복적이며, 신규 콘텐츠 사이의 텀이 길면 권태가 올 수 있다는 지적.

### 운영 이슈: 콘솔 출시 지연

콘솔 버전은 수차례 연기되었다. 당초 2023년 8월 예정이었다가 10월로, 다시 "예기치 못한 난관"으로 추가 연기되었다. 특히 Kinetic Games의 사우샘프턴 사무실 화재가 콘솔 개발에 상당한 지연을 초래했다. 최종적으로 PS5·PS VR2·Xbox Series 버전은 2024년 10월 29일에야 출시되었다. (출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)), [PlayStation LifeStyle](https://www.playstationlifestyle.net/2024/10/18/phasmophobia-ps5-release-date-october-2024/))

### 가장 큰 논란: 2026년 5월 캐릭터 업데이트 리뷰 폭탄

장기간 "압도적으로 긍정적" 평가를 유지하던 게임이 처음으로 심각한 유저 반발을 맞은 사건이다. Kinetic Games는 2026년 5월 5일 Player Character Update(0.17.0.0)를 출시했는데, 반응이 즉각적이고 가혹했다. (출처: [PC Gamer](https://www.pcgamer.com/games/horror/we-want-to-start-today-by-apologising-phasmophobia-is-fixing-issues-with-its-player-character-update-after-a-slew-of-complaints/), [GAMES.GG](https://games.gg/news/phasmophobia-review-bombed-character-update/), [The Escapist](https://www.escapistmagazine.com/news-phasmophobia-reviews-tumble-after-character-update/))

- **리뷰 급락**: 5월 한 달간 긍정 약 600건 대 부정 약 2,000건으로 역전. 전체 평가가 일시적으로 75% 수준까지 하락.
- **"휘는 등(bendy backs)" 제거 논란**: 5년간 이어진 물리법칙을 무시하는 우스꽝스러운 애니메이션이 팬들에게 사랑받는 "고유의 매력"으로 자리 잡았는데, 이를 제거한 것이 상당수 플레이어를 분노케 했다.
- **신규 기술 문제**: 손과 오브젝트 정렬 오류, 손전등 시야 가림, 저널 가독성, 아이템 상호작용 감각 등 다수의 불만.
- **코스메틱 그라인드**: 기대보다 적은 커스터마이징 옵션과, 일부 보상이 상당한 시간 투자가 필요한 프레스티지 조건 뒤에 잠긴 점.

개발사 대응으로 Kinetic Games는 이례적으로 사과문을 발표했다. "우리는 오늘 먼저 사과로 시작하고자 한다(We want to start today by apologising)"며 "우리의 약속을 지키지 못했다(didn't deliver on our promises)"고 인정하고 수정을 약속했다. 이 사건은 장수 게임이 핵심 팬층의 정체성과 충돌하는 변경을 가했을 때의 위험을 잘 보여주는 사례다.

### 평가가 갈리는 지점

- **얼리 액세스 장기화**: 출시 5년이 넘도록 정식 1.0이 나오지 않은 점에 대해 일부 비판. (출처: [PC Gamer](https://www.pcgamer.com/phasmophobia-will-linger-in-early-access-longer-than-planned/))
- **클론 게임과의 비교**: 《Demonologist》, 《Ghost Watchers》 등 후발 주자들이 더 화려한 비주얼을 내세우면서, 《Phasmophobia》의 그래픽이 상대적으로 낡았다는 지적도 나왔다.

---

## 7. 영향과 유산

### 장르에 미친 영향

《Phasmophobia》는 사실상 "협동 유령 사냥 시뮬레이션"이라는 하위 장르를 정의한 작품이다. 출시 이후 그 공식 — 팀 기반 조사, 장비 시스템, 유령 식별, 음성 인식 — 을 차용한 게임들이 쏟아졌다. (출처: [GameRant](https://gamerant.com/phasmophobia-indie-horror-ghost-hunting-games-genre-influence/), [Screen Rant](https://screenrant.com/phasmophobia-demonologist-coop-comparison/), [TheGamer](https://www.thegamer.com/phasmophobia-like-co-op-horror-games/))

### 후속작/모방작/장르 확장

- **Demonologist**: 가장 직접적으로 영향받은 후발작. 더 화려한 비주얼로 인기를 끌었다.
- **Ghost Exorcism INC.** (2021년 중반): 느린 유령 식별 과정과 음성 인식 메카닉을 그대로 차용.
- **Forewarned**: 고대 이집트 유적을 배경으로, 협동·장비·식별 구조를 《Phasmophobia》에서 가져왔다.
- **Ghost Watchers**: 유사 메카닉으로 인기 급상승.
- **Ghost Hunter Corps** 등 다수의 협동 공포 게임이 이 흐름 속에서 등장했다.

GameRant는 "정식 출시도 하지 않은 채로 《Phasmophobia》가 인디 공포 산업과 커뮤니티의 명백한 정의적 힘이 되었다"고 평했다.

### 산업적 의미

1. **1인 인디의 가능성 증명**: 마케팅 예산 없이, 기성 Unity 에셋으로 시작한 1인 프로젝트가 글로벌 메가 히트가 될 수 있음을 보여줬다. 이는 인디 개발자들에게 강력한 사례가 되었다.
2. **반(反) 라이브 서비스 모델의 성공**: MTX·DLC 없이 최초 판매만으로 2,500만 장을 판 사례는, "트레드밀" 없이도 장기 성공이 가능함을 입증했다.
3. **Kinetic Publishing 설립**: Knight는 성공을 바탕으로 다른 인디 게임을 지원하는 퍼블리싱 레이블 Kinetic Publishing을 출범시켰다. 그는 "사람을 고용하기 시작했을 때부터, 심지어 혼자였을 때부터 늘 궁극의 목표였다"고 밝혔다. (출처: [VGC](https://www.videogameschronicle.com/news/phasmophobias-creator-is-launching-kinetic-publishing-to-champion-indies/), [GameSpot](https://www.gamespot.com/articles/phasmophobia-studio-wants-its-new-publishing-label-to-explore-more-than-scares/1100-6538736/), [Unity Blog](https://unity.com/blog/kinetic-publishing-indie-games))

### 문화적 의미

- **스트리밍 시대의 게임**: 《Phasmophobia》는 "보기 좋은 게임이 잘 팔린다"는 트위치 시대의 공식을 완벽히 구현했다. 음성 인식과 협동 비명은 클립으로 무한 재생산되었다.
- **할리우드 진출**: 2025년 6월, Blumhouse Productions와 Atomic Monster가 Kinetic Games와 협력해 영화화를 발표했다(배급사·개봉일 미정). 이는 Blumhouse가 《Five Nights at Freddy's》(2023) 성공 이후 추진하는 또 다른 게임 원작 영화다. (출처: [Variety](https://variety.com/2025/film/news/phasmophobia-movie-in-development-blumhouse-1236417534/), [Deadline](https://deadline.com/2025/06/phasmophobia-film-adaptation-blumhouse-1236422753/), [Kinetic Games](https://kineticgames.co.uk/news/phasmophobia-film-adaptation-blumhouse))
- **플랫폼 확장**: 2024년 콘솔 진출, 2026년 Nintendo Switch 2 이식 발표(The Game Awards 2025)로 IP의 생명력이 계속 확장되고 있다.

---

## 8. 부록

### 주요 업데이트 타임라인

| 시기 | 업데이트/사건 | 내용 |
|------|---------------|------|
| 2019년 12월 | 초기 알파 체인지로그 | 작업명 《Spectrophobia》 |
| 2020년 3월 3일 | 명칭 변경 | 게임명 《Phasmophobia》, 회사명 Kinetic Games로 변경, Steam 페이지 공개 |
| 2020년 6월 | 발표 트레일러 | VR 지원·얼리 액세스 공개 |
| 2020년 9월 18일 | 얼리 액세스 출시 | Windows, 14달러 |
| 2020년 10월 | 바이럴 폭발 | 트위치 5위권, Steam 1위 |
| 2022년 9월 27일 | Apocalypse 업데이트 | 구 Asylum 맵을 Sunny Meadows로 대체, 메인 메뉴 보드·Custom Difficulty 추가 |
| 2023년 2월 27일 | 0.8.1.0 | Monkey Paw(저주받은 물건) 추가 |
| (Ascension 업데이트) | 레벨링/프레스티지 개편 | 레벨링 시스템 개편 및 프레스티지 시스템 도입 |
| 2024년 10월 29일 | 콘솔 출시 | PS5, PS VR2, Xbox Series X/S, 완전 크로스플레이, 19.99달러 |
| 2025년 (Chronicle) | 미디어 시스템 개편 | 저널 Media 탭, Sound Recorder 신규 장비 |
| 2026년 5월 5일 | Player Character Update(0.17.0.0) | 캐릭터 모델/애니메이션 개편 → 리뷰 폭탄 논란 |
| 2026년 (예정) | Nintendo Switch 2 이식 | The Game Awards 2025에서 발표 |
| (예정) | 1.0 정식 출시 | 원래 명칭 "Horror 2.0", 사냥·이벤트·상호작용 개편 및 로어 보강 |

(출처: [Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game)), [Phasmophobia Wiki - Planned updates](https://phasmophobia.fandom.com/wiki/Planned_updates_and_features), [Kinetic Games Roadmap](https://kineticgames.co.uk/news/phasmophobia-2025-roadmap), [dotesports](https://dotesports.com/phasmophobia/news/phasmophobia-2025-roadmap))

### 핵심 통계 표

| 지표 | 수치 | 출처/시점 |
|------|------|-----------|
| 얼리 액세스 출시일 | 2020년 9월 18일 | Wikipedia |
| 출시 가격 | 14달러(현재 19.99달러) | Steam |
| 유령 종류 | 27종 | Wikipedia |
| 증거 유형 | 7종(유령당 3종) | Phasmophobia Wiki |
| 맵 수 | 14개(소형 7·중형 5·대형 2) | Phasmophobia Wiki |
| 저주받은 물건 | 7종 | Wikipedia |
| 난이도 | 5단계(Amateur~Insanity) | Phasmophobia Wiki |
| Steam 역대 최고 동접 | 약 112,717명 | LEVVVEL |
| 2020년 10월 동접 피크 | 약 86,000명 | Wikipedia |
| Steam 유저 평가 | 약 95~96% 긍정(80만+ 건) | Steambase |
| 누적 판매(2025년 7월) | 2,500만 장 | LEVVVEL/WN Hub |
| 콘솔 판매(2025년 2월) | 200만 장(104일) | Wikipedia |
| 개발 인력 | 1인 → 약 32인 | PCGamesN |

### 주요 인터뷰 및 자료

- Daniel Knight 인터뷰 — 라이브 서비스 거부 철학: [PCGamesN](https://www.pcgamesn.com/phasmophobia/live-service-interview)
- 《The Witcher 3》가 코어 메카닉에 준 영감: [TheGamer](https://www.thegamer.com/phasmophobia-the-witcher-3-prologue-quest-saved/), [GameRant](https://gamerant.com/witcher-3-quest-phasmophobia-inspiration/)
- 1인 개발자에서 팀으로의 성장: [PCGamesN](https://www.pcgamesn.com/phasmophobia/developer-update), [GameSpot](https://www.gamespot.com/articles/phasmophobia-dev-is-preparing-to-shake-things-up-again/1100-6535210/)
- Kinetic Publishing 설립: [VGC](https://www.videogameschronicle.com/news/phasmophobias-creator-is-launching-kinetic-publishing-to-champion-indies/), [Unity Blog](https://unity.com/blog/kinetic-publishing-indie-games)
- Eurogamer × Daniel Knight 인터뷰(CHRONICLE 출시 즈음, 초기 개발사부터): [X/PlayPhasmo 안내](https://x.com/PlayPhasmo/status/1944791286331904172)
- 캐릭터 업데이트 사과/논란: [PC Gamer](https://www.pcgamer.com/games/horror/we-want-to-start-today-by-apologising-phasmophobia-is-fixing-issues-with-its-player-character-update-after-a-slew-of-complaints/)
- 영화화 발표: [Variety](https://variety.com/2025/film/news/phasmophobia-movie-in-development-blumhouse-1236417534/), [Deadline](https://deadline.com/2025/06/phasmophobia-film-adaptation-blumhouse-1236422753/)

### 참고 자료 목록 (영어권 매체 중심)

- [Phasmophobia (video game) — Wikipedia](https://en.wikipedia.org/wiki/Phasmophobia_(video_game))
- [Phasmophobia on Steam](https://store.steampowered.com/app/739630/Phasmophobia/)
- [PC Gamer — Best Co-op Game 2020](https://www.pcgamer.com/best-co-op-game-2020-phasmophobia/)
- [PC Gamer — Will linger in Early Access](https://www.pcgamer.com/phasmophobia-will-linger-in-early-access-longer-than-planned/)
- [Kotaku — Twitch's Latest Horror Sensation](https://kotaku.com/twitchs-latest-horror-sensation-phasmophobia-has-stre-1845362213)
- [GameSpot — Dev Is Preparing To Shake Things Up Again](https://www.gamespot.com/articles/phasmophobia-dev-is-preparing-to-shake-things-up-again/1100-6535210/)
- [GameRant — Major Impact on Indie Horror](https://gamerant.com/phasmophobia-indie-horror-ghost-hunting-games-genre-influence/)
- [Screen Rant — Demonologist Co-Op Comparison](https://screenrant.com/phasmophobia-demonologist-coop-comparison/)
- [Game Developer — 1 Million Console Copies](https://www.gamedeveloper.com/business/phasmophobia-sales-1-million-console-copies)
- [Rely on Horror — Surpasses 20 Million](https://www.relyonhorror.com/latest-news/phasmophobia-surpasses-20-million-copies-sold/)
- [LEVVVEL — Phasmophobia Statistics](https://levvvel.com/phasmophobia-statistics/)
- [The Game Awards — Best Debut Indie Game Winners](https://thegameawards.com/winners/best-debut-indie-game)
- [Variety — Blumhouse Film Adaptation](https://variety.com/2025/film/news/phasmophobia-movie-in-development-blumhouse-1236417534/)
- [Phasmophobia Wiki (Fandom) — Evidence, Map, Ghost, Difficulty, Money, Voice chat 등](https://phasmophobia.fandom.com/wiki/Evidence)

---

*본 분석서는 2026년 5월 기준으로 영어권 매체와 개발사 공개 자료를 바탕으로 작성되었으며, 모든 수치와 날짜는 명시된 출처에 근거한다. 얼리 액세스 게임 특성상 일부 콘텐츠 수치(유령 종류, 맵 수 등)는 향후 업데이트로 변동될 수 있다.*
