# Untitled Goose Game (2019) 심층 분석

> "It's a lovely morning in the village, and you are a horrible goose."
> ("마을엔 사랑스러운 아침이 밝았고, 당신은 끔찍한 거위입니다.")
> — 게임 공식 카피이자, 거의 모든 리뷰의 첫 문장이 된 한 줄

2019년 9월, 단 네 명의 호주 멜버른 개발자가 만든 작은 인디 게임 한 편이 트위터 타임라인과 레딧, 그리고 셀럽들의 입소문을 타고 그해 가장 화제가 된 비디오 게임 중 하나로 떠올랐다. AAA 대작들이 수백 명의 인력과 수천만 달러를 쏟아붓던 한 해에, 거위 한 마리가 영국 시골 마을 주민들을 골탕 먹이는 이 게임은 발매 3개월 만에 100만 장을 팔았고, 이듬해 D.I.C.E.와 GDC에서 동시에 '올해의 게임'을 거머쥐며 인디 게임으로서는 이례적인 대관식을 치렀다. 본 분석서는 *Untitled Goose Game*의 개발사 비화부터 핵심 메카닉, 평가, 밈 바이럴 현상, 그리고 짧은 플레이타임 논쟁까지를 장문으로 다룬다.

---

## 1. 게임 개요

### 기본 정보

| 항목 | 내용 |
|---|---|
| 정식 명칭 | Untitled Goose Game (직역: 무제 거위 게임) |
| 개발사 | House House (호주 멜버른) |
| 퍼블리셔 | Panic Inc. (미국 오리건주 포틀랜드) |
| 장르 | 스텔스 퍼즐 / 샌드박스 / 코미디 액션 |
| 엔진 | Unity |
| 최초 출시일 | 2019년 9월 20일 (macOS, Nintendo Switch, Windows) |
| 추가 출시일 | 2019년 12월 17일 (PlayStation 4, Xbox One) |
| 스팀/itch.io 출시 | 2020년 9월 23일 (멀티플레이어 업데이트와 동시) |
| 음악 | Dan Golding (클로드 드뷔시 《전주곡집》 편곡) |

