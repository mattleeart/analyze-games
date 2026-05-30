# The Legend of Zelda: Breath of the Wild (2017) — 오픈월드 공식을 재정의한 화학 엔진의 야생

> "A masterclass in open-world design."
> — Jose Otero, IGN 10/10 리뷰 (2017년 3월 2일)
>
> "The most impressive game Nintendo has ever created."
> — Peter Brown, GameSpot 10/10 리뷰

> 본 분석서는 2017년 3월 3일 Nintendo Switch / Wii U로 발매된 《The Legend of Zelda: Breath of the Wild》(이하 BotW)를 한 편의 장문 평론으로 정리한 것이다. 영어권 매체 리뷰, GDC 2017 "Change and Constant: Breaking Conventions with The Legend of Zelda: Breath of the Wild" 강연, Eiji Aonuma·Hidemaro Fujibayashi·Takuhiro Dohta·Satoru Takizawa의 공식 인터뷰, Wikipedia의 종합 데이터, Game Maker's Toolkit(Mark Brown)·Thumbsticks·Kotaku·Game Developer 등의 디자인 분석 글을 1차 소스로 삼았다. 인용 통계와 점수는 모두 공개된 자료에 근거하며, 추정치는 [추정]으로 명시한다.

---

## 1. 게임 개요

### 1-1. 한 줄 요약

《The Legend of Zelda: Breath of the Wild》는 1986년 패미컴 디스크 시스템판 《The Legend of Zelda》가 제시한 "지도 한 장을 손에 쥐고 어디로든 갈 수 있다"라는 원초적 자유의 약속을, 30년 만에 3D 오픈월드의 언어로 환원한 작품이다. 표면적으로는 시리즈 19번째 메인 타이틀이지만, 본질적으로는 닌텐도가 "Zelda series의 관습을 깨자(Rethinking the conventions of Zelda)"라는 슬로건 아래 2011년 《Skyward Sword》 발매 직후부터 약 5년에 걸쳐 진행한 거대한 디자인 리부트의 결과물이다. 발매 시점에 평론가들이 만점을 던지며 "오픈월드 장르의 기준점"이라 호명했고, 7년이 지난 지금도 이 호명은 거의 그대로 유효하다.

### 1-2. 기본 정보

| 항목 | 내용 |
| --- | --- |
| **개발사** | Nintendo Entertainment Planning & Development (EPD) — 구 Nintendo EAD가 2015년 재편된 조직. Zelda 팀이 그 안의 핵심 사업부. |
| **공동 개발 지원** | Monolith Soft 도쿄 제2제작부. Wikipedia 및 GamesRadar 보도 기준 약 50명 규모로 풍경/지형 디자인을 지원했고, Miyamoto가 E3 2016에서 "교토와 도쿄에서 합쳐 100명 이상이 도와주고 있다"고 발언. |
| **퍼블리셔** | Nintendo (전 세계). |
| **발매일** | 2017년 3월 3일 (Nintendo Switch 글로벌 런칭 타이틀 / Wii U 동시 발매. Wii U 입장에서는 Nintendo가 자체 퍼블리시한 마지막 작품이라는 상징성을 함께 가진다.) |
| **장르** | 액션 어드벤처, 오픈월드, 일부 서바이벌·샌드박스 요소. |
| **엔진** | Havok 기반의 자체 수정 물리 엔진 + 자체 개발 "Chemistry Engine". |
| **언어 지원** | 발매 시점 영어/일본어/프랑스어/독일어/스페인어/이탈리아어/네덜란드어/러시아어/중국어(번체·간체 사후 추가). |
| **개발 기간** | 약 4~5년 (2013~2017). Aonuma 본인이 인터뷰에서 "Skyward Sword가 끝난 직후부터 다음 Zelda를 구상하기 시작했다"고 밝힘. |
| **개발 인원** | 최대 약 300명 (Aonuma, 2017년 닌텐도 다이렉트 인터뷰 / Famitsu 보도 기준). 초기 코어 약 10명에서 시작해 후반부로 갈수록 늘어남. Monolith Soft 지원 인력 포함 시 사실상 400명대. |
| **예산** | 공식 미공개. ResetEra·GameFAQs 등의 추산은 300명 × 4년 × 평균 인건비 기반으로 1억 달러 내외를 거론하나 [추정]. |

### 1-3. 주요 크레딧

| 역할 | 인물 | 비고 |
| --- | --- | --- |
| 시리즈 프로듀서·총괄 | **Eiji Aonuma** (青沼英二) | 1998년 《Ocarina of Time》부터 사실상의 Zelda 시리즈 감수자. BotW에서는 프로듀서로 후방 지원. |
| 디렉터 | **Hidemaro Fujibayashi** (藤林秀麿) | 《The Minish Cap》, 《Phantom Hourglass》, 《Skyward Sword》의 디렉터. 시리즈 외부 출신(Capcom)에서 합류해 도쿄가 아닌 오사카 출신 특유의 "관습을 의심하는 시선"을 가져왔다는 평. |
| 기술 디렉터 | **Takuhiro Dohta** (堂田卓宏) | Chemistry Engine·물리 시스템 책임자. GDC 2017 강연 메인 발표자. |
| 아트 디렉터 | **Satoru Takizawa** (滝澤智) | 인상주의·일본 애니메이션 톤의 아트 방향 결정. |
| 메인 캐릭터 아티스트 | **Takumi Wada** (和田貴美) | 신생 Link·Zelda 디자인. |
| 시나리오 | **Akihito Toda**, **Naoki Mori** | "memory recall" 구조의 비선형 내러티브 책임. |
| 음악 | **Manaka Kataoka** (片岡真央), **Yasuaki Iwata** (岩田恭明), **Hajime Wakai** (若井秀和) | Kataoka가 리드 컴포저로 오픈 필드 음악·전투 테마 대부분을 작곡. |
| 사운드 디렉션 | Hajime Wakai (also Sound Director) | 환경음 우선·미니멀 피아노 모티프 디자인. |
| 시리즈 사운드 트랙 어드바이저 | Koji Kondo | 메인 테마 작곡 자문, 미공개 인터뷰에서 "젊은 작곡가들의 도전을 옆에서 본 작품"이라 언급. |

### 1-4. 발매 플랫폼·재발매 이력

