# NieR Replicant ver.1.22474487139... (2021) 심층 분석

> 11년 묵은 컬트 클래식을, 그 후예가 거둔 메가히트의 빛을 빌려 다시 빚어낸 작품. 《NieR Replicant ver.1.22474487139...》는 단순한 리마스터의 외피를 쓰고 있지만, 실은 한 작가주의 디렉터의 가장 사적인 이야기를 전 세계 관객 앞에 처음으로 정식 공개한 사건이었다.

---

## 1. 게임 개요

### 정식 명칭과 그 농담
이 게임의 정식 명칭은 《NieR Replicant ver.1.22474487139...》다. 끝에 붙은 길고 무의미해 보이는 숫자열은 요코 타로(Yoko Taro) 특유의 농담으로, √1.5(루트 1.5, 약 1.2247...)의 근사치다. 원작 《NieR Replicant》(2010)를 "버전 1.0"으로 본다면, 이 작품은 "완전한 2.0(리메이크)도, 단순 1.5(리마스터)도 아닌, 그 사이 어딘가"라는 자기규정을 숫자 장난으로 표현한 셈이다. 개발진 스스로도 이 작품을 "리마스터"나 "리메이크"가 아니라 **"버전 업그레이드(version upgrade)"**라고 불렀다.

### 개발사·퍼블리셔·출시
- **개발**: Toylogic + Square Enix 공동 개발. 원작 《NieR》(2010)를 만든 Cavia는 이미 해체되었기에, 신규 파트너로 Toylogic이 합류했다.
- **퍼블리셔**: Square Enix.
- **출시일**: 일본 2021년 4월 22일, 글로벌 4월 23일.
- **플랫폼**: PlayStation 4, Xbox One, PC(Steam). Xbox에서는 출시일에 Game Pass로 동시 제공.
- **발표**: 2020년 3월 29일, 시리즈 10주년 기념 "NieR 10시간 생방송"(NicoNico)에서 최초 공개. 즉 이 작품 자체가 시리즈 10주년 기념 프로젝트였다.