(출처: [Wikipedia – Untitled Goose Game](https://en.wikipedia.org/wiki/Untitled_Goose_Game))

### 개발사 House House

House House는 호주 멜버른에 기반을 둔 독립 게임 스튜디오로, **Nico Disseldorp, Stuart Gillespie-Cook, Jacob(Jake) Strasser, Michael McMaster** 네 명의 공동 창립자로 구성되어 있다. *Untitled Goose Game*은 이 스튜디오의 두 번째 작품으로, 데뷔작은 2016년에 내놓은 로컬 멀티플레이어 물리 게임 *Push Me Pull You*였다.

House House는 데뷔작과 마찬가지로 호주 빅토리아주의 영화·미디어 진흥 기관인 **Film Victoria**의 지원을 받았다. 개발자 Stuart Gillespie-Cook은 이 지원이 "우리를 지속 가능하게 만들고, 진짜 스튜디오로 만들어 주었다(making us sustainable and making us into a real studio)"고 회고했다. 즉, 이 게임은 호주 정부의 게임 산업 육성 정책이라는 제도적 토양 위에서 탄생한 작품이기도 하다. (출처: [Game Developer – Road to the IGF](https://www.gamedeveloper.com/game-platforms/road-to-the-igf-house-house-s-i-untitled-goose-game-i-))

### 퍼블리셔 Panic Inc.의 역할

퍼블리셔는 미국 포틀랜드의 소프트웨어 회사 **Panic Inc.**가 맡았다. Panic은 본래 macOS용 개발 도구(Coda, Transmit 등)와 핸드헬드 게임기 Playdate로 알려진 회사로, *Firewatch*(Campo Santo)에 이은 두 번째 퍼블리싱 프로젝트가 바로 이 게임이었다. 중요한 점은 **Panic의 역할이 자금 지원과 마케팅에 한정되었고, House House가 지식재산권(IP)을 온전히 보유했다**는 것이다. 이는 작은 인디 스튜디오가 창작 통제권을 지키면서도 안정적인 퍼블리싱 파이프라인을 확보한 모범 사례로 자주 언급된다. (출처: [Wikipedia](https://en.wikipedia.org/wiki/Untitled_Goose_Game), [Portland Monthly](https://www.pdxmonthly.com/arts-and-culture/2019/10/this-portland-published-video-game-has-taken-the-internet-by-storm))

### 개발 규모

핵심 개발 인력은 사실상 **4인 팀**이었으며, 여기에 작곡/사운드를 담당한 Dan Golding이 외부 협력자로 합류했다. 정확한 개발 예산은 공개된 바 없으나[추정], Film Victoria의 보조금과 Panic의 펀딩이 주요 재원이었다. 기획부터 발매까지의 개발 기간은 2016년 후반 아이디어 발상, 2017년 트레일러 공개, 2019년 발매에 이르는 약 2~3년에 걸쳐 진행되었다.

---

## 2. 게임 설명: 이 게임이 대체 무엇인가

### 컨셉 한 줄 요약

플레이어는 영국 어느 한적한 시골 마을에 침입한 **한 마리의 길거리 거위**가 되어, 마을 주민들의 평화로운 아침을 조직적으로, 그리고 의도적으로 망쳐 놓는다. 전투도, 폭력도, 죽음도 없다. 오직 거위 한 마리가 할 수 있는 일 — 꽥꽥거리고(honk), 뒤뚱대고, 부리로 물건을 훔치고, 사람을 골탕 먹이는 것 — 만으로 이루어진 게임이다.

### 세계관과 톤

게임의 무대는 시간대가 모호한, 그러나 명백히 영국적인 전원 마을이다. 잘 손질된 정원, 펍, 잡화점, 마을 광장 같은 공간이 아이소메트릭(쿼터뷰) 시점으로 깔끔하게 펼쳐진다. 등장하는 인간 NPC들은 정원사, 잡화점 주인, 한 쌍의 노부부, 펍 주인, 그리고 한 소년 등으로, 모두 둥글둥글하고 표정이 단순화된 만화적 디자인을 갖고 있다. 줄거리라 할 만한 서사는 없다. 거위에게는 동기도, 배경 설정도, 대사도 주어지지 않는다. **"당신은 끔찍한 거위입니다"**라는 한 줄이 사실상 이 게임의 전부이자 모든 것이다.

이 의도적인 서사의 공백이야말로 게임의 핵심 미학이다. 거위가 왜 마을을 괴롭히는지에 대한 설명은 없고, 그 빈자리를 플레이어 각자의 상상과 해석이 채운다. 영국 비평지 *Frieze*는 이 게임을 두고 "나쁜 짓을 하는 것이 왜 이렇게 기분 좋은가(Why It Feels Good to Be Bad)"라는 제목으로 다뤘는데, 이는 게임이 제공하는 핵심적 쾌감 — 결과에 대한 책임 없이 마음껏 말썽을 부리는 해방감 — 을 정확히 짚은 것이다. (출처: [Frieze](https://www.frieze.com/article/untitled-goose-game-and-why-it-feels-good-be-bad))

### 아트 디렉션

미니멀하고 평면적인 셀 셰이딩(cel-shading) 스타일의 3D 그래픽을 사용한다. 색감은 파스텔톤으로 부드럽고, 그림자와 디테일은 과감히 생략되어 있다. 캐릭터의 표정은 거의 변하지 않고, 동작과 상황만으로 코미디를 전달한다. 이 절제된 비주얼은 1인칭 시점이 아니라 약간 떨어진 시점에서 상황 전체를 무대 위 한 컷처럼 조망하게 만들어, 마치 무성영화나 만화 칸을 보는 듯한 느낌을 준다.

### 사운드와 음악 — 이 게임의 숨은 주인공

음악은 *Untitled Goose Game*에서 단순한 배경음을 넘어선 핵심 디자인 요소다. 작곡가 **Dan Golding**(사운드트랙 큐레이션 및 편곡 담당)은 새로 곡을 작곡하는 대신, **클로드 드뷔시(Claude Debussy)의 솔로 피아노 《전주곡집(Préludes)》 중 6곡**을 발췌·편곡했다. 무성영화 시대 영화관에서 피아니스트가 화면을 보며 즉흥적으로 반주하던 전통에서 영감을 얻은 선택이었다. (출처: [Game Developer – Getting goosey with Debussy](https://www.gamedeveloper.com/audio/getting-goosey-with-debussy-creating-an-adaptive-score-for-i-untitled-goose-game-i-))

이 음악 시스템의 진짜 혁신은 **동적·반응형(adaptive/reactive) 구현**에 있다. Golding의 작업 방식을 정리하면 다음과 같다.

- 각 전주곡을 **두 가지 버전**으로 녹음했다. 하나는 평범한 연주 버전, 다른 하나는 더 느리고 에너지가 낮은(low-energy) 버전이다.
- 이 두 버전을 각각 **약 300~400개(자료에 따라 196~425개)의 1~3초짜리 짧은 스템(stem) 조각**으로 분해했다.
- 게임은 플레이어의 행동(거위가 가만히 있는지, 사고를 치는지, 도망치는지)에 따라 어느 버전의 어느 조각을 다음에 재생할지 실시간으로 선택한다.
- 그 결과, 음악은 마치 **눈앞의 상황을 지켜보며 즉흥 반주하는 라이브 피아니스트**처럼 거위의 행동에 정확히 반응한다. 거위가 사고를 치면 음악이 격렬하고 빠르게 몰아치고, 거위가 숨죽이고 있으면 음악도 잦아든다.

Golding에 따르면 게임 첫 번째 전주곡 하나만 해도 가능한 변주의 경우의 수가 **0이 52개 붙은 숫자(a number with 52 zeros after it)**에 달해, 수학적으로는 모든 플레이어가 매번 서로 다른 연주를 듣게 된다. (출처: [ZoneOut](https://www.zoneout.com/untitled-goose-game-soundtrack-making-debussy-dynamic/), [UC Press – Journal of Sound and Music in Games](https://online.ucpress.edu/jsmg/article/2/1/1/115922/Finding-Untitled-Goose-Game-s-Dynamic-Music-in-the))

음악적으로는 기존 드뷔시 곡에 **템포·맥박·음량·음역(register)을 변형**해 긴박함, 놀람, 움직임, 장난스러움의 정서를 주입했다. 이 사운드트랙은 2020년 3월 27일 정식 발매되었고(Decca/iam8bit 등), 바이닐 에디션은 더블 그루브(double groove)로 제작되어 바늘을 어디에 떨어뜨리느냐에 따라 다른 트랙이 재생되는 무작위성을 물리적으로 구현했다. Golding은 이 작업으로 2020년 호주 ARIA 어워드 '최우수 오리지널 사운드트랙' 후보에 올랐다.

게임의 또 다른 시그니처 사운드는 단연 거위의 **"꽥꽥(HONK)"** 소리다. 컨트롤러의 한 버튼만 누르면 언제든 울려 퍼지는 이 honk는 게임의 정체성 그 자체가 되었고, 후술할 밈 현상의 핵심 소재가 되었다.

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

### 거위가 할 수 있는 일 — 단출한 동사 목록

이 게임의 메카닉은 놀라울 정도로 단순하다. 거위가 할 수 있는 행동은 다음으로 제한된다.

- **꽥꽥거리기(Honk)** — 버튼 하나로 큰 소리를 낸다. 주민의 주의를 끌거나 놀라게 하는 데 쓴다.
- **부리로 물건 잡기/물기(Grab)** — 열쇠, 모자, 안경, 채소, 라디오 등 거의 모든 작은 물체를 물어 옮긴다.
- **고개 숙이기/웅크리기(Duck/Lower head)** — 키를 낮춰 은신하거나 좁은 틈으로 통과한다.
- **달리기(Run)** — 위기 상황에서 빠르게 도주한다.
- **날갯짓(Flap wings)** — 위협하거나 시선을 끄는 동작.
- **뒤뚱뒤뚱 걷기(Waddle)** — 기본 이동.

이 여섯 가지 남짓한 '동사'의 조합만으로 게임의 모든 퍼즐이 설계된다. 개발진은 이 단순함을 의도적으로 추구했다.

### 코어 게임플레이 루프: To-Do List

게임의 진행 구조는 **'할 일 목록(To-Do List)'**을 중심으로 돌아간다. 마을은 여러 구역(정원 → 번화가/잡화점 → 펍 → 노부부의 뒷마당 → 모형 마을 광장 등)으로 나뉘며, 각 구역마다 클립보드에 적힌 듯한 체크리스트 형태의 목표가 주어진다. 예시는 다음과 같다.

- "정원사를 호수에 빠뜨리기(Make the gardener wear his sun hat / get the groundskeeper to wear his hat)"
- "피크닉 도시락 차려 먹기(Have a picnic)"
- "소년을 물에 빠뜨리기"
- "특정 물건(열쇠, 신발 한 짝 등)을 훔쳐 특정 장소에 갖다 놓기"

각 목표는 **무엇을(What)** 해야 하는지만 알려줄 뿐, **어떻게(How)** 달성할지는 전혀 알려주지 않는다. 플레이어는 환경과 NPC의 반응을 관찰하며 인과관계를 추론하고, 시행착오를 통해 해법을 발견한다. 충분한 수의 목표를 완수하면 다음 구역으로 넘어가는 문이 열린다. 목표 달성 순서는 비선형적이어서, 플레이어는 자기 페이스대로 마을을 휘젓고 다닐 수 있다.

이 구조는 개발진이 직접 밝혔듯 **Hitman 시리즈의 미션 구조**에서 영감을 얻은 것이다. 명확한 타깃과 목표가 있지만 접근 방식은 자유로운 '암살 의뢰' 구조를, 폭력을 제거하고 코미디로 치환한 것이다. House House의 Jake Strasser는 이렇게 설명했다.

> "It has a set-up and a punchline. By removing the violence from it, we just let the situations exist as a joke."
> ("(각 미션에는) 빌드업과 펀치라인이 있습니다. 거기서 폭력을 제거함으로써, 우리는 그 상황들이 그저 하나의 농담으로 존재하게 둔 거죠.")
> (출처: [Game Developer / Wikipedia](https://en.wikipedia.org/wiki/Untitled_Goose_Game))

### 스텔스의 전복: 취약하면서 동시에 무적인 존재

이 게임은 전통적인 스텔스 장르의 문법을 비튼다. 개발 과정에서 NPC의 시야(field of view)를 제한하는 시스템을 도입한 뒤로 게임플레이가 본격적으로 스텔스 중심이 되었다. 그러나 그 결과물은 *Metal Gear*나 *Splinter Cell*과는 전혀 다른 감각을 준다.

- 거위는 인간과 **직접 싸울 수 없다.** 주민이 다가오면 물건을 빼앗기거나 구역 밖으로 쫓겨난다.
- 그러나 주민도 거위를 **영구히 막을 수 없다.** 죽음도, 게임 오버도 없다. 쫓겨나도 곧 되돌아올 수 있다.

이 '동시에 취약하고 무적인' 설정은 독특한 리듬을 만들어낸다. 성공의 열쇠는 어둠 속에 숨는 전통적 은신이 아니라 **주의 분산(distraction), 방향 오도(misdirection), 그리고 완벽한 타이밍**이다. 거위는 honk로 NPC를 한쪽으로 유인하고, 그 틈에 반대편에서 목표물을 가로채며, 들켜서 쫓기더라도 도망쳐 다음 기회를 노린다. 즉, 처벌 없는 시행착오를 무한히 반복할 수 있는 안전한 놀이터(playground)가 게임 전체의 설계 철학이다.

### 진행 구조와 엔드게임

본편을 클리어하면 마을 전체를 무대로 한 **추가 도전 과제 목록(보너스 To-Do List)**이 해금된다. 예컨대 "단 일정 시간 내에 모든 구역을 거쳐 황금 종을 훔쳐 자기 둥지로 가져오기" 같은 고난도·스피드런성 목표들이다. 이는 짧은 본편의 리플레이성을 보강하기 위한 장치다.

### UI/UX 디자인 철학

UI는 극도로 미니멀하다. 화면 한구석에 클립보드 형태의 To-Do List가 떠 있고, 달성한 항목에는 손글씨로 줄이 그어진다. 별도의 튜토리얼 텍스트나 퀘스트 마커는 거의 없으며, 플레이어가 직접 만져보고 발견하도록 유도한다. 컨트롤은 버튼 하나에 한 가지 행동을 매핑한 직관적 구성으로, 누구나 몇 초 만에 익힐 수 있다. 이 '쉬운 진입, 깊은 발견'의 설계가 광범위한 대중성에 결정적으로 기여했다.

### 멀티플레이어 (2020년 협력 업데이트)

발매 약 1년 뒤인 **2020년 9월 23일**, House House는 모든 플랫폼에 **무료 2인 로컬 협동(co-op) 업데이트**를 배포했다. 동시에 이 게임은 처음으로 Steam과 itch.io에도 출시되었다. 핵심 내용은 다음과 같다.

- 두 명의 플레이어가 한 화면(local multiplayer)에서 각각 한 마리의 거위를 조종해 본편 전체를 함께 플레이한다.
- 두 번째 거위는 부리·발이 더 분홍빛이고 부리 밑동에 혹(basal knob)이 있어 외형이 구분된다.
- 사운드 디자이너가 두 번째 거위에게 **별개의 honk 소리**를 부여했다.
- 협동 전용 상호작용이 추가됐다. 예: 두 거위가 갈퀴(rake)를 림보 막대처럼 함께 들기, 한 거위가 다른 거위를 상자에 담아 끌고 다니기, 각자 워키토키를 들고 서로에게 honk를 송신하기.

PlayStation 공식 블로그에 게재된 개발기에서 House House는 협동 모드 추가가 단순한 인원 복제가 아니라, 두 거위가 만들어내는 **혼돈의 시너지(chaos)**를 어떻게 자연스럽게 녹여낼지에 대한 고민이었다고 밝혔다. (출처: [PlayStation Blog](https://blog.playstation.com/2020/09/22/how-house-house-added-multiplayer-to-untitled-goose-game/), [Game Informer](https://gameinformer.com/indie-world/2020/08/18/two-player-co-op-comes-to-untitled-goose-game-next-month))

### 라이브 운영 / MTX 부재

이 게임에는 시즌 패스, 마이크로트랜잭션(MTX), 라이브 서비스 요소가 **전혀 없다.** 단발성 패키지 게임으로, 2020년 협동 업데이트가 유일한 주요 콘텐츠 추가였다. 이는 당시 만연하던 라이브 서비스/과금 모델과 정반대의 행보로, 게임이 받은 호평의 한 축이기도 했다.

---

## 4. 평가

### Metacritic / OpenCritic 점수

플랫폼별 Metacritic 점수는 다음과 같으며, 전반적으로 "대체로 호의적(generally favorable)" 평가에 해당한다.

| 플랫폼 | Metacritic 점수 |
|---|---|
| Nintendo Switch | 81 / 100 |
| Xbox One | 81 / 100 |
| PlayStation 4 | 80 / 100 |
| PC (Windows) | 79 / 100 |

OpenCritic 기준으로는 비평가의 **약 82%가 이 게임을 추천(Recommended)**했다. (출처: [Metacritic](https://www.metacritic.com/game/untitled-goose-game/), [OpenCritic](https://opencritic.com/game/8308/untitled-goose-game))

### 주요 평론 인용

**IGN (8/10)** — "brief but endlessly charming adventure that had me laughing"
("짧지만 끝없이 사랑스러운 모험으로, 나를 계속 웃게 만들었다")

**GameSpot (8/10, 리뷰 제목 "Saved By The Bell")** — 게임의 사운드트랙이 자아내는 소극(farce)의 감각을 두고 "버스터 키튼(Buster Keaton) 영화를 연상시킨다(reminiscent of a Buster Keaton film)"고 평했다. 무성영화적 코미디의 리듬을 음악이 완성한다는 평이다. (출처: [GameSpot](https://www.gamespot.com/reviews/untitled-goose-game-review-saved-by-the-bell/1900-6417308/))

**Game Informer (7.5/10)** — 게임의 엉뚱함(silliness)을 칭찬하면서도, **반복적이고 너무 짧다(repetitive and too short)**고 지적했다. (출처: [Game Informer](https://gameinformer.com/review/untitled-goose-game/untitled-goose-game-review-the-joys-of-goosing-around))

**Destructoid (8.5/10)** — 영국 클레이메이션 시리즈 *Shaun the Sheep(숀더쉽)*에 빗대 호평했다.

**Eurogamer** — 점수제 대신 "Recommended(추천)" 등급을 부여했다.

**Polygon** — 점수를 매기지 않았으나 게임의 매력과 유머를 호의적으로 다뤘다.

전반적으로 비평계는 **유머, 절제된 디자인, 반응형 음악, 발견의 즐거움**을 일관되게 칭찬했고, 비판은 거의 전적으로 **짧은 분량과 후반부 반복성**에 집중되었다.

### 수상 이력 — 인디 게임의 대관식

*Untitled Goose Game*의 수상 기록은 인디 게임으로서 비범한 수준이다.

| 시상식 | 결과 | 비고 |
|---|---|---|
| **D.I.C.E. Awards 2020 (제23회)** | **Game of the Year (올해의 게임) 수상** | *Control*, *Death Stranding* 등을 제침. 2020년 2월 13일 |
| D.I.C.E. Awards 2020 | Outstanding Achievement for an Independent Game 수상 | 최우수 인디 게임 |
| D.I.C.E. Awards 2020 | Outstanding Achievement in Character 수상 | 캐릭터상 — 수상자는 '거위(The Goose)' |
| **GDC Awards 2020 (Game Developers Choice)** | **Game of the Year (올해의 게임) 수상** | 동료 개발자 투표 기반 최고 영예 |
| **BAFTA Games Awards 2020** | **Family (가족) 부문 수상** | 4개 부문 후보 (Audio Achievement, Family, Best Game 등) |
| Golden Joystick Awards 2019 | **Breakthrough Award (House House) 수상** | Ultimate Game of the Year 후보에도 노미네이트 |
| The Game Awards 2019 | Best Independent Game 후보 | 노미네이트 |

특히 D.I.C.E.와 GDC라는, 게임 업계가 가장 권위를 인정하는 두 시상식에서 동시에 '올해의 게임'을 수상한 것은, 2019년이 *Death Stranding*, *Control*, *Sekiro*, *Resident Evil 2 리메이크* 등 화제작이 즐비했던 해였음을 감안하면 더욱 이례적이다. (출처: [PlayStation Lifestyle](https://www.playstationlifestyle.net/2020/02/14/dice-2020-awards-untitled-goose-game-game-of-the-year/), [BAFTA](https://www.bafta.org/media-centre/press-releases/winners-announced-british-academy-games-awards-2020/), [GamesRadar](https://www.gamesradar.com/uk/untitled-goose-game-breakthrough-golden-joystick-2019/))

### 상업 지표

- 발매 후 **2주 만에 Nintendo Switch에서만 10만 장 이상** 판매. (출처: Wikipedia 집계)
- 호주, 영국, 미국 Nintendo Switch 차트에서 **1위** 등극.
- **2019년 말까지 전 플랫폼 합산 100만 장 이상** 판매 — 즉 발매 약 3개월 만에 밀리언셀러 달성. (출처: [MCV/DEVELOP](https://mcvuk.com/business-news/untitled-goose-game-tops-one-million-sales-in-just-3-months/), [TweakTown](https://www.tweaktown.com/news/69550/strange-awesome-untitled-goose-game-sold-1-million-units/index.html))

4인 스튜디오가 만든 인디 게임이 분기 만에 100만 장을 돌파한 것은, 당시 인디 시장에서도 손에 꼽히는 성과였다.

### 유저 평가

Metacritic 유저 스코어와 Steam 평가 모두 대체로 긍정적이었으나, 일부 유저층에서는 **가격 대비 짧은 분량**에 대한 불만이 비평계보다 더 강하게 표출되었다. ResetEra와 NeoGAF의 리뷰 스레드에서는 "It's very good(정말 좋다)"는 전반적 합의 속에서도 분량 논쟁이 반복적으로 등장했다. 그러나 게임이 자아낸 압도적인 호감과 밈 문화는 이런 불만을 상당 부분 상쇄했다.

### 평론–유저 괴리

평론과 유저 평가 사이의 큰 간극은 없었다. 양쪽 모두 "매력적이지만 짧다"는 핵심 평가에서 일치했다. 다만 **이 게임의 진짜 평가는 점수표가 아니라 인터넷 밈과 문화적 침투력에서 드러났다**는 점이 특이하다. 80점대 초반이라는 비교적 평범한 메타스코어에 비해, 게임의 문화적 영향력은 그해 어떤 90점대 대작보다도 컸다.

---

## 5. 성공 요인 분석 (핵심)

### (1) 기원 — Slack의 농담 한 줄에서 시작된 게임

이 게임의 탄생 설화는 그 자체로 전설이 되었다. **2016년 8월, Stuart Gillespie-Cook이 House House의 사내 Slack에 거위 스톡 사진 한 장을 올리며 농담조로 "우리 이걸로 게임 하나 만들자(we should make a game about this)"고 적은 것**이 시작이었다. 팀원들은 "왜 거위가 웃긴가"를 두고 농담을 주고받았고, 한 명이 이를 트윗한 뒤 한동안 잊혔다. 그러다 어느 시점에 그 Slack 대화를 다시 꺼내 진지하게 발전시키면서 실제 프로젝트가 되었다. (출처: [Wikipedia](https://en.wikipedia.org/wiki/Untitled_Goose_Game), [Vice – Honks vs. Quacks](https://www.vice.com/en/article/honks-vs-quacks-a-long-chat-with-the-developers-of-untitled-goose-game/))

영감의 원천은 명확했다. **3D 이동의 질감은 *Super Mario 64*, 미션 구조는 *Hitman* 시리즈.** 두 거대 프랜차이즈에서 핵심을 추출해 폭력을 제거하고 코미디로 재조립한 것이 이 게임의 설계도였다. (참고로 개발 중 검토된 대체 제목 중에는 *Some Like it Honk*도 있었다.)

### (2) 2017년 바이럴 트레일러 — 발매 2년 전에 이미 스타가 되다

성공의 결정적 변곡점은 **2017년 10월 4일 공개된 90초짜리 프리알파 트레일러**였다. 이 짧은 영상은 **공개 첫 주에만 트위터에서 200만 회 이상**의 조회수를 기록하며 바이럴이 되었다. 아직 게임이 완성되지도 않은 시점에 컨셉만으로 인터넷을 강타한 것이다.

이 트레일러의 폭발적 반응은 House House에게 "우리가 뭔가 대중적인 컨셉을 쥐고 있다"는 확신을 주었고, 결과적으로 게임을 완전한 프로젝트로 발전시키고 Panic과의 퍼블리싱 계약으로 이어지는 동력이 되었다. 즉 이 게임은 **발매되기 한참 전부터 마케팅이 사실상 완료된** 희귀한 사례다. 발매 전 2년간 쌓인 기대감과 인지도가 발매와 동시에 폭발했다. (출처: [Know Your Meme](https://knowyourmeme.com/memes/subcultures/untitled-goose-game), [Wikipedia](https://en.wikipedia.org/wiki/Untitled_Goose_Game))

### (3) 밈으로서의 완벽한 설계 — 인터넷 바이럴 마케팅 효과

이 게임은 의도했든 아니든 **밈으로 변환되기에 최적화된** 구조를 갖고 있었다. 발매 직후 인터넷은 *Untitled Goose Game* 밈으로 도배되다시피 했다.

- *PC Gamer*는 "인터넷이 엄청난 양의 거위 게임 밈과 팬아트를 honk해냈다(The internet has honked out a ton of Untitled Goose Game memes and art)"고 보도했다. (출처: [PC Gamer](https://www.pcgamer.com/the-internet-has-honked-out-a-ton-of-untitled-goose-game-memes-and-art/))
- *Slate*은 "거위 게임 밈이 모든 것이자 모든 곳에 있다(memes are everything and everywhere)"고 표현했다. (출처: [Slate](https://slate.com/technology/2019/10/untitled-goose-game-memes-are-about-everything-honk-honk.html))

밈으로서의 강력함은 **"끔찍한 거위"라는 공식의 무한한 확장성**에서 나왔다. 이 컨셉은 *어벤져스*, *Persona 5*, *Dark Souls*, *Pokémon* 등 어떤 다른 세계관에도 그대로 이식되어 농담으로 성립했다. "당신은 끔찍한 X입니다" 포맷, 그리고 "the goose game"이라는 별명으로 입소문이 퍼지면서, 게임을 모르던 사람조차 "그 거위 게임 어떻게 사?"라고 묻는 단계에 이르렀다.

셀럽 효과도 컸다. 모델 **Chrissy Teigen**은 우연히 이 게임을 발견해 남편인 가수 John Legend에게 사 달라고 했고, *Twin Peaks*의 배우 Kyle MacLachlan, 밴드 Blink-182 등이 게임을 언급하며 화제성이 주류 문화로 번졌다. *Inverse*의 표현대로, 이 게임은 그해 출시된 어떤 AAA 타이틀과도 비교할 수 없는 트위터·레딧 밈 폭풍을 일으켰다. (출처: [Inverse](https://www.inverse.com/article/59521-untitled-goose-game-memes-reddit-twitter-reviews), [Daily Dot](https://www.dailydot.com/memes/untitled-goose-game-memes/))

이것은 사실상 **제로(0)에 수렴하는 광고비로 달성한 바이럴 마케팅의 교과서**다. 4인 스튜디오에는 대규모 마케팅 예산이 없었지만, 게임의 컨셉 자체가 광고였고, 유저들이 자발적으로 만든 밈이 무한 증식하는 무료 광고망이 되었다.

### (4) 디자인 측면의 성공 요인

- **즉각적 이해 가능성**: "당신은 끔찍한 거위"라는 한 줄로 게임 전체가 설명된다. 진입 장벽이 사실상 0이다.
- **처벌 없는 놀이터**: 죽음·실패가 없어 누구나 부담 없이 즐긴다. 이는 게이머와 비게이머 모두를 포용했다.
- **나쁜 짓의 쾌감**: 일상 속 소소한 무정부적 말썽을 결과 없이 저지르는 해방감.
- **무성영화적 코미디 + 반응형 드뷔시 음악**: 비주얼, 상황, 사운드가 삼위일체로 코미디 타이밍을 완성했다.

### (5) 타이밍과 시장 환경

2019년은 거대 라이브 서비스 게임과 무거운 시네마틱 대작이 시장을 지배하던 해였다. 그런 피로감 속에서 **짧고, 가볍고, 순수하게 즐거운** 게임에 대한 갈증이 있었고, *Untitled Goose Game*은 그 빈자리를 정확히 채웠다. Nintendo Switch라는 캐주얼·휴대 친화적 플랫폼과의 궁합도 완벽했다.

### (6) 동시기 작품 대비 차별점

같은 시기 *Death Stranding*과 *Control*이 진지함과 작가주의로 무장했다면, *Untitled Goose Game*은 정반대 방향에서 — 순수한 유머와 미니멀리즘으로 — 승부했다. D.I.C.E.에서 바로 그 두 작품을 제치고 GOTY를 받은 것은, 게임이 "재미"라는 가장 본질적인 가치를 가장 순수하게 구현했음을 업계가 인정한 사건이었다.

---

## 6. 비평적 시각 / 한계 / 논란

### (1) 짧은 플레이타임 논쟁 — 가장 큰 쟁점

이 게임을 둘러싼 거의 유일하면서도 가장 격렬한 논쟁은 **분량**이다.

- 본편 클리어 시간은 **약 2시간** 내외로 평가된다. 일부 리뷰는 "3~4일 저녁이면 끝나는 게임(a game for 3-4 evenings)"이라 표현했다.
- *Game Informer*(7.5/10)는 명시적으로 "반복적이고 너무 짧다"고 지적했다.
- 다수 비평가가 "유일한 단점은 너무 짧다는 것"이라거나, "몇 개 길목을 둘러보고 나면 재미가 너무 빨리 끝난다"고 평했다.
- 일부는 가격표(약 USD 19.99) 대비 분량이 부족하다고 보았다.

후반부 **반복성** 문제도 함께 지적되었다. 짧은 분량임에도 "물건을 훔치고, 옮기고, 주민에게 쫓기는" 패턴이 일정 횟수 이상 반복되면 신선함이 떨어진다는 것이다.

반론도 만만치 않았다. "짧기 때문에 오히려 경험이 닳지 않는다(short length keeps the experience from wearing thin)", "짧지만 더없이 만족스러운 슬랩스틱 여정"이라는 옹호론이다. 이 논쟁은 결국 **'게임의 가치는 길이로 측정되는가'**라는 더 큰 질문으로 이어졌고, *Untitled Goose Game*은 그 논의의 대표 사례가 되었다. (출처: [Game Informer](https://gameinformer.com/review/untitled-goose-game/untitled-goose-game-review-the-joys-of-goosing-around), [GameSpot](https://www.gamespot.com/reviews/untitled-goose-game-review-saved-by-the-bell/1900-6417308/), Metacritic 종합)

### (2) 디자인적 약점

- **퍼즐 해법의 협소함**: 각 목표의 해법이 대체로 하나로 수렴해, *Hitman*류의 다채로운 자유도까지는 도달하지 못했다는 평.
- **콘텐츠 부족**: 협동 업데이트 이전까지는 본편과 보너스 목록 외에 추가 콘텐츠가 없었다.
- **반응형 음악의 그림자**: 음악 시스템은 혁신적이지만, 짧은 분량 탓에 드뷔시 곡 레퍼토리가 제한적이라 장시간 플레이 시 반복감이 생길 수 있다.

### (3) 운영/논란 이슈

심각한 운영 논란이나 출시 사고는 없었다. 다만 게임의 폭발적 화제성에 비해 **메타스코어(80점대 초반)가 상대적으로 평범했다**는 점은, 평가의 척도가 점수표만으로는 이 게임의 문화적 무게를 담아내지 못한다는 흥미로운 사례를 남겼다.

### (4) 평가가 갈리는 지점

핵심은 **"무엇이 게임의 가치를 정의하는가"**다. 분량·도전성·플레이타임 가성비를 중시하는 관점에서는 다소 박하고, 발견의 즐거움·코미디·문화적 임팩트를 중시하는 관점에서는 그해 최고의 게임 중 하나였다. 같은 게임을 두고 "과대평가된 짧은 미니게임"과 "올해의 게임"이라는 정반대 평가가 공존한 것이다.

(참고: 게임 자체에 인종·정치적 논란은 확인되지 않았다. "끔찍한 거위" 이미지가 일부 인터넷 밈에서 무정부적·반항적 상징으로 차용된 사례는 있으나, 이는 게임 텍스트 내부의 논란이 아니라 외부 밈 문화의 자발적 전용에 해당한다.)

---

## 7. 영향과 유산

### (1) 장르·산업적 영향

*Untitled Goose Game*은 **'동물 시점의 비폭력 샌드박스 코미디'**라는 하위 장르의 가능성을 대중에게 각인시켰다. 이후 동물·생물을 주인공으로 한 작은 인디 코미디 게임들에 직간접적 영감을 주었다는 평가를 받는다. 또한 "짧고 완결된 인디 게임이 AAA 대작을 제치고 GOTY를 받을 수 있다"는 선례를 만들어, 인디 개발자들에게 강력한 동기를 부여했다.

### (2) 호주 게임 산업과 제도적 의미

이 게임의 성공은 **호주 게임 산업의 위상**을 끌어올린 사건으로 평가된다. Film Victoria의 지원을 받은 4인 스튜디오가 세계적 성공을 거두자, 이는 호주 정부가 **디지털 게임 세금 공제(Digital Games Tax Offset, 2023년 도입)** 정책을 추진하는 데 상징적 사례로 인용되었다.[추정: 직접 인과 입증보다는 대표 성공 사례로 거론되는 맥락] House House는 또한 수익의 1%를 호주 원주민(Indigenous Australian) 단체에 기부하는 정책을 밝힌 바 있다. (출처: [Wikipedia](https://en.wikipedia.org/wiki/Untitled_Goose_Game))

### (3) 문화적 의미 — 게임이 밈을 넘어 문화 아이콘으로

- **밈·문화 아이콘화**: honk 소리와 "끔찍한 거위"는 2019년을 대표하는 인터넷 밈으로 자리 잡았고, 팬아트·시·굿즈로 무한 증식했다. *Know Your Meme*에 별도 항목으로 등재되었다.
- ***Untitled Goose Game Live* (2022년 6월)**: 호주의 ACMI(스크린 문화 박물관)와 Orchestra Victoria가 협업해, 게임 플레이에 맞춰 드뷔시 기반 사운드트랙을 실시간 오케스트라로 연주하는 라이브 공연이 열렸다. 비디오 게임 음악의 라이브 즉흥성을 무대화한 독특한 시도였다.
- **박물관 전시 (2024년)**: PAX Aus 2024 기간 동안 ACMI에서 게임의 성공, 문화적 영향, 디자인, 호주적 뿌리를 조명하는 전시가 열렸다. 게임이 단순 상품을 넘어 **보존·연구할 문화 유산**으로 인정받은 것이다. (출처: [Video Games Industry Memo](https://www.videogamesindustrymemo.com/p/honk-inside-the-untitled-goose-game), [ACMI](https://www.acmi.net.au/about/media/media-releases/australian-cultural-institutions-unite-to-collect-videogames/))

### (4) 후속작·확장

별도의 정식 후속작은 발표되지 않았으나, 2020년 무료 협동 업데이트가 게임의 생명력을 연장했다. House House는 이후 신작 개발을 이어가고 있다.[추정: 구체적 신작 정보는 본 조사에서 미확정]

### (5) 한 줄 요약

*Untitled Goose Game*은 "작고, 짧고, 단순하지만 완벽하게 즐거운" 게임이 어떻게 한 해의 게임 문화 전체를 점령하고 업계 최고 영예까지 거머쥘 수 있는지를 보여준 **인디 게임의 모범 사례이자 인터넷 시대 바이럴 마케팅의 교과서**다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 수치 / 내용 | 출처 |
|---|---|---|
| 개발 인력 | 핵심 4인 + 외부 작곡가 1인 | Wikipedia |
| 엔진 | Unity | Wikipedia |
| 최초 발매 | 2019.09.20 (Switch/macOS/Win) | Wikipedia |
| 콘솔 확장 | 2019.12.17 (PS4/Xbox One) | Wikipedia |
| Steam/itch.io + 협동 업데이트 | 2020.09.23 | PlayStation Blog |
| Switch Metacritic | 81/100 | Metacritic |
| OpenCritic 추천율 | 약 82% | OpenCritic |
| 본편 플레이타임 | 약 2시간 | 다수 리뷰 종합 |
| Switch 2주 판매 | 10만 장 이상 | Wikipedia |
| 누적 판매 | 100만 장 이상 (2019년 말, 발매 3개월) | MCV/DEVELOP |
| 2017 트레일러 조회수 | 첫 주 트위터 200만+ | Know Your Meme |
| 음악 스템 수 | 곡당 약 196~425개 (1~3초 단위) | ZoneOut / UC Press |
| 주요 수상 | D.I.C.E. GOTY, GDC GOTY, BAFTA Family, Golden Joystick Breakthrough | 각 시상식 |

### 음악 시스템 요약

- 원곡: 클로드 드뷔시 《전주곡집(Préludes)》 중 6곡 발췌
- 편곡/큐레이션: Dan Golding
- 방식: 각 곡을 일반/저에너지 두 버전으로 녹음 → 수백 개의 1~3초 스템으로 분해 → 플레이어 행동에 따라 실시간 조합 재생
- 효과: 무성영화 시대 즉흥 반주 피아니스트를 시뮬레이션 / 첫 곡만으로도 0이 52개 붙은 경우의 수
- 발매: 2020.03.27 사운드트랙 정식 발매, 바이닐은 더블 그루브로 무작위 재생 구현
- Dan Golding, 2020 ARIA 어워드 최우수 오리지널 사운드트랙 후보

### 주요 인터뷰 / 자료

- Game Developer (Gamasutra), "Getting goosey with Debussy: Creating an adaptive score for Untitled Goose Game" — 사운드 시스템 상세
  https://www.gamedeveloper.com/audio/getting-goosey-with-debussy-creating-an-adaptive-score-for-i-untitled-goose-game-i-
- Game Developer, "Road to the IGF: House House's Untitled Goose Game" — 개발사/IGF 인터뷰
  https://www.gamedeveloper.com/game-platforms/road-to-the-igf-house-house-s-i-untitled-goose-game-i-
- Vice, "Honks vs. Quacks: A Long Chat With the Developers of 'Untitled Goose Game'" — 기원·디자인 철학 심층 인터뷰
  https://www.vice.com/en/article/honks-vs-quacks-a-long-chat-with-the-developers-of-untitled-goose-game/
- PlayStation Blog, "How House House added multiplayer to Untitled Goose Game" — 협동 업데이트 개발기
  https://blog.playstation.com/2020/09/22/how-house-house-added-multiplayer-to-untitled-goose-game/
- UC Press, Journal of Sound and Music in Games, "Finding Untitled Goose Game's Dynamic Music in the World of Silent Cinema" — 학술 분석
  https://online.ucpress.edu/jsmg/article/2/1/1/115922/

### 참고 자료 목록 (영어권 매체 중심)

- Wikipedia – Untitled Goose Game / House House
- Metacritic / OpenCritic – 평론 종합
- IGN, GameSpot, Game Informer, Eurogamer, Destructoid – 개별 리뷰
- PC Gamer, Slate, Inverse, Daily Dot, BuzzFeed, Uproxx, iMore – 밈/바이럴 보도
- Know Your Meme – 밈 현상 아카이브
- MCV/DEVELOP, TweakTown – 판매 지표
- PlayStation Lifestyle, BAFTA, GamesRadar, GameRant, ScreenRant – 수상 보도
- ZoneOut, iam8bit, Discogs – 사운드트랙 자료
- ACMI, Video Games Industry Memo, Frieze, Portland Monthly – 문화적 영향/전시/퍼블리셔
- Vice, Game Developer (Gamasutra) – 개발자 인터뷰

---

*본 분석서는 2026년 5월 기준, 영어권 매체 및 공개 자료를 토대로 작성되었다. 판매량·점수·날짜는 인용 출처를 명시했으며, 직접 확인되지 않은 추론에는 [추정] 표기를 부기했다.*