- **2017.03.03** Nintendo Switch / Wii U 동시 발매. Switch는 글로벌 런칭 타이틀.
- **2017.06.30** DLC 1탄 "The Master Trials" 발매 (Trial of the Sword, Master Mode, Hero's Path 등 추가).
- **2017.12.07** DLC 2탄 "The Champions' Ballad" 발매 (One-Hit Obliterator 챌린지, 신규 던전 EX Trial of the Sword).
- **2025.06.05** Nintendo Switch 2 Edition. 4K/HDR/60fps 지원, Zelda Notes 모바일 연동 추가. Metacritic 94점.

---

## 2. 게임 설명 — 이 게임은 정확히 무엇인가

### 2-1. 컨셉과 슬로건

BotW의 캐치프레이즈는 "Step outside, and witness what awaits you"로, 발매 직전 2017년 닌텐도 다이렉트 트레일러에서 명시적으로 사용됐다. 그러나 개발팀 내부의 진짜 슬로건은 다른 것이었다. GDC 2017 강연에서 Fujibayashi는 단상 위에 한 줄을 띄웠다.

> "Rethink the conventions of Zelda." — Hidemaro Fujibayashi, GDC 2017 (한국어 의역: "Zelda의 관습을 재고하자.")

이 "Zelda의 관습"이란 무엇인가? Fujibayashi는 강연에서 다섯 가지를 짚었다. ① 정해진 순서로 던전을 클리어해야 한다. ② 벽은 넘을 수 없다. ③ 검은 검대로, 활은 활대로 분리된 도구다. ④ 스토리는 컷신으로 일방적으로 전달된다. ⑤ 플레이어는 "디자이너가 의도한 솔루션"을 찾는 것이 목적이다. BotW는 이 다섯 가지 모두를 의도적으로 부쉈다. 그 결과, 본질적으로 "30년 동안 만들어온 자신들의 안전망을 스스로 걷어차는" 행위가 됐고, 그 도전 자체가 작품의 의의가 됐다.

### 2-2. 세계관과 시간선

[전체 구간 스포일러] BotW는 시리즈 정사 연표(공식 가이드북 《Hyrule Historia》)에 따르면 "시간선이 통합된 먼 미래"에 위치한다. 정확한 위치는 닌텐도가 끝내 명시하지 않았으나, Aonuma는 "(시간선 논쟁에) 종지부를 찍지 않을 것"이라고 발언한 바 있다(2017, Famitsu). 핵심 설정은 다음과 같다.

- **만년 전**, 고대 시이카(Sheikah) 부족이 가논(Ganon)의 부활을 예지하고 4기의 "신수(Divine Beast)"와 무수히 많은 "가디언(Guardian)"이라는 자율 병기를 제작했다. 100년 전, 그것을 다시 발굴해 다가올 재앙에 대비했다.
- **100년 전**, 예언대로 가논이 부활했으나 가디언 군단이 그의 통제 하에 들어가며 하이랄 왕국은 멸망했다. 신수의 조종사였던 4명의 챔피언(Mipha·Daruk·Revali·Urbosa)은 신수 내부에서 전사했고, 왕은 사망, 링크는 빈사 상태로 회생의 사당(Shrine of Resurrection)에 잠들었으며, 젤다는 "신성한 힘(Sealing Power)"을 각성해 가논을 하이랄 성에 봉인했다.
- **현재**, 100년 만에 깨어난 링크에게는 기억이 없다. 빈 손에 시이카 슬레이트 하나만 주어진다. 100년 동안 가논을 홀로 막아온 젤다의 힘은 한계에 다다랐다. 링크는 잃어버린 기억을 찾고, 4기의 신수를 해방시키고, 마스터 소드를 회수하고, 최종적으로 하이랄 성에서 재앙의 가논(Calamity Ganon)을 격파해야 한다.

이 설정의 디자인적 함의가 중요하다. "튜토리얼은 100년의 동면 후 깨어나는 노년의 영웅"이라는 출발점은 "왜 플레이어가 모든 능력을 잃은 상태에서 시작하는가"라는 게임 디자인의 영원한 정당화 문제를, 내러티브 안에서 자연스럽게 해결한다. 또한 "이미 한 번 실패한 영웅"이라는 설정 덕분에, 플레이어가 약하다는 느낌·세계가 황량하다는 분위기가 서사적으로 정당화된다.

### 2-3. 주요 캐릭터

- **Link** — 100년 동안 잠들어 있던 하이랄 왕녀 친위 기사. 무성격에 가까운 침묵의 주인공이지만, BotW에서는 "기억" 컷신을 통해 100년 전의 인간적이고 다소 미숙했던 청년 링크가 단편적으로 묘사된다.
- **Princess Zelda** — 시리즈 통틀어 가장 입체적인 묘사를 받은 젤다. 신성한 힘이 발현되지 않아 아버지(왕)와 갈등을 빚는 학자 기질의 공주. 100년 동안 가논을 봉인하며 외친 마지막 대사 "Link... please save Hyrule"은 발매 직전 트레일러에서 사용되어 화제가 됐다.
- **King Rhoam** — 죽은 하이랄 왕. 위장한 노인의 모습으로 위대한 고원에서 링크에게 튜토리얼을 안내한다.
- **The Champions** — 4종족의 전사. Zora의 공주 **Mipha**(링크에게 연심을 품었던 인물), Goron 전사 **Daruk**, Rito 궁수 **Revali**(자존심 강한 라이벌), Gerudo 전사 **Urbosa**(젤다의 어머니 같은 존재).
- **Impa** — 시이카 부족의 장로. 카카리코 마을에서 링크에게 가논의 정체와 신수 해방의 의의를 알려준다.
- **Purah와 Robbie** — 하테노/아카라 연구소의 시이카 학자. 시이카 슬레이트 룬 업그레이드 및 가디언 무기 해석 담당.
- **Kass** — 아코디언을 든 음유시인 리토. 챔피언들의 시를 부르며 사이드 퀘스트의 단서를 준다. Champions' Ballad DLC에서 큰 비중.

### 2-4. 무드·톤·아트 디렉션

Takizawa 아트 디렉터가 가장 자주 인용하는 단어가 "전원시(pastoral)"와 "인상주의(impressionism)"다. 《Le Monde》 인터뷰(2017)에서 Aonuma 본인이 "Paul Cézanne을 좋아한다"고 언급했고, 풀밭의 흔들림·구름의 그라데이션·먼 산의 색온도 변화는 의도적으로 후기 인상주의 회화의 색채감을 참조하고 있다.

또 다른 큰 축은 **Studio Ghibli, 특히 미야자키 하야오의 풍경 미학**이다. Nintendo Life·CBR 등에서 반복적으로 지적된 바, 풀밭을 가로지르는 바람의 표현, 일본 동물 애니메이션의 동작 감각, 그리고 "Princess Mononoke적인 자연의 신성함"이 명확히 느껴진다. Takizawa는 GDC 2017 강연에서 "기술적 한계 때문에 사실적 텍스처를 포기하고 페인터리(painterly) 스타일을 선택한 것이 결과적으로 게임의 영원성을 만들었다"고 회고했다.

기술적으로는 **셀 셰이딩 + 라디오시티 + 동적 광원**의 조합이다. 그러나 BotW가 셀 셰이딩 게임으로 보이지 않는 이유는, Takizawa가 "선의 두께를 거의 0에 가깝게 조정하고 그라데이션을 미세하게 깔았기 때문"이다(《Famitsu》 2017년 4월호).

### 2-5. 사운드 — "음악을 비우는 음악"

리드 컴포저 **Manaka Kataoka**는 《Animal Crossing》·《Phantom Hourglass》·《Spirit Tracks》를 거친 닌텐도 베테랑이지만, Zelda 시리즈에서 처음으로 메인 컴포저를 맡았다. 그녀가 선택한 길은 시리즈의 영웅적 오케스트라 테마를 정면으로 부정하는 것이었다. "오픈 필드에서는 자연의 소리를 듣고, 멀리 짐승의 울음과 강의 흐름을 느꼈으면 했다. 그래서 음악을 일부 희생했다"(닌텐도에브리싱 인터뷰, 2017).

대신 그녀는 다음과 같은 디자인을 택했다.

- **시간대별 동적 피아노 모티프** — 낮에는 일정한 간격으로 흩어지는 피아노 단음, 새벽에는 약간의 현, 밤에는 거의 묵음에 가까운 잔향. 같은 지역도 시간대마다 음악이 다르다.
- **지역 모티프** — 카카리코 마을은 일본풍 샤미센, 게루도 사막은 중동 풍 더블 리드, 조라 영역은 아일랜드 풍 하프 등. 모티프는 1분이 안 되는 짧은 루프지만 변주가 많다.
- **메인 테마의 의도적 지연** — 트레일러에서 들렸던 오케스트라 메인 테마는 정작 게임 안에서는 하이랄 성에 진입했을 때, 그리고 최종 보스전에서 결정적으로 등장한다. 작곡가 야스아키 이와타가 인터뷰에서 "메인 테마를 마지막 보상으로 남겨둔 것은 의도된 디자인"이라고 언급.

이 "비우는 음악"은 발매 직후 평론과 유튜브 분석가들 사이에서 갈렸으나, 시간이 지날수록 "오픈월드에서 BGM 피로를 어떻게 줄일 것인가"의 모범 답안으로 자리 잡았다.

---

## 3. 핵심 시스템 / 메카닉 — 가장 중요한 장

### 3-1. 코어 게임플레이 루프 (모먼트-투-모먼트)

BotW의 한 사이클을 1분 단위로 분해하면 다음과 같다.

1. **목표 응시(Look)**: 플레이어는 언덕 위에 서서 멀리 시이카 타워 또는 사당, 산봉우리, 적의 야영지를 본다. 트라이앵글 룰(3-3 참조)에 의해 시야에 들어오는 "관심 지점"은 한 번에 2~3개로 제한된다.
2. **이동 선택(Decide)**: 직선으로 갈 것인지, 산을 오를 것인지, 풀밭을 우회할 것인지 결정한다. 패러글라이더와 스태미나 게이지가 비용 함수에 들어간다.
3. **상호작용(Interact)**: 도중에 새가 둥지에 알을 품고 있거나, 풀더미가 흔들리거나, 보코블린이 야영하고 있거나, 가디언이 누워 있는 발견이 발생한다. 거의 모든 상호작용은 "물리·화학 엔진" 안에서 결과가 결정된다.
4. **보상(Reward)**: 사당 발견, 코록 씨앗, 새로운 레시피, 새 무기, 또는 기억의 회상. 시이카 슬레이트 지도에 새로운 핀이 박힌다.
5. **다음 응시**: 보상 직후 다시 멀리 새로운 트라이앵글이 보인다. 사이클이 닫힌다.

이 루프의 본질은 **"한 사이클 안에서 풀스크린이 절대 의도되지 않은 발견으로 끊긴다"**는 점이다. Game Maker's Toolkit의 Mark Brown(2017)은 이를 "infinite loop of discoveries — a breadcrumb trail of landmarks"라 표현했다.

### 3-2. 진행 구조 — 비선형의 정도

BotW의 진행 구조는 다음과 같이 위계를 가진다.

**Tier 1 (강제)** — 위대한 고원(Great Plateau) 튜토리얼. 약 1~3시간 분량. 4개의 튜토리얼 사당에서 4개의 룬(Magnesis, Stasis, Cryonis, Remote Bomb)을 얻고, 패러글라이더를 노인에게서 받아야 평원 밖으로 나갈 수 있다. 이 절벽이 사실상 "튜토리얼 감옥"이다.

**Tier 2 (권장이나 강제 아님)** — 4기 신수 해방. 그러나 신수는 어떤 순서로든 클리어할 수 있고, 모두 클리어하지 않아도 최종 보스에 갈 수 있다. 신수를 클리어할수록 챔피언의 가호(특수 능력)가 추가되어 난이도가 낮아진다.

**Tier 3 (완전 자유)** — 120개의 사당 (Shrine), 900개의 코록 씨앗, 76개의 사이드 퀘스트, 42개의 사당 퀘스트, 마스터 소드 회수(13하트 요구). 어떤 순서로든 할 수 있다.

**최종 보스** — 위대한 고원에서 패러글라이더를 받자마자 곧장 하이랄 성으로 직진해서 가논을 격파할 수 있다. **이것이 BotW의 가장 충격적인 디자인 선언**이다. Aonuma는 "이걸 막지 않은 것은 의도였다. 시이카 슬레이트와 패러글라이더만 있으면 모든 시스템이 작동하니까"(《Game Informer》 2017)라고 말했다. 실제로 스피드런 Any% 카테고리에서는 30분 안에 게임 클리어가 가능하다.

### 3-3. 트라이앵글 룰 — 오픈월드 장르의 새로운 문법

GDC 2017과 그 이후 Mark Brown의 영상에서 공개된 가장 영향력 있는 디자인 원칙. 닌텐도는 하이랄 전체 지형을 **"삼각형(피라미드/원뿔 형태의 언덕·산·바위)의 집합"**으로 설계했다. 삼각형은 세 가지 스케일로 운용된다.

- **대형 삼각형** — 데스 마운틴, 게루도 고원, 하이랄 성처럼 멀리서도 보이는 시각적 랜드마크. 30km 떨어진 지점에서도 보이게 설계.
- **중형 삼각형** — 시야를 가리는 차폐물. 플레이어 시야 안에 들어오는 관심 지점을 의도적으로 2~3개로 제한한다. "오픈월드 피로(open-world fatigue)"의 주범인 "동시에 50개의 아이콘이 뜨는 미니맵 문제"를 지형으로 해결한 것.
- **소형 삼각형** — 점프·등반 동작의 미시적 리듬. 작은 바위 하나, 나무 하나가 캐릭터 동작의 페이싱을 만든다.

Mark Brown은 이 룰이 해결한 본질적 문제를 이렇게 정리한다. 개발 후반부 테스트에서 플레이어는 두 부류로 갈렸다. (a) 80%는 명시된 마커를 따라 직선으로만 이동, (b) 20%는 무작정 방황하다 길을 잃었다. 어느 쪽도 "발견의 즐거움"을 느끼지 못했다. 트라이앵글 룰은 두 부류를 통합시켰다. **"시야를 가리는 산이 있으면 플레이어는 그 너머에 무엇이 있는지 궁금해진다. 그래서 산을 넘는다. 그 너머에서 새로운 산이 보인다. 다시 넘는다. 이 자체가 게임의 코어 루프가 된다."**

이 디자인 철학은 이후 《Genshin Impact》(2020), 《Elden Ring》(2022), 《Horizon Forbidden West》(2022), 《Tears of the Kingdom》(2023), 《Black Myth: Wukong》(2024) 등 거의 모든 후속 오픈월드의 지형 디자인에 직접 영향을 줬다.

### 3-4. 화학 엔진(Chemistry Engine) — BotW의 진짜 발명품

기술 디렉터 **Takuhiro Dohta**가 GDC 2017에서 가장 길게 설명한 부분. 닌텐도는 "물리 엔진(Physics Engine)"에 대응하는 개념으로 "**화학 엔진(Chemistry Engine)**"이라는 자체 시스템을 만들었다. 정의는 다음과 같다.

> "Physics engine handles motion. Chemistry engine handles state."
> — Takuhiro Dohta, GDC 2017
> (한국어 의역: "물리 엔진은 움직임을, 화학 엔진은 상태를 다룬다.")

화학 엔진은 세 가지 규칙으로 작동한다.

1. **Elements alter material states** — 원소(불·물·전기·바람·얼음)는 물체의 상태를 바꾼다. 예: 불은 나무를 태운다, 얼음은 물을 얼린다.
2. **Elements transform each other** — 원소들끼리도 서로 상호작용한다. 예: 물은 불을 끈다, 번개는 물을 통해 전도된다.
3. **Materials don't affect each other's states** — 물체끼리는 서로의 상태를 직접 바꾸지 않는다(이건 물리 엔진의 영역).

이 단순한 3원칙이 만들어내는 결과가 폭발적이다. 예시:

- 풀밭에 불을 붙이면 → 화염이 바람 방향으로 번진다 → 화염 위에 상승 기류가 발생한다 → 그 기류에 패러글라이더를 펴면 → 절벽 위로 단숨에 날아오를 수 있다.
- 비가 오는 중에 금속 무기를 들고 있으면 → 번개가 떨어진다 → 사망 또는 적 폭사.
- 적 야영지의 폭발 통을 화살(또는 불화살)로 맞히면 → 통이 폭발 → 적이 무기를 손에서 떨어뜨림 → 그 무기를 주워 쓸 수 있음.
- 얼음 칸토라를 물 위에 만들어 다리로 쓰면서, 그 위에서 정지(Stasis) 룬으로 통나무에 운동에너지를 누적시켜 적을 멀리 날려보낼 수 있다.

이 화학 엔진이 시리즈의 또 다른 발명품인 **"Multiplicative Gameplay(곱셈식 게임플레이)"**를 가능케 한다. Fujibayashi의 정의를 그대로 옮기면:

> "We shifted from additive design to multiplicative design. Objects react to player's action, and objects also influence each other."
> — Hidemaro Fujibayashi, GDC 2017
> (한국어 의역: "우리는 덧셈식 설계에서 곱셈식 설계로 옮겨갔다. 물체가 플레이어 행동에 반응할 뿐 아니라, 물체와 물체끼리도 서로 영향을 미친다.")

전통적 Zelda(또는 대부분의 게임)은 "Bomb로 벽을 부순다", "Hookshot으로 천장 핀을 잡는다"처럼 도구와 솔루션이 1:1로 묶인 **덧셈식**이었다. BotW는 도구(룬 4개) × 환경(불·물·전기·바람·얼음·금속·풀·나무 등) × 무기(화살·검·창·검·기괴한 가디언 무기) × 시간/날씨로 곱셈된다. 결과적으로 한 사당 퍼즐을 5가지 이상의 방법으로 풀 수 있고, "이 방법은 의도된 솔루션이 아닐 것 같은데 작동한다"는 경험이 상시 발생한다. Kotaku의 Jason Schreier가 "Breath of the Wild always says yes"라고 표현한 것이 바로 이 지점이다.

### 3-5. 시이카 슬레이트 룬 — 게임 시스템의 백본

플레이어가 처음 위대한 고원에서 받는 도구. 4기의 사당에서 각각 하나씩 4개의 룬이 해금된다. 모두 무한 재사용이 가능하며 쿨다운만 존재한다.

| 룬 | 기능 | 디자인 의도 |
| --- | --- | --- |
| **Remote Bomb** (구·각형 2종) | 원격 폭탄. 던지고 트리거로 폭파. 무한. | 전통 Zelda 폭탄과 달리 무한대로 쓸 수 있어 **자원 관리가 아닌 도구로서 작동**. 채광·낚시·전투·물리 퍼즐 등 다목적. |
| **Magnesis** | 금속 물체 자기력 조작. 멀리 있는 철 상자·문·다리를 끌어 옴. | "물리 엔진이 실제로 작동한다"는 시각적 증명. |
| **Stasis** | 물체를 시간 정지. 정지 중 가한 충격은 누적되었다가 한꺼번에 폭발. | "운동에너지의 누적"이라는 물리 개념을 게임 메카닉으로 직접 번역. 거대 바위를 정지 → 망치로 때려 운동에너지 축적 → 시간이 풀리면 산 너머로 날려보내는 트릭이 명물. |
| **Cryonis** | 수면 위에 얼음 기둥 생성. 다리·받침대로 사용. | 강·해안 지형의 **수직성**을 보장. |

DLC 1탄에서 **Hero's Path Mode** (지난 200시간의 동선을 지도에 그려주는 기능), **Travel Medallion** (한 곳에 임시 워프 포인트 설치) 같은 메타 도구가 추가됐다.

### 3-6. 전투 시스템 — 무기 내구도와 회피 시스템

BotW의 전투는 액션 어드벤처라기보다 **즉흥 활용(improvisation) 시뮬레이터**에 가깝다.

- **무기 내구도** — 모든 무기·방패·활은 사용 횟수에 따라 부서진다(마스터 소드 제외, 마스터 소드도 30회 정도 쓰면 충전 모드로 전환됨). 이는 발매 직후 가장 큰 논란을 일으킨 시스템(6장 참조).
- **회피·패리 시스템** — 적의 공격 직전에 점프 또는 옆구르기를 입력하면 **Flurry Rush**(슬로우 모션 8연타)가 발동된다. 적의 화살을 정확한 타이밍에 막으면 **Perfect Guard**가 되어 무기 손상이 없고 일부 적은 화살을 튕겨낸다.
- **스니크 어택** — 야간에 등을 보인 적에게 접근하면 약 8배 데미지. 보코블린 야영지를 사전에 정리하는 핵심 전술.
- **활시위 시점의 슬로우 모션** — 점프 후 공중에서 활을 당기면 시간이 느려져 정확한 헤드샷을 노릴 수 있다. 회의주의자들의 핵심 슬레이어 무브.

가장 상징적인 적은 **Lynel(라이넬)**이다. 켄타우로스 같은 거대 짐승으로, 4가지 색상(빨강 → 파랑 → 흰색 → 은빛 → 황금)으로 강도가 올라간다. 게임 후반의 라이넬은 일반 적이라기보다 보스에 가까운 난이도이며, 라이넬을 헤드샷으로 마운트하여 검을 박는 액션이 BotW 액션의 백미로 평가된다. **Guardian(가디언)**은 100년 전 시이카가 만든 자율 병기로, 거미형(스토커)·고정형(스토너)·소형 비행형으로 나뉜다. 게임 초반에 멀리서 가디언이 발사하는 푸른 레이저에 일격사 당하는 경험은 BotW 초반의 트라우마로 회자된다.

### 3-7. 등반·스태미나·날씨 시스템

BotW가 다른 모든 오픈월드와 결정적으로 구분되는 것은 **"세계의 거의 모든 표면이 등반 가능하다"**는 점이다. Aonuma가 인터뷰에서 강조한 핵심.

> "If you see a mountain, you can climb it."
> — Eiji Aonuma, E3 2016 시연
> (한국어 의역: "산이 보이면, 그 산은 오를 수 있는 산이다.")

등반의 비용은 **스태미나 게이지(Stamina Wheel)**다. 등반·달리기·패러글라이더·전력 활시위·수영이 모두 같은 자원에서 빠진다. 이 단일 자원이 BotW의 모든 행동을 통합한다. 게이지는 5개의 사당 보상(Spirit Orb 4개)으로 한 칸씩 늘릴 수 있다.

**날씨와 등반의 결합**이 BotW의 또 다른 결정적 시스템이다. **비가 오면 등반 시 미끄러진다.** 한 번 미끄러지면 1~2m 떨어지고, 비가 그칠 때까지 산 등반이 거의 불가능해진다. 이를 두고 발매 직후 "짜증나는 시스템"이라는 비판도 있었지만, **"즉시 멈추지 말고 모닥불 앞에 앉아 아침까지 시간을 보내라"**라는 시간 시스템 사용을 강제하는 의도된 디자인이다. Fujibayashi: "비가 오면 그 자체가 게임의 일부이며, 비를 피하기 위해 동굴로 들어가면 그 동굴이 새로운 발견이 된다"(GDC 2017).

이 외 날씨 시스템은 **온도**도 관리한다. 영하의 설산에 들어가면 옷이나 따뜻한 요리가 없으면 체력이 깎이고, 화염 화산 지역(Eldin)은 반대로 옷이 불에 탄다. **번개 폭풍** 중에는 금속 무기를 장비하면 100% 번개에 맞아 즉사한다(=의도적으로 적 위에 금속 무기를 던지면 적을 번개로 잡을 수 있다).

### 3-8. 사당(Shrine) — 던전을 분해해 다시 짓다

전통 Zelda의 던전 8~9개를 BotW는 **120개의 미니 던전(사당)**으로 분해했다. 평균 5~15분 분량, 단일 콘셉트의 퍼즐 또는 전투 챌린지. 4개의 룬, 물리, 화학을 활용한 작은 실험실이다. 모든 사당은 클리어 시 **Spirit Orb 1개**를 주고, 4개를 모으면 카카리코·하테노 등의 여신 동상에 헌납하여 하트 컨테이너 또는 스태미나 게이지 한 칸으로 교환할 수 있다.

사당의 디자인 카테고리:
- **Combat Trial** — 단일 보스 가디언과의 전투 (Major Test of Strength 등급은 후반에도 위협적).
- **Physics Puzzle** — Magnesis로 미로 안의 공을 굴리는 식의 물리 퍼즐.
- **Stasis / Cryonis Puzzle** — 운동에너지 누적 또는 얼음 다리 활용.
- **Motion Puzzle** — Joy-Con 자이로를 활용한 미로 회전.
- **Shrine Quest 보상형** — 게임 세계에서 특정 조건을 만족시켜야 입구가 열림 (예: Eventide Island).

특히 **Eventide Island**의 사당 퀘스트는 평론가들이 BotW 디자인의 정수로 꼽는다. 섬에 발을 디딘 순간 모든 장비·요리·룬 외 능력이 박탈되고, 섬에 흩어진 자원만으로 적과 싸워 3개의 오브를 회수해야 한다. 단 한 번이라도 죽으면 처음부터. "BotW의 모든 시스템이 한 작은 섬 안에 압축되어 있다"는 평이다.

### 3-9. 코록 씨앗 — 900개의 강박

지도 전역에 숨겨진 작은 풀의 정령 "Korok"이 900개 존재한다. 각각은 특정 환경적 단서(같은 색의 꽃 5개, 풀밭 한가운데 떨어져 있는 돌, 시야 정중앙에 우물처럼 보이는 흙더미 등)를 통해 등장하며 코록 씨앗 1개를 준다. 씨앗은 코록 숲의 거대 정령 Hestu에게 가져가 인벤토리 슬롯(무기·활·방패)을 확장하는 데 쓰인다. 모든 슬롯 확장에 필요한 씨앗은 약 441개로, 나머지 459개는 "수집의 즐거움" 이외에 어떤 보상도 없다.

900개를 모두 모은 플레이어는 황금 똥(Hestu's Gift)을 받는다. 《Vice》의 기사("Finding All 900 Korok Seeds Is a Journey Into Madness", 2017)에서 첫 100% 달성자 Jesus Arce는 발매 11일 만에 모든 씨앗을 수집했다고 보도됐다. 닌텐도가 황금 똥을 보상으로 둔 것은 **"완벽주의자의 시간을 비웃는 농담"**으로 해석되어 인터넷 밈이 됐다.

### 3-10. 요리 시스템

화학 엔진의 응용 사례. 최대 5개의 재료를 냄비에 던지면 결과물이 자동 생성된다. 같은 재료라도 비율과 보조 재료에 따라 다른 요리가 나오며, **곤충·도마뱀·괴물 부위를 섞으면 "엘릭서(Elixir)"**가 된다. 효과는 회복, 한기·열기 저항, 전기 저항, 스태미나 회복, 공격력/방어력 일시 상승, 야간 시야 등 다양하다. 인벤토리에서 직접 조리하는 것이 아니라 **세계 안의 모닥불 옆 냄비에 던지는** 형태라 "요리 자체가 게임의 한 장면"이 된다. 10% 확률로 발생하는 크리티컬 효과(+추가 하트, +효과 시간, +효과 등급)가 존재해 미세한 도박 요소도 있다.

### 3-11. 최종 보스 — 하이랄 성과 가논

하이랄 성은 단일 던전이라기보다 **수직적 오픈 던전**이다. 외부 정원·내부·지하 감옥·왕좌의 방·천문대까지 모든 경로가 외부에서 접근 가능하며, 도서관에서는 100년 전 젤다의 일기를 발견할 수 있다. 신수를 클리어하지 않고 도착하면 신수 보스 4명이 추가 보스로 다시 등장한다(Waterblight·Fireblight·Thunderblight·Windblight Ganon). 신수를 모두 클리어했다면 신수의 가호가 발동되어 챔피언들이 가논의 체력을 절반으로 깎고 시작한다.

최종 보스는 두 단계다.

1. **Calamity Ganon** — 천문대 지하의 거미 형태. "Ganondorf의 분노가 인격을 잃은 것"이라는 디자인. 4개의 Blight Ganon의 공격 패턴을 종합.
2. **Dark Beast Ganon** — 하이랄 평원 위의 거대 멧돼지 형태. 광활한 평원에서 말을 타고 빛의 화살로 마이크 부분을 쏘는 시네마틱 보스전. 아티스트 Yuki Hamada는 "Hyrule Field의 거대함을 마지막에 다시 한 번 보여주고 싶어 그렇게 큰 보스를 만들었다"고 회고.

엔딩 후 자유 탐색이 가능하지만 "Ganon 격파 이전"의 세이브로 돌아가며 별도의 NG+는 없다. DLC를 켜면 마스터 모드(적 한 등급 강화·체력 회복) 도전이 가능하다.

### 3-12. UI/UX 철학 — 미니멀과 비대각화

BotW의 UI는 시리즈 역사상 가장 비어있다. 화면에 상시 표시되는 정보는 좌상단의 하트·스태미나, 우하단의 무기/활/방패 슬롯, 우상단의 미니맵 정도다. **퀘스트 마커가 없는 사당이 많고**, 사이드 퀘스트도 NPC 대사로만 추적된다(시이카 슬레이트에서 "Adventure Log"를 열어야 텍스트 단서를 다시 볼 수 있다). 미니맵의 "이동 가능 지점"은 플레이어가 직접 사당·타워를 발견하고 등록해야만 나타난다.

이 디자인은 "오픈월드의 정보 과부하"라는 상위 카테고리 문제에 대한 닌텐도의 답이다. 동시기 Ubisoft 오픈월드(Assassin's Creed, Far Cry 시리즈)의 "타워에 올라가면 미니맵에 50개의 아이콘이 한꺼번에 뜬다" 방식과 정반대다.

---

## 4. 평가

### 4-1. Metacritic·OpenCritic 점수

| 매체 | 점수 | 핵심 평 |
| --- | --- | --- |
| **Metacritic (Switch)** | **97/100 (109 리뷰)** | 2017년 최고 점수이자 역대급 평가. 2010년대 최고 게임 다수 리스트 1위. |
| Metacritic (Wii U) | 96/100 (14 리뷰) | Switch보다 약간 낮으나 동일 작품. |
| Metacritic (Switch 2 Edition, 2025) | 94/100 | 4K/60fps 패치 버전. |
| **OpenCritic (Switch)** | **96/100, Mighty 등급, 96% 추천** | 절대 다수의 매체가 만점. |
| **User Score (Metacritic)** | 약 **8.7/10** | 평론과 유저 점수 모두 9점대 근접. |

Wikipedia는 BotW를 "Metacritic 사상 가장 많은 만점(100점) 리뷰를 받은 게임"으로 기록한다. 이 기록은 GTA V, BG3, Elden Ring 등의 후발 주자들에게도 깨지지 않았다(2025년 5월 기준).

### 4-2. 주요 매체 평가 인용

- **IGN — 10/10 (Jose Otero, 2017.03.02)**: "Evocative, exhilarating, and a masterclass in open-world design. ... It's a wonderful sandbox full of mystery, dangling dozens upon dozens of tantalizing things in front of you that just beg to be explored." (의역: "환기력 있고 짜릿한 오픈월드 디자인의 정수. ... 신비로 가득 찬 멋진 샌드박스, 탐험을 갈구하는 수십 개의 매혹적인 것들이 눈앞에 매달려 있다.")
- **GameSpot — 10/10 (Peter Brown)**: "A defining moment for The Legend of Zelda series, and the most impressive game Nintendo has ever created. ... A watershed game that reinvents a 30-year-old franchise."
- **Polygon — 10/10 (Arthur Gies)**: "The first current, vital-feeling Zelda in almost 20 years. Nintendo finally treats its audience like intelligent people."
- **Game Informer — 10/10 (Kyle Hilliard)**: "Represents a profound new direction for one of gaming's best franchises and a new high point for open-world interactive experiences."
- **Edge — 10/10 (Issue 304)**: "Not since Ocarina of Time have we set foot in a world that feels so mind-bogglingly vast and unerringly magical." Edge가 만점을 준 19번째 게임이자 시리즈에서 《Ocarina of Time》, 《Skyward Sword》에 이은 세 번째 만점.
- **Famitsu — 40/40 (4명 만점)**: 1986년 이후 약 25번째 만점.
- **Kotaku — Triumphant (Jason Schreier)**: "Triumphant. Groundbreaking. The pinnacle of Zelda. ... Breath of the Wild always says yes."
- **Eurogamer — Essential (Tom Phillips)**: Essential 추천 배지. "A miracle of a game."
- **Time — Masterpiece (Matt Peckham)**: "A masterpiece Zelda game."

### 4-3. 수상 이력

| 시상식 | 수상 |
| --- | --- |
| **The Game Awards 2017** (2017.12.07) | **Game of the Year**, Best Game Direction, Best Action/Adventure Game |
| **D.I.C.E. Awards 21회 (2018.02.22)** | **Game of the Year**, Adventure Game of the Year, Outstanding Achievement in Game Direction, Outstanding Achievement in Game Design |
| **GDC Awards 2018** | **Game of the Year**, Best Design, Best Audio |
| **BAFTA Games Awards 2018** | **Game Innovation Award** (총 GOTY는 What Remains of Edith Finch에 양보, 그러나 9개 부문 노미네이트) |
| **SXSW Gaming Awards 2018** | Video Game of the Year, Excellence in Game Design 등 |
| **Japan Game Awards 2017** | Grand Award |
| **Famitsu Awards 2017** | Game of the Year |
| **IGN, GameSpot, Polygon, Eurogamer, Entertainment Weekly, Time, Game Informer GOTY 2017** | 거의 모든 매체에서 GOTY 수상 |
| **Metacritic 2010년대 최고 작품 리스트** | 18개 매체의 "Decade Best" 리스트에서 1위 — 2010년대 어떤 게임보다도 많은 1위 표 |

### 4-4. 상업 성과

- **2025년 3월 기준 글로벌 누적 판매 약 3,451만 장** (Switch 약 3,364만 / Wii U 약 170만). Statista, Nintendo IR 자료 기반.
- **시리즈 역대 최고 판매작** (이전 기록은 1998년 《Ocarina of Time》의 약 1,000만 장 수준).
- **북미 런칭** Switch 925,000장 + Wii U 약 35만 = 1.3M. Switch 본체 906,000대를 상회 → **"100% 이상의 어태치율(attach rate)"** 기록. WCCFTech, GameSpot 보도. 닌텐도 회장 Tatsumi Kimishima는 "전례 없는 어태치율"이라 언급.
- **일본 런칭(3월 3~5일)** Switch판 193,060장 + Wii U판 결합 약 23만 장. Famitsu 보도.
- **Nintendo Switch 자체의 흥행 트리거**: Switch는 2017년 3월 발매 후 약 2개월 만에 274만 대 판매. 발매 시점 평론가들의 만장일치 만점이 본체 판매에 직접 기여했다는 분석이 닌텐도 내부 미팅 자료(주주총회 Q&A 2017.06)에서 언급됐다.
- **2018년 BotW는 닌텐도의 "에버그린(evergreen)" 타이틀로 자리잡아 매 분기 100만 장 이상의 신규 판매**.
- **Black Friday/Holiday 시즌**마다 가격이 거의 떨어지지 않는 닌텐도의 정가 정책의 상징.

### 4-5. 유저 평가와 평론-유저 괴리

평론은 거의 만장일치 만점이었지만, 발매 직후 일부 코어 Zelda 팬덤에서는 비판도 적지 않았다. Metacritic 유저 스코어 약 8.7/10에 분포가 있다. 핵심 비판 지점은 6장에서 다룬다.

ResetEra·NeoGAF·Reddit /r/Breath_of_the_Wild의 메가스레드를 종합하면 유저 평은 다음과 같이 갈렸다.

- **긍정 (다수)**: "시리즈를 처음 좋아하게 된 작품", "오픈월드를 다시 좋아하게 만든 작품", "탐험과 발견의 마법을 부활시킨 작품".
- **부정 (소수, 그러나 큰 목소리)**: "전통 던전이 없다", "내러티브가 약하다", "무기 내구도가 짜증난다", "맵이 비어있다", "최종 보스가 쉽다(특히 신수 4개를 모두 깬 경우)".

흥미로운 점은 시간이 갈수록 비평적 합의가 더 강해진다는 것이다. 2023년 《Tears of the Kingdom》이 발매되며 BotW의 디자인 철학이 "검증된 표준"이 되었기 때문이다.

---

## 5. 성공 요인 분석 — 왜 BotW는 이렇게 컸나

### 5-1. 디자인적 성공 요인

1. **"발견의 자유"라는 게임 약속의 새로운 정의**. Aonuma는 "Zelda의 본질은 발견이지만 시리즈는 오래 그 본질에서 멀어졌다"고 인정했다. BotW는 그 본질을 화학·물리·다중 솔루션·트라이앵글 룰로 재발견했다.
2. **"Yes의 게임"이라는 메타 디자인 철학**. 플레이어가 "이런 게 가능할까?"라고 생각한 것의 대부분이 작동한다. 이것이 SNS·YouTube 시대의 게임에서 결정적이었다. 사람들이 자신의 발견을 클립으로 공유하면서 무료 마케팅이 폭증.
3. **트라이앵글 룰**이 만든 "오픈월드 피로"의 해결. 50개의 아이콘이 동시에 뜨는 미니맵 패러다임을 부수고, 시야의 자연스러운 제어로 발견의 페이싱을 만들었다.
4. **시이카 슬레이트 4룬의 통합성**. 4개의 도구만으로 모든 환경 시스템과 상호작용하는 미니멀한 인터페이스 디자인.
5. **사당이라는 새로운 던전 단위**. 8시간짜리 거대 던전 하나보다, 10분짜리 사당 120개가 휴대 모드 시대의 플레이 패턴에 더 잘 맞았다.
6. **음악의 의도적 비움**. 환경음과 발걸음 소리에 집중시킴으로써 "이곳에 있다"는 감각을 극대화.
7. **세이브의 자유**. 어디서든 즉시 세이브 가능하고 5개의 자동 슬롯이 있어 휴대 모드 환경에 최적화. Switch의 휴대 모드라는 새로운 플랫폼 형태와의 시너지가 결정적이었다.

### 5-2. 마케팅·출시 전략

1. **Nintendo Switch 런칭 타이틀이라는 위치**. Switch라는 신규 플랫폼의 "킬러 앱"으로 기능했다. 일본 IT 전문지 《Famitsu》는 "Switch가 팔린 게 아니라 BotW가 팔리면서 Switch가 끌려갔다"고 평했다.
2. **E3 2016 단일 타이틀 부스 전략**. 닌텐도는 그해 E3에서 BotW만을 부스에 전시했다(다른 모든 발표 없이). "닌텐도가 한 게임만으로 E3 부스를 채운다"는 사건이 화제가 되며 기대치를 극대화.
3. **GDC 2017 강연 (발매 이틀 전)**. 평론가들이 만점 점수를 매기는 시점에 개발자가 강연을 통해 "왜 우리가 관습을 깼는지" 설명함으로써 평론의 의미를 강화.
4. **임바고 운영의 정밀함**. 평론가들에게 30일 이상의 충분한 플레이 시간을 제공해 깊은 리뷰가 나오게 함. 평론들이 단순 점수가 아닌 "에세이 수준의 평"을 쓰게 됨.
5. **Wii U 동시 발매라는 위험한 결정**. 후방 호환의 메시지 + Wii U 유저에 대한 의리 + Switch가 실패할 경우의 보험. 결과적으로 Wii U판이 약 170만 장 팔리며 Wii U의 라스트 댄스 역할을 했다.

### 5-3. 타이밍과 시장 환경

1. **오픈월드 장르의 피로 시기**. 2015~2016년은 Ubisoft 공식(Assassin's Creed, Far Cry, Watch Dogs)의 정점이자 피로의 시작이었다. 《Mad Max》(2015), 《Just Cause 3》(2015) 등 거대하나 공허한 오픈월드가 양산됐다. BotW는 "다른 길이 있다"는 신선한 답을 던졌다.
2. **《Horizon Zero Dawn》 발매 1주 후**. 같은 2017년 2월 28일 PS4 독점 《Horizon Zero Dawn》이 발매됐다. 두 작품은 평행한 평가를 받았고 GOTY 경쟁 구도가 형성됐다. 결과는 BotW의 압승이었으나 두 작품의 동시 발매가 "오픈월드의 새 시대"를 알리는 신호탄이 됐다.
3. **휴대 모드 시대의 도래**. iPhone 발매 10주년인 2017년, 휴대 게임에 대한 인식이 변했고 Switch는 거치/휴대 하이브리드라는 새 패러다임을 제시했다. BotW는 그 안에서 "60시간짜리 거대 RPG도 휴대로 가능하다"는 증명이 됐다.

### 5-4. 개발 방법론

1. **2D 프로토타입 우선**. NES 《Zelda》 엔진 형태의 2D 프로토타입에서 화학·물리 엔진을 먼저 검증. 풀에 불을 붙이고, 나무를 베어 뗏목을 만들고, 사냥을 하는 모든 시스템이 2D에서 먼저 작동했다. 이 자료는 GDC 2017에서 영상으로 공개됐다.
2. **"왜 안 되는가"를 질문하는 회의 문화**. Fujibayashi가 강연에서 강조한 부분. "이걸 못하게 할 이유가 있는가?"가 모든 디자인 회의의 첫 질문이었다.
3. **Monolith Soft 외주 활용**. 《Xenoblade Chronicles》의 오픈월드 노하우를 가진 약 50~100명의 외부 인력을 받아들임. 닌텐도 본사가 다른 회사의 노하우를 적극 받아들인 드문 사례.
4. **테스트 환경의 광범위함**. 닌텐도는 "어떤 플레이어도 게임을 부수지 못한다"가 아니라 "어떤 플레이어도 자신만의 방식으로 게임을 풀 수 있다"를 목표로 테스트했다. QA가 발견한 "버그 같은 해법"이 실제로는 디자인으로 인정받아 살아남은 사례가 많다(예: 봄벨릴 점핑·평면 점프 등).

### 5-5. 커뮤니티·IP 효과

1. **30년 시리즈의 누적된 신뢰**. 시리즈 사상 처음으로 코어 Zelda 팬뿐 아니라 일반 게이머·언론·시상식·산업의 모든 시선이 모인 출시.
2. **YouTube/Reddit 생태계 폭발**. "BotW로 가능한 것" 영상이 발매 2년간 매주 화제. 유튜버 BeardBear, Croton, Linkus7 등이 글리치·콤보·완벽한 솔루션 영상을 매주 업로드.
3. **스피드런 커뮤니티의 부흥**. Any% 30분, 100% 60시간대의 카테고리가 정착. 2017년 GDQ에 BotW가 등장하며 게임 발매 후 1년 안에 스피드런으로 인기를 끈 최초의 닌텐도 타이틀이 됐다.

### 5-6. 동시기 작품 대비 차별점

- **《Horizon Zero Dawn》** (2017.02.28) 대비: HZD는 "정교한 스크립트형 오픈월드", BotW는 "시스템 기반 샌드박스". 두 작품을 같은 해에 플레이한 평론가들 대다수가 BotW를 "더 미래 지향적"이라 평했다.
- **《Mass Effect: Andromeda》** (2017.03.21) 대비: 같은 달 발매됐으나 ME:A는 잡다한 사이드 콘텐츠로 비판받았고 BotW는 정확히 그 안티 테제가 됐다.
- **《Super Mario Odyssey》** (2017.10.27) 대비: 같은 해 같은 회사의 GOTY 경쟁작. BotW가 GOTY를 받았으나 Mario Odyssey가 "Best Family/Best Action Platformer"을 가져갔다. 두 작품이 Switch의 두 기둥으로 자리매김.

---

## 6. 비평적 시각·한계·논란

### 6-1. 무기 내구도 — 가장 큰 논쟁

발매 직후 가장 격렬한 논쟁의 주제. ScreenRant·CBR·TheGamer 등 거의 모든 매체에서 별도 기사로 다뤘다. 핵심 비판은 "무기가 너무 빨리 부서져 전투의 흐름이 끊긴다"는 것. 일부 플레이어들은 "강한 무기를 발견해도 부서질까봐 못 쓴다"는 역설을 호소했다.

**Fujibayashi의 의도**: "플레이어가 한 무기에 의존하지 않고 새로운 무기를 끊임없이 시도하도록 설계했다. 무기를 부수는 행위 자체가 적과 마주칠 동기가 된다." 즉, "보상이 무기에서 무기로 흘러가도록 설계된 경제 시스템"이라는 입장.

**반론**: 게임 후반에 강력한 무기를 얻고 나서도 부서지는 속도가 크게 줄지 않는다. 마스터 소드조차 30회 사용 후 충전 모드에 들어가 10분 대기해야 한다. 결국 "최고의 무기를 아껴 쓰다 게임이 끝난다"는 안티-패턴이 발생.

**닌텐도의 대응**: 《Tears of the Kingdom》(2023)에서 Fuse 시스템을 도입해 "무기에 다른 물건을 결합해 내구도와 효과를 확장"하는 방향으로 부분적 답을 냄. 그러나 본질적 내구도 시스템 자체는 유지.

### 6-2. 전통 던전의 부재

전통 Zelda 시리즈의 골격이었던 "고유한 미학과 메카닉을 가진 8~9개의 거대 던전"이 BotW에는 없다. 4개의 신수가 그 역할을 일부 대체하지만, **신수 4개는 모두 비슷한 톤(시이카 기계 미학, 푸른 발광 빛, 비슷한 보스 디자인)을 공유**한다. 시리즈 팬덤(특히 《Twilight Princess》, 《Wind Waker》를 사랑하는 코어 팬)에서는 "Zelda의 영혼이 빠졌다"는 비판이 강했다. 이는 ResetEra·GameFAQs 보드에서 발매 후 6개월 동안 가장 활발했던 논쟁 주제.

이 비판에 대한 닌텐도의 답은 《Tears of the Kingdom》의 4개 던전(Water Temple, Wind Temple, Fire Temple, Lightning Temple)에서 부분적으로 회복됐다.

### 6-3. 스토리 전달의 약점

스토리는 "100년 전 회상"을 통해 단편적으로 전달된다. 18개의 메모리 컷신이 지도 전역에 흩어져 있고 순서 없이 회수 가능하다. 이 비선형성이 일부 플레이어에게는 "감정적 임팩트의 분산"으로 다가왔다. "Mipha가 죽었다는 것을 게임 시작 10시간 후에 알게 되거나, 마지막에 알게 되거나, 아예 모르고 끝낼 수도 있다."

또한 메인 시나리오의 "임팩트 있는 장면"이 게임 안에서 거의 모두 회상으로 처리되어, 현재 시점에서는 정적인 산책 게임처럼 느껴진다는 비판도 있었다.

### 6-4. 음악의 비움 — 호불호의 진원지

위에서 "성공 요인"으로 거론한 음악의 미니멀리즘이, 동시에 가장 큰 호불호의 진원지이기도 했다. 일부 시리즈 팬은 "Zelda는 영웅적 음악의 시리즈"라는 정체성이 사라졌다고 한탄했다. 발매 직후 PC Gamer·GameRant 등에서는 "BotW의 음악은 결여를 통해 의도를 보여주지만, 거대 트레일러 음악을 원하는 팬에게는 실망"이라는 양면 분석이 자주 등장했다.

### 6-5. 프레임 레이트와 해상도

Switch 도킹 모드 900p, 휴대 모드 720p, 30fps 락. 코록 숲처럼 풀이 빽빽한 지역에서는 발매 시점 20fps대까지 떨어졌다. 발매 후 두 차례 패치로 약간의 개선이 있었으나 완전 해결은 안 됐다. 디지털 파운드리(Digital Foundry)의 분석에서는 "Wii U판이 일부 구간에서 Switch판보다 더 안정적"이라는 흥미로운 역설이 보고됐다. Switch 2 Edition(2025)에서 4K/60fps로 마침내 해결.

### 6-6. 최종 보스의 난이도와 어색함

신수 4기를 모두 격파한 플레이어에게 가논의 체력은 절반에서 시작하고 챔피언의 가호가 발동되어 전투가 5~10분 만에 끝난다. "30시간 모험의 클라이맥스가 너무 빠르게 끝난다"는 비판. 반대로 신수를 하나도 깨지 않고 가는 플레이어는 사상 최고 난이도를 경험하는데, 이 양극화 자체가 디자인 선택이지만 일부 평론가들은 "보스전 자체의 만족도가 낮다"고 평가했다.

### 6-7. 사이드 퀘스트의 단순함

76개의 사이드 퀘스트 다수가 "X를 찾아오라" 또는 "Y를 N개 모아오라" 수준의 심부름. 코록 씨앗과 함께 "충분히 깊지 않은 양의 콘텐츠"라는 평이 있었다. 《The Witcher 3》(2015)의 심리적·도덕적 사이드 퀘스트와 비교하면 BotW의 사이드 콘텐츠는 표면적이다는 평. 이는 일부에서 "닌텐도의 무던한 톤" 한계로도 해석됐다.

### 6-8. 빈 맵의 문제

상위 자에 따라 360km²(또는 측정 방법에 따라 60~100km²)에 달하는 맵이 후반부로 갈수록 "걸으면 5분 동안 적·NPC·이벤트가 없는 구간"이 적지 않다. 일부 평론은 이를 "고요의 미학"으로 옹호했고, 일부는 "콘텐츠 밀도의 부족"으로 비판했다. Polygon의 평론가 Maddy Myers는 후일 회고에서 "BotW의 비어있음은 분명 의도지만, 의도가 모든 플레이어에게 작동하지는 않는다"고 정리했다.

### 6-9. 운영 측 논란 — 거의 없음

BotW는 라이브 운영 게임이 아니라 패키지/싱글플레이 게임이라 마이크로트랜잭션·시즌패스 같은 라이브 운영 논란은 없었다. DLC 1+2를 패키지로 묶은 Expansion Pass $19.99가 유일한 추가 수익 모델이고, 이 가격 자체에 대한 큰 논란은 없었다. 이는 동시기의 EA·Activision·Ubisoft의 라이브 서비스 모델과 큰 대조를 이뤘고, 닌텐도의 "한 번 만들고 끝내는" 비즈니스 모델의 우월성을 강조하는 사례로 자주 인용됐다.

### 6-10. amiibo 의존성에 대한 미세한 비판

특정 보상(에포나 말, 트와일라잇 링크 의상, 마조라의 가면 등)이 amiibo에서만 얻을 수 있어 "수집욕 마케팅"이라는 미세한 비판이 있었다. 그러나 이 보상들이 게임 진행에 필수가 아니고 컬렉터블에 가까워 큰 논란으로 번지지는 않았다.

---

## 7. 영향과 유산

### 7-1. 오픈월드 장르에 미친 직접적 영향

BotW는 발매 즉시 "오픈월드의 새로운 기준"이 됐고, 7년이 지난 2024년 시점에서 이를 부정하는 평론가는 거의 없다. 직접적 영향이 보이는 작품들:

- **《Genshin Impact》** (miHoYo, 2020): 등반·패러글라이더·스태미나 게이지·삼각형 지형·원소 상호작용까지 BotW의 디자인 언어를 거의 그대로 차용. miHoYo는 발매 초기 표절 논란이 있었으나, "BotW가 정한 오픈월드 문법을 가챠+서비스 모델로 변환했다"는 평이 우세해졌다. 《Genshin Impact》의 글로벌 매출은 2024년 누적 50억 달러 이상으로, BotW가 만든 디자인 언어의 상업적 검증이 됐다.
- **《Immortals Fenyx Rising》** (Ubisoft, 2020): "Ubisoft가 BotW를 만든다면?"이라는 자조적 표현이 붙은 작품. 트라이앵글 룰·등반·날씨를 그대로 차용했으나 Ubisoft 공식의 아이콘 미니맵을 유지해 어색한 하이브리드가 됐다.
- **《Elden Ring》** (FromSoftware, 2022): "FromSoftware가 BotW를 만든다면?"의 답. 미니맵 아이콘 없는 자유 탐험, "산이 보이면 갈 수 있다"는 약속, 화려한 트라이앵글 지형. Hidetaka Miyazaki는 인터뷰에서 "Zelda 시리즈는 항상 영향이지만, BotW는 특히 ‘열린 발견’의 측면에서 직접적인 자극이었다"고 인정.
- **《Horizon Forbidden West》** (Guerrilla, 2022): 패러글라이더(Shieldwing) 도입은 명백한 BotW 영향. 등반의 자유도도 1편보다 크게 늘었다.
- **《The Legend of Zelda: Tears of the Kingdom》** (Nintendo, 2023): BotW의 직접적 후속작. Ultrahand·Fuse·Recall·Ascend의 4개 새 룬이 BotW의 화학·물리 엔진을 한층 강화했다. 발매 후 첫 3일 1,000만 장 판매로 시리즈 최단 기록.
- **《Black Myth: Wukong》**(Game Science, 2024): 중국 발 액션 RPG이지만 지형의 입체성과 시야 가이드 설계에서 BotW의 흔적이 명확.
- **《Manor Lords》**(Hooded Horse, 2024)와 같은 시티 빌더조차 "지형이 게임플레이를 결정한다"는 메시지를 받았다.

### 7-2. "BotW 효과"라는 산업 용어

평론과 산업 매체에서 "the BotW effect"라는 용어가 정착됐다. GamerSpot·TheGamer의 분석에 따르면 이 용어는 다음을 의미한다.

1. **"산이 보이면 가야 한다"는 약속**.
2. **"미니맵 아이콘으로 채워진 오픈월드는 죽었다"는 인식**.
3. **"여러 시스템이 곱해지면 한 디자이너가 의도하지 않은 경험이 생긴다"는 디자인 철학**.
4. **"퍼즐은 단일 솔루션이 아니라 여러 솔루션을 갖는다"는 인식의 확산**.

이 효과는 단순히 모방을 넘어 "오픈월드를 디자인할 때 BotW를 안 봤다"고 말하는 디자이너가 거의 사라졌음을 의미한다.

### 7-3. 산업적 의미

1. **닌텐도의 부활**. Wii U의 상업적 실패 이후 회의적 시선을 받던 닌텐도가 BotW + Switch 콤보로 부활. 2017~2025년 동안 닌텐도는 Switch 1.5억 대 이상을 판매하며 콘솔 시장의 정상에 복귀.
2. **휴대 모드와 거대 RPG의 양립 증명**. "휴대용 기기에서 60시간 RPG는 안 된다"는 통념을 부수고, 이후 Switch에서 《The Witcher 3》, 《Skyrim》, 《Doom》까지 이식되는 길을 열었다.
3. **GOTY 경쟁의 새 차원**. 2017년 TGA의 BotW vs. Horizon Zero Dawn 경쟁은 "그래픽으로 평가하는 시대의 종언, 시스템으로 평가하는 시대의 시작"으로 기억된다.
4. **GDC 발표의 산업 표준화**. BotW의 GDC 2017 강연은 이후 거의 모든 거대 작품(《God of War 2018》, 《Death Stranding》, 《Elden Ring》)이 발매 직후 GDC에서 디자인 후일담을 발표하게 만든 선례가 됐다.

### 7-4. 문화적 의미

1. **닌텐도 IP의 글로벌 위상 재확인**. BotW의 평가는 닌텐도 게임을 "어린이용"으로 분류하던 서구 일부 평론의 시선을 무너뜨렸다. 2017년 The New York Times·The Guardian이 게임 평론을 본격 다루기 시작한 첫 해이기도 하다.
2. **"오픈월드"라는 단어의 의미 변화**. BotW 이전의 "오픈월드"는 GTA식 도시 시뮬레이션 또는 Ubisoft식 아이콘 채집이었다. BotW 이후의 "오픈월드"는 시스템적 발견을 의미한다.
3. **스피드런 컨퍼런스(SGDQ/AGDQ)에서의 BotW의 위상**. 발매 1년 후부터 거의 모든 GDQ에 BotW Any% 또는 100% 런이 들어가며, "닌텐도 발매작이 스피드런으로 사랑받는 첫 사례"가 됐다.
4. **모드 씬과 에뮬레이션 문화의 폭발**. Cemu(Wii U 에뮬레이터)는 BotW가 발매된 2017년 3월 직후 Patreon 후원이 한 달에 $4,000 → $40,000으로 급증해 전체 Patreon에서 3위에 잠시 올랐다. BotW가 PC 에뮬레이션 씬을 사실상 대중화한 계기. 이후 4K/60fps 모드, "Second Wind" 같은 매시브 모드 등 거대한 모드 생태계가 형성됐다.
5. **"여신 동상에 황금 똥을 헌납하는" 밈**. 코록 씨앗 900개를 모은 보상이 황금 똥이라는 사실은 인터넷 게이밍 밈으로 자리잡았고, 이후 "완벽주의자를 비웃는 닌텐도식 농담"의 대표 사례가 됐다.

### 7-5. 다른 닌텐도 IP에 미친 영향

- **《Super Mario Odyssey》**(2017): "맵을 탐험해 모든 것을 줍는다"는 BotW식 콜렉터블 구조가 일부 들어가 있다.
- **《Pokémon Sword/Shield》**의 Wild Area, 《Pokémon Legends: Arceus》(2022), 《Pokémon Scarlet/Violet》(2022)의 오픈월드는 BotW의 영향이 명확하다. Pokémon 시리즈가 30년 만에 처음으로 본격 오픈월드를 시도한 직접적 계기.
- **《Splatoon 3》의 Salmon Run·Splatlands**, **《Animal Crossing: New Horizons》의 섬 디자인**까지도 BotW의 "발견의 즐거움"이라는 디자인 어휘에서 영향을 받았다고 닌텐도가 공식 인터뷰에서 언급.

---

## 8. 부록

### 8-1. GDC 강연·포스트모템 자료

- **GDC 2017 — "Change and Constant: Breaking Conventions with The Legend of Zelda: Breath of the Wild"** (Hidemaro Fujibayashi, Satoru Takizawa, Takuhiro Dohta). GDC Vault: https://www.gdcvault.com/play/1024562/Change-and-Constant-Breaking-Conventions
- **GDC YouTube 공식 영상**: https://www.youtube.com/watch?v=QyMsF31NdNc (한 영상 90분, 3부)
- **Internet Archive 보관본**: https://archive.org/details/gdc-2017-breaking-conventions-with-the-legend-of-zelda-breath-of-the-wild
- **Game Developer 정리 기사**: https://www.gamedeveloper.com/design/video-designing-i-zelda-breath-of-the-wild-i-s-unconventional-mechanics
- **Thumbsticks (Chemistry/Physics 분석)**: https://www.thumbsticks.com/gdc-17-breath-of-the-wild-science-lies/
- **Mark Brown / Game Maker's Toolkit — "How Nintendo Solved Zelda's Open World Problem"**: https://gmtk.substack.com/p/how-nintendo-solved-zeldas-open-world (트라이앵글 룰의 가장 영향력 있는 외부 분석)
- **Game Developer — "Breath of the Wild Open World Analysis: Gravity to go Forward"**: https://www.gamedeveloper.com/design/breath-of-the-wild-open-world-analysis-gravity-to-go-forward
- **80.lv — "The Design Secrets of Breath of the Wild"**: https://80.lv/articles/the-design-secrets-of-breath-of-the-wild

### 8-2. 주요 인터뷰

- **Eiji Aonuma 《Le Monde》 인터뷰 (2017)** — 영어 번역본: https://nintendoeverything.com/aonuma-on-zelda-breath-of-the-wild-full-le-monde-interview-translation/
- **Eiji Aonuma 《Vice》 인터뷰**: https://www.vice.com/en/article/a-conversation-with-zelda-veteran-and-breath-of-the-wild-producer-eiji-aonuma/
- **《Game Informer》 E3 2016 Aonuma 프리뷰 인터뷰**: 시리즈가 Skyrim에 영감을 받은 부분과 받지 않은 부분.
- **Nintendo Everything — Aonuma on 4-year development**: https://nintendoeverything.com/eiji-aonuma-on-breath-of-the-wilds-development-process-the-games-physics-engine-more/
- **Manaka Kataoka 음악 인터뷰** (Nintendo Everything): https://nintendoeverything.com/breath-of-the-wild-composers-on-changing-up-zeldas-music-formula-and-more/

### 8-3. 핵심 통계 표

| 지표 | 수치 | 출처 |
| --- | --- | --- |
| Metacritic Switch | 97/100 | metacritic.com |
| Metacritic Wii U | 96/100 | metacritic.com |
| OpenCritic | 96/100 (Mighty) | opencritic.com |
| Famitsu | 40/40 (만점) | Famitsu Issue 1475 |
| Edge | 10/10 | Edge Issue 304 |
| 글로벌 누적 판매 (2025.03) | ~34.51M | Statista, Nintendo IR |
| Switch 판매 | ~33.64M (2025.12) | Nintendo IR |
| Wii U 판매 | ~1.70M (2020.12) | Nintendo IR |
| 북미 런칭 어태치율 | 100% 초과 | WCCFTech 2017 |
| 일본 런칭 첫 주 | ~230,000 (Switch+Wii U) | Famitsu 2017.03 |
| 사당 총 수 | 120개 | 본 게임 |
| 코록 씨앗 총 수 | 900개 | 본 게임 |
| 사이드 퀘스트 | 76개 | 본 게임 |
| 사당 퀘스트 | 42개 | 본 게임 |
| 신수 (메인 던전) | 4기 | 본 게임 |
| 룬 (시이카 슬레이트) | 4종 + 카메라/슬레이트 | 본 게임 |
| 평균 클리어 시간 (메인) | ~50시간 | HowLongToBeat |
| 100% 완전 클리어 | ~190시간 | HowLongToBeat |
| 발매 시 최고 속도 Any% (2017) | ~50분 | Speedrun.com |
| 2024 시점 최고 속도 Any% | ~22~30분 | Speedrun.com (sketodara01417 외) |
| 개발 기간 | 4~5년 (2013~2017) | Aonuma 인터뷰 |
| 개발 인력 | 약 300명 (Monolith Soft 포함 ~400명) | Nintendo IR Q&A 2017 |
| 추정 예산 | ~$1억 [추정] | ResetEra 추산 |
| TGA 2017 GOTY | 수상 | The Game Awards |
| BAFTA 2018 Game Innovation | 수상 (GOTY는 Edith Finch) | BAFTA |
| D.I.C.E. 2018 GOTY | 수상 | AIAS |
| GDCA 2018 GOTY | 수상 | GDC |

### 8-4. 참고 자료 목록 (영어권 매체 중심)

리뷰
- IGN — Jose Otero — 10/10, 2017.03.02
- GameSpot — Peter Brown — 10/10, 2017.03.02
- Polygon — Arthur Gies — 10/10, 2017.03.02
- Game Informer — Kyle Hilliard — 10/10, 2017.03.02 (Issue 287 표지)
- Edge — 10/10, 2017.03.02 (Issue 304)
- Famitsu — 40/40, 2017.02.28
- Kotaku — Jason Schreier (점수 없음, "Triumphant"), 2017.03.02
- Eurogamer — Tom Phillips — Essential, 2017.03.02
- Time — Matt Peckham — "Masterpiece", 2017.03.02
- Variety, EW, New York Times, The Guardian — 모두 만점급 추천

산업·디자인 분석
- Wikipedia — The Legend of Zelda: Breath of the Wild (가장 종합적 1차 자료)
- Game Maker's Toolkit (YouTube) — Mark Brown — "How Nintendo Solved Zelda's Open World Problem"
- Thumbsticks — GDC 정리 시리즈
- Game Developer (구 Gamasutra) — 디자인 후일담 다수
- Zelda Universe / Zelda Dungeon / Zelda Wiki — 백과사전적 자료
- 80.lv — 아트·디자인 분석
- Nintendo Everything — 닌텐도 인터뷰 번역
- Bloomberg / Jason Schreier — 산업 측 보도
- Famitsu — 일본 측 자료

사용자 자료
- Reddit /r/Breath_of_the_Wild — 100% 가이드·발견 메가스레드
- ResetEra — 평가·논쟁 메가스레드 다수
- Speedrun.com /botw — 카테고리·기록·글리치 정보
- GameFAQs — 가이드·FAQ
- Vice — "Finding All 900 Korok Seeds Is a Journey Into Madness"

### 8-5. 한 줄 결론

> 닌텐도는 1986년 자신들이 만들어낸 자유라는 약속의 의미를, 30년이 지난 2017년에 다시 발견했고, 그 발견을 모든 동시대 디자이너에게 강제로 공유했다. 《Breath of the Wild》는 단지 한 시리즈의 19번째 작품이 아니라, "오픈월드"라는 단어 자체의 정의를 갱신한 사건이다. 이 갱신이 갱신되려면 또 한 번의 30년이 필요할지도 모른다.

---

작성: 2026-05-20.
출처: Wikipedia (en), Metacritic, OpenCritic, IGN, GameSpot, Polygon, Game Informer, Edge, Kotaku, Eurogamer, Time, Famitsu, Nintendo IR, Statista, GDC Vault, GDC YouTube, Game Maker's Toolkit, Thumbsticks, Game Developer, 80.lv, Nintendo Everything, Le Monde, Vice, Speedrun.com, Reddit /r/Breath_of_the_Wild, ResetEra, GameFAQs, HowLongToBeat, ZeldaUniverse, ZeldaDungeon.