(출처: [Toylogic 공식](https://www.toylogic.com/news/news_details.php?dat=game-20210423), [PlayStation Blog 2020-09-24](https://blog.playstation.com/2020/09/24/nier-replicant-ver-1-22474487139-arrives-april-23-2021/), [Wikipedia: Nier](https://en.wikipedia.org/wiki/Nier))

### 주요 크레딧
- **크리에이티브 디렉터**: 요코 타로(Yoko Taro) — 시리즈의 작가주의 핵심.
- **게임 디렉터**: 사이토 사키(Saki Ito).
- **프로듀서**: 사이토 요스케(Yosuke Saito) — 《NieR》, 《NieR:Automata》, 《Drakengard》 시리즈를 관통하는 프로듀서.
- **작곡**: 오카베 케이이치(Keiichi Okabe)와 그의 스튜디오 MONACA.
- **액션 전투 자문**: PlatinumGames의 타우라 타카히사(Takahisa Taura). 그는 《NieR:Automata》의 게임 디자이너로, 이번 리메이크의 전투 손맛이 Automata 팬의 기대치에 부합하도록 자문했다.

### 엔진/기술 스택
원작은 PS3 세대에 머물러 있었기에, ver.1.22는 그래픽을 전면 재구축하여 60fps, 현세대 해상도, 개선된 모델·조명·이펙트를 구현했다. 다만 핵심 자산(레벨 디자인, 맵 구조)은 의도적으로 원작의 골격을 보존하는 방향을 택했다.

---

## 2. 게임 설명 — 이 게임이 무엇인가

### Gestalt와 Replicant — 11년의 사연 (가장 중요한 맥락)
이 게임을 이해하려면 먼저 원작의 두 갈래 출시 사정을 알아야 한다. 2010년, 《NieR》는 **두 가지 버전**으로 나왔다.

- **《NieR Gestalt》** — 서구(북미·유럽) 출시판. 주인공이 **딸 요나(Yonah)를 구하려는 중년 아버지**.
- **《NieR Replicant》** — 일본 출시판. 주인공이 **여동생 요나를 구하려는 형/청년**.

왜 갈랐는가? Square Enix 미국 지사가 "미국 시장에서는 아버지 캐릭터가 더 공감을 산다"고 조언했기 때문이다. 그 결과 서구 플레이어들은 11년간 "형 버전"인 Replicant를 정식으로 경험할 길이 없었다. 《NieR Replicant ver.1.22》는 바로 그 Replicant 버전을 **전 세계에 처음 정식 출시**한 작품이다. 요코 타로 본인은 한 인터뷰에서 "나는 Replicant 쪽 이야기를 더 선호한다"고 밝혔다 ([PCGamesN](https://www.pcgamesn.com/nier-replicant/ver-1-22474487139-interview-story-better)). 즉 이 리메이크는 디렉터가 가장 아끼는 원본을, 검열도 변형도 없이 세계 무대에 올린 의미를 가진다.

### 세계관과 줄거리 [스포일러 포함]
무대는 마법성 역병이 휩쓸고 간 머나먼 미래의 지구다. 인류는 멸종 위기에서 살아남기 위해 **Project Gestalt(프로젝트 게슈탈트)**라는 거대한 계획을 세웠다. 인간의 **영혼(Gestalt, 게슈탈트)**을 육체에서 분리해 보존하고, 한편으로 영혼 없는 인공 육체인 **Replicant(레플리칸트)**를 만들어, 훗날 둘을 재결합시켜 인류를 부활시킨다는 구상이었다.

그러나 계획은 어긋난다. Replicant들이 자아를 갖게 되면서, 자신들을 되찾으려 다가오는 Gestalt를 괴물로 인식해 **"Shade(그림자)"**라 부르며 적대했다. 영혼과 육체, 곧 원래는 하나였던 두 존재가 서로를 죽이는 비극이 펼쳐진다.

[스포일러] 플레이어가 조작하는 주인공 **Nier(니어, 플레이어가 이름 지정 가능)**는 불치병 **흑문병(Black Scrawl)**에 걸린 여동생 **요나(Yonah)**를 구하기 위해, 말하는 마도서 **그리무아르 바이스(Grimoire Weiss)**와 함께 봉인된 마법 시구(Sealed Verses)를 찾아 세계를 떠돈다. 여정에서 그는 반(半)-Shade 검사 **카이네(Kainé)**, 그리고 자신을 바라보는 모든 것을 석화시키는 눈을 가진 소년 **에밀(Emil)**을 만난다.

이야기의 핵심 반전은 최종 보스 **그림자의 군주(Shadowlord)**의 정체에 있다. 그는 프롤로그에 등장했던 "원래의 니어"가 변한 **최초의 게슈탈트(Original Gestalt)**다. 그 또한 흑문병에 걸린 자신의 딸 요나(Gestalt)를 구하려 했던 한 명의 아버지였다. 모든 게슈탈트는 그에게 연결되어 안정화되어 있다. 결국 플레이어가 적으로 싸우는 존재와 플레이어 자신은 **똑같이 "요나를 구하려는 가족"**이라는, 시점에 따라 선악이 뒤집히는 잔혹한 거울 구조가 드러난다.

### 다회차 엔딩 구조
《NieR》 시리즈의 상징인 다회차(NG+) 서사가 여기서도 핵심이다.
- **엔딩 A**: 1회차 클리어. 표면적 결말.
- **엔딩 B**: 2회차. 같은 사건을 Shade(그림자)들의 독백·시점을 곁들여 다시 보여주며, 적이었던 존재들에게도 사연이 있었음을 폭로한다.
- **엔딩 C / D**: 종반의 선택. 카이네를 살리기 위해 **니어 자신의 존재를 희생**할지 결정한다. **엔딩 D**에서 니어는 카이네를 구하려 자신을 세계에서 지워버린다 — 이때 **플레이어의 세이브 데이터가 실제로 삭제되고**, 게임 속 모두가 그를 잊는다. 게임 외부의 플레이어에게까지 상실을 체감시키는 요코 타로 특유의 메타 연출이다.
- **엔딩 E (리메이크 신규)**: 원작 당시 소설 형태로만 존재하던 후일담 "The Lost World"를 게임으로 구현했다. 엔딩 D로부터 3년 뒤, 카이네의 시점에서 진행되며, 사라진 니어를 되찾는 결말을 제시한다. 이 엔딩 E와 그에 딸린 신규 보스·에피소드가 ver.1.22의 가장 큰 신규 콘텐츠다.

(출처: [RPG Overload](https://rpgoverload.com/nier-replicant-full-plot-and-all-endings-explained/), [canmom.art](https://canmom.art/nier/nier-part-2), [Protagonist of Nier - Wikipedia](https://en.wikipedia.org/wiki/Protagonist_of_Nier), [GamingBolt: Ending E Explained](https://gamingbolt.com/nier-replicant-ver-1-22474487139-the-ending-explained))

### 무드·톤·아트 디렉션
《NieR》의 정서는 "아름다운 멜랑콜리"로 요약된다. 황량한 폐허, 텅 빈 마을, 끝없이 반복되는 일상 노동(낚시·농사) 사이로, 가족애와 상실, 폭력의 무게가 천천히 스며든다. 톤은 시종 무겁고 쓸쓸하지만, 사이사이 자조적 유머(말하는 책 바이스의 독설, 카이네의 거친 입담)가 균형을 잡는다. ver.1.22는 이 분위기를 현세대 그래픽으로 더 선명하게 끌어올렸다.

### 사운드와 음악
음악은 이 작품의 가장 강력한 무기다. (별도 섹션에서 상세히 다룬다.)

---

## 3. 핵심 시스템 / 메카닉

### 코어 루프와 장르 변주(Genre-Shifting)
《NieR Replicant》의 가장 독창적인 설계는 **하나의 게임 안에서 끊임없이 장르를 바꾸는 것**이다. 기본은 3인칭 액션 RPG이지만, 보스전이나 특정 구역에 들어서면 카메라가 바뀌며 게임 자체가 다른 장르로 변신한다.

- **탄막 슈팅(bullet hell)**: 보스전에서 적의 마법 공격이 화면을 가득 메우는 탄막으로 쏟아진다. 그리무아르(마도서)들이 쏘는 무수한 붉은 탄을 피하며 싸운다.
- **횡스크롤 플랫포머 / 탑다운 / 아이소메트릭**: 던전 구역마다 시점이 2D 횡스크롤, 위에서 내려다보는 탑다운, 비스듬한 아이소메트릭으로 전환된다.
- **텍스트 어드벤처**: 특정 가옥 내부 등에서는 화면이 텍스트 기반 어드벤처 게임으로 바뀐다.

이 장르 전환들은 단순한 기믹을 넘어, 게임이라는 매체 자체에 대한 메타적 오마주이자 패러디(데이비드 케이지식 연출, 레트로 게임 등)로 기능한다.

### 전투 메카닉 (리메이크의 최대 개선점)
원작의 전투는 투박하다는 평을 받았다. ver.1.22는 PlatinumGames 타우라 타카히사의 자문 아래 전투 손맛을 대폭 끌어올렸다.
- **콤보**: 경공격(light)과 중공격(heavy)을 섞어 콤보를 구성한다.
- **능동 회피·패링·스태거(신규)**: 리메이크에서 추가된 능동 회피(dodge)와 패링이 핵심이다. 타이밍을 맞춰 패링하면 적을 스태거(경직)시킬 수 있어, 전투가 훨씬 능동적이고 빨라졌다.
- **마법(Sealed Verses)**: 그리무아르 바이스의 봉인 시구가 마법 공격이다. 흑창(Dark Lance), 흑수(Dark Hand), 방패형 마법 등 다양하며, 보스전은 물리·마법·탄막 회피를 모두 섞어야 풀린다.

### 무기·강화·자원 경제
- **무기**: 편수검(one-handed), 양수검(two-handed), 창(spear) 세 계열을 수집하고 강화한다.
- **재화**: 골드로 더 좋은 무기를 사거나 강화 재료를 산다. 골드를 모으는 사실상 유일한 안정적 경로가 **사이드 퀘스트**라는 점이 후술할 비판의 한 축이 된다.
- **Word(말) 시스템**: 무기와 마법에 "단어(Word)"를 장착해 능력치 버프를 받는 독특한 시스템. 접두/접미 단어 조합으로 공격력·MP회복·상태이상 등을 커스터마이즈한다. 리메이크 신규 단어 "Ashurfarra"는 신규 에피소드 보스 "Louise" 격파 후 얻으며, MP 회복 가속과 HP 흡수를 동시에 부여한다.

### 부가 활동
낚시, 농사·정원 가꾸기, 채집, 보물찾기 등 평화로운 일상 활동이 풍부하다. 이는 종말 후 세계에서도 이어지는 "소박한 삶"의 정서를 강화하지만, 일부는 운(낚시 확률 등) 의존도가 높아 호불호가 갈린다.

### 세이브 시스템
세이브는 마을 등에 배치된 **우체통(Post Box)** 세이브 포인트에서만 정식으로 이뤄진다. 보스 직전이나 신규 구역 진입 시 체크포인트형 오토세이브가 작동하지만, 게임을 종료했다 다시 켜면 마지막 우체통 세이브 지점에서 로드된다. 즉 현대적 "아무 데서나 세이브"는 없고, 클래식한 세이브 포인트 구조를 유지했다.

### 리메이크 신규 콘텐츠 총정리
- **추가 에피소드 "Mermaid(인어)"**: Grimoire NieR 수록 소설을 기반으로 한 본편 신규 구간. 신규 스토리·캐릭터·적·보스("Louise")를 포함.
- **엔딩 E**: 위 서사 섹션 참조. 신규 보스("The Little Mermaid" 소설 기반)와 함께 제공.
- **최강 무기 Kaine's Sword**: 엔딩 E 해금 후 카이네의 오두막에서 입수. 풀강화 시 공격력 999, 마법력 100%로 게임 내 최강.
- **그래픽 전면 개선, 60fps, 신규 의상, UI 개선** 등.

(출처: [Game Informer](https://gameinformer.com/the-game-awards-2020/2020/12/10/take-a-look-at-some-flashy-nier-replicant-gameplay), [Slant Magazine](https://www.slantmagazine.com/games/nier-replicant-ver-1-22474487139-review/), [TheSixthAxis](https://www.thesixthaxis.com/2021/04/22/nier-replicant-review-remaster-ver-1-22474487139/), [SAMURAI GAMERS](https://samurai-gamers.com/nier-replicant-remaster-ver-122474487139/changes-in-ver-1-22474487139/))

---

## 4. 평가

### 평론 점수
- **Metacritic**: PS4 **83**(평론 97개, 유저 평점 8.3 / 988표), Xbox One **83**(평론 11개), PC **80**(평론 16개).
- **OpenCritic**: **83**, 상위 11% 게임, 비평가 **85% 추천**.

### 주요 개별 평론
| 매체 | 점수 | 비고 |
|------|------|------|
| GamingTrend | 100 | 만점 |
| IGN Japan | 90 | |
| Atomix | 90 | |
| PlayStation LifeStyle | 85 | |
| IGN (글로벌) | 80 (8/10) | |
| GameSpot | 80 (8/10) | |
| Game Informer | 83 | |
| GameSkinny | 80 | |
| VideoGamer | 60 | 회의적 |
| Eurogamer | (점수 없음) | "Okay, but not great"에 가까운 미온적 평 |

평론가들이 한목소리로 칭찬한 지점은 **스토리·캐릭터·사운드트랙·다회차 구조·엔딩의 충격**이었다. 특히 전투 손맛이 원작 대비 대폭 개선되어, "이제는 이야기를 즐기기 위해 전투를 견딜 필요가 없다"는 평이 많았다.

(출처: [Metacritic](https://www.metacritic.com/game/nier-replicant-ver122474487139/), [OpenCritic](https://opencritic.com/game/11154/nier-replicant-ver-1-22474487139), [ResetEra 리뷰 스레드](https://www.resetera.com/threads/nier-replicant-review-thread.413988/))

### 상업 지표
- **2021년 6월**: 전 세계 출하·디지털 합산 **100만 장 돌파**. 첫 주 10만 장 이상을 팔며 일본 차트에서 《Monster Hunter Rise》를 제쳤다.
- **2022년 12월**: **150만 장 돌파**.
- **2026년(최근)**: **200만 장 돌파**.

이는 일본 한정 컬트 타이틀이었던 원작과 비교하면 비약적 성공이다. 참고로 후속작 《NieR:Automata》는 2026년 2월 **누적 1,000만 장**을 돌파했다.

(출처: [Square Enix 보도자료](https://press.na.square-enix.com/SHIPMENTS-AND-DIGITAL-SALES-FOR-CRITICALLY-ACCLAIMED-NIER-REPLICANT-VE), [MP1st](https://mp1st.com/news/nier-replicant-ver-1-22-shipments-and-digital-sales-surpass-one-million-units), [RPG Site](https://www.rpgsite.net/news/19690-nier-replicant-remaster-sales-numbers-2-million-copies-2026), [Final Weapon](https://finalweapon.net/2026/02/20/nier-automata-sales-surpass-10-million-units-worldwide/))

### 평론-유저 괴리
유저 점수(PS4 8.3)는 평론 메타스코어(83)와 거의 일치한다. 다만 그 안에는 명확한 결이 있다. **스토리에 깊이 빠진 팬**은 만점에 가까운 평가를, **게임플레이 구조의 반복성을 못 견딘 신규 유저**는 박한 평가를 남기는 양극 분포가 관찰된다.

---

## 5. 성공 요인 분석

### (1) 역방향 후광 효과 — Automata가 끌어올린 원류
가장 결정적인 성공 요인은 **《NieR:Automata》(2017)의 메가히트**다. Automata는 출시 후 수년간 입소문으로 판매가 누적되며 시리즈를 컬트에서 메인스트림으로 끌어올렸다. 개발진은 인터뷰에서 "Automata가 (당시) 550만 장 넘게 팔렸으니, Replicant 새 버전을 내면 팔릴 것"이라고 판단했다고 밝혔다 ([Siliconera](https://www.siliconera.com/yoko-taro-and-yosuke-saito-on-nier-replicants-new-additions/)). 즉 후속작의 성공이 원작 리메이크의 시장을 만들어준, 흔치 않은 **역방향 후광 효과**다.

### (2) "원작을 처음 정식 출시"라는 희소성
서구 시장은 11년간 Replicant 버전을 정식으로 못 했다. Automata로 시리즈에 입문한 수백만 신규 팬에게, "이 모든 이야기의 시작점"을 처음 정식으로 즐길 기회는 그 자체로 강력한 구매 동기였다.

### (3) "보존과 현대화"의 영리한 균형
개발진은 원작의 정서와 레벨 구조를 보존하면서, 신규 팬이 가장 불편해할 **전투 손맛만 집중적으로 현대화**했다. Automata의 디자이너를 자문으로 영입해 "Automata에서 넘어온 플레이어가 위화감 없이 받아들일 전투"를 목표로 삼은 것은 정확한 타깃 설정이었다.

### (4) 신규 콘텐츠로 더블딥(재구매) 유도
완전 신규 엔딩 E, 추가 에피소드 Mermaid, 신규 보스·무기는 원작을 이미 한 코어 팬에게도 "다시 살 이유"를 제공했다.

### (5) 10주년 기념이라는 타이밍과 마케팅
시리즈 10주년 생방송에서 깜짝 발표하는 이벤트성 마케팅, 그리고 출시일 Xbox Game Pass 동시 제공으로 진입 장벽을 낮춘 점이 초기 도달률을 키웠다.

### 동시기 작품 대비 차별점
2021년에는 이미 현대화된 오픈월드·고예산 액션 RPG가 즐비했다. 그 속에서 《NieR Replicant》는 "세련된 게임플레이"로 경쟁하지 않았다. 대신 **작가주의 서사, 메타 연출, 음악**이라는, 다른 게임이 흉내 내기 어려운 정서적 자산으로 차별화했다.

---

## 6. 비평적 시각 / 한계 / 논란

### (1) 후반부의 반복성 — 가장 일관된 비판
거의 모든 리뷰가 지적한 약점은 **후반부의 반복적 사이드 퀘스트(fetch quest)와 백트래킹**이다. 같은 지역을 몇 번이고 오가게 만드는 구조, 단조로운 심부름 퀘스트, 그리고 무기 강화에 필요한 골드를 모으려면 결국 그 지루한 퀘스트를 반복해야 하는 경제 설계가 도마에 올랐다. 일부 평론은 "2010년 기준으로도 구식이던 구조가 그대로 남아 있다"고 평했다 ([Slant](https://www.slantmagazine.com/games/nier-replicant-ver-1-22474487139-review/), [WayTooManyGames](https://waytoomany.games/2021/05/06/review-nier-replicant-ver-1-22474487139/)).

### (2) "원작 보존"의 양날
전투는 현대화했지만 레벨 디자인·퀘스트 구조는 의도적으로 보존했다. 이 결정은 원작의 정체성을 지키는 한편, 신규 플레이어에게는 "왜 이건 안 고쳤나"라는 불만을 남겼다. 보존과 현대화 사이에서 그은 선이 모두를 만족시키지는 못했다.

### (3) Automata와의 비교 함정
일부 평론은 "Automata가 너무 뛰어나기 때문에, 그것을 먼저 경험한 플레이어에게 Replicant를 추천하기가 오히려 어렵다"는 역설을 지적했다. 시리즈의 정점이 그 뿌리를 가리는 모양새다.

### (4) 다회차 강제
진정한 결말(엔딩 C/D/E)에 도달하려면 같은 본편을 여러 번 돌아야 한다. 이 메타 서사는 시리즈의 매력이자, 시간이 부족한 플레이어에겐 진입장벽이다.

---

## 7. 영향과 유산

### 시리즈 정전(canon)의 완성
ver.1.22는 흩어져 있던 《NieR》 시리즈의 출발점을 전 세계에 정식·현대적 형태로 안착시켰다. Drakengard → NieR(Gestalt/Replicant) → Automata로 이어지는 요코 타로 유니버스의 "정사 입구"가 비로소 누구나 접근 가능한 형태로 정리된 것이다.

### 작가주의 게임 디자인의 재확인
세이브 데이터를 삭제하는 엔딩, 시점에 따라 선악이 뒤집히는 서사, 플레이어를 공범으로 만드는 메타 연출 — 요코 타로식 화법이 현세대 하드웨어에서도 유효함을 증명했다. 이는 후대 내러티브 디자이너들에게 "게임만이 할 수 있는 이야기 방식"의 교과서적 사례로 인용된다.

### 리메이크 방법론의 사례 연구
"무엇을 고치고 무엇을 남길 것인가"라는 리메이크의 근본 질문에서, ver.1.22는 **핵심 불만(전투)만 외과적으로 수술하고 정체성(서사·음악·구조)은 보존**하는 접근의 대표 사례로 자주 거론된다. 그 성공과 한계(반복성 미해결) 모두가 후속 리메이크 프로젝트의 참고점이 된다.

### 산업적·문화적 의미
한 번 상업적으로 실패에 가까웠던 작품이, 후속작의 성공과 팬덤의 헌신에 힘입어 10년 뒤 200만 장 IP로 재탄생한 서사 자체가 의미심장하다. "느린 성공(slow burn)"과 "장기 IP 가치"의 모범 사례이며, 컬트 타이틀이 메인스트림으로 승격하는 과정을 보여준다.

---

## 8. 부록

### 음악 상세 (작곡·재녹음)
- **작곡**: 오카베 케이이치(Keiichi Okabe)와 MONACA 팀.
- **보컬**: 에미 에반스(Emi Evans), 제이니크 니콜(J'Nique Nicole), 나카가와 나미(Nami Nakagawa). 기타: 고토 타카노리(Takanori Goto).
- **가사 언어**: 현실 언어가 아니라, 미래에 변형된 언어를 가정한 가상의 **"Chaos Language"**. 영어·일본어·게일어·이탈리아어 등을 합성·변형해 만든 인공어로, 특정 국가에 매이지 않는 보편적 애상을 자아낸다.
- **리메이크의 음악 갱신**: ver.1.22에서는 **모든 보컬과 합창을 재녹음**하고, 원작에서 기계로 만들었던 악기 파트를 **실연주로 교체**했다. 그 결과 "훨씬 풍부한" 사운드가 되었으며, 당초 "굳이 손댈 필요가 있나" 회의적이던 평론가들도 "Song of the Ancients", "Temple of Drifting Sands", "Dance of the Evanescent", "Grandma" 등의 재편곡이 원곡보다 낫다고 인정했다.
- **평가**: 게임 음악사상 최고의 사운드트랙 중 하나로 꾸준히 꼽힌다.

(출처: [Music of Nier - Wikipedia](https://en.wikipedia.org/wiki/Music_of_Nier), [RPGFan 음악 리뷰](https://www.rpgfan.com/music-review/nier-replicant-ver-1-22474487139-original-soundtrack/), [PlayStation Blog: Emi Evans 인터뷰](https://blog.playstation.com/2020/12/18/nier-replicant-singer-emi-evans-talks-music-chaos-language-and-more/), [NME: 오카베 인터뷰](https://www.nme.com/features/gaming-features/nier-composer-keiichi-okabe-i-always-conveyed-the-tragic-fates-that-the-protagonist-and-characters-are-burdened-with-2924765))

### 주요 인터뷰
- [PCGamesN — "I prefer the story in Replicant" (요코 타로/사이토 인터뷰)](https://www.pcgamesn.com/nier-replicant/ver-1-22474487139-interview-story-better)
- [Siliconera — Yoko Taro & Yosuke Saito on New Additions](https://www.siliconera.com/yoko-taro-and-yosuke-saito-on-nier-replicants-new-additions/)
- [NIER Wiki — Interview with the Creators (ver.1.22...)](https://nier.fandom.com/wiki/Interview_with_the_Creators_(ver.1.22...))
- [PlayStation Blog — Emi Evans on Chaos Language](https://blog.playstation.com/2020/12/18/nier-replicant-singer-emi-evans-talks-music-chaos-language-and-more/)

### 핵심 통계 표
| 항목 | 내용 |
|------|------|
| 정식명 | NieR Replicant ver.1.22474487139... (√1.5 농담) |
| 개발/퍼블리셔 | Toylogic + Square Enix / Square Enix |
| 크리에이티브 디렉터 | 요코 타로(Yoko Taro) |
| 게임 디렉터 | 사이토 사키(Saki Ito) |
| 프로듀서 | 사이토 요스케(Yosuke Saito) |
| 작곡 | 오카베 케이이치 / MONACA |
| 출시 | 2021-04-22(JP) / 04-23(글로벌) |
| 플랫폼 | PS4, Xbox One, PC(Steam), Game Pass 동시 |
| Metacritic | PS4 83 / Xbox One 83 / PC 80, 유저 8.3 |
| OpenCritic | 83, 비평가 85% 추천 |
| 판매량 | 100만(2021.6) → 150만(2022.12) → 200만(2026) |
| 핵심 신규 콘텐츠 | 엔딩 E, 추가 에피소드 Mermaid, 신규 보스/무기, 전투 현대화, 음악 재녹음 |

### 참고 자료 목록 (영어권 매체 중심)
- [Wikipedia: Nier](https://en.wikipedia.org/wiki/Nier)
- [Wikipedia: Music of Nier](https://en.wikipedia.org/wiki/Music_of_Nier)
- [Wikipedia: Protagonist of Nier](https://en.wikipedia.org/wiki/Protagonist_of_Nier)
- [Metacritic](https://www.metacritic.com/game/nier-replicant-ver122474487139/)
- [OpenCritic](https://opencritic.com/game/11154/nier-replicant-ver-1-22474487139)
- [PlayStation Blog: 출시 발표](https://blog.playstation.com/2020/09/24/nier-replicant-ver-1-22474487139-arrives-april-23-2021/)
- [Toylogic 공식](https://www.toylogic.com/news/news_details.php?dat=game-20210423)
- [Square Enix 보도자료: 100만 돌파](https://press.na.square-enix.com/SHIPMENTS-AND-DIGITAL-SALES-FOR-CRITICALLY-ACCLAIMED-NIER-REPLICANT-VE)
- [RPG Site: 200만 돌파](https://www.rpgsite.net/news/19690-nier-replicant-remaster-sales-numbers-2-million-copies-2026)
- [Slant Magazine 리뷰](https://www.slantmagazine.com/games/nier-replicant-ver-1-22474487139-review/)
- [TheSixthAxis 리뷰](https://www.thesixthaxis.com/2021/04/22/nier-replicant-review-remaster-ver-1-22474487139/)
- [RPGFan 음악 리뷰](https://www.rpgfan.com/music-review/nier-replicant-ver-1-22474487139-original-soundtrack/)
- [GamingBolt: 엔딩 E 해설](https://gamingbolt.com/nier-replicant-ver-1-22474487139-the-ending-explained)
- [RPG Overload: 전체 플롯/엔딩 해설](https://rpgoverload.com/nier-replicant-full-plot-and-all-endings-explained/)

---

*본 분석서는 영어권 매체·공식 인터뷰·판매 보도자료를 기반으로 작성되었다. 모든 판매 수치와 점수는 위 출처에 근거하며, 미확인 정보는 포함하지 않았다.*
