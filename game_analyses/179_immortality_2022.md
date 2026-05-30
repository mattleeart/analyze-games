# 《IMMORTALITY》 (2022) 심층 분석 — FMV의 정점, 그리고 영화에 깃든 불멸의 존재

> 한 여배우가 세 편의 영화를 찍고 단 한 편도 개봉하지 못한 채 사라졌다. 50여 년이 흐른 뒤, 당신은 편집실의 의자에 앉아 그 잃어버린 필름의 잔해를 한 컷씩 되감으며 진실을 추적한다. 그리고 어느 순간, 화면이 당신을 마주 본다. 《IMMORTALITY》는 영화라는 매체의 마법을 게임의 문법으로 번역해낸, FMV(Full-Motion Video) 장르 역사상 가장 야심차고 완성도 높은 시도다.

---

## 1. 게임 개요

《IMMORTALITY》는 Sam Barlow가 만들고 그의 스튜디오 **Half Mermaid Productions**가 퍼블리싱한 인터랙티브 필름(FMV) 게임이다. 2022년 8월 30일 Windows와 Xbox Series X/S로 동시 출시되었으며, Xbox 진영에서는 **출시 당일(Day 1) Game Pass**에 포함되었다. 이후 다음과 같이 멀티플랫폼으로 확장되었다.

| 플랫폼 | 출시일 | 비고 |
|---|---|---|
| Windows / Xbox Series X·S | 2022-08-30 | Day 1 Xbox Game Pass |
| Android / iOS | 2022-11-16 | Netflix Games 독점 |
| macOS | 2023-04-05 | |
| PlayStation 5 | 2024-01-23 | |

장르는 통상적인 의미의 "게임"이라기보다 **인터랙티브 필름**으로 분류된다. 플레이어는 캐릭터를 직접 조작하지 않으며, 대신 **필름 클립을 탐색하고 재배열하며 미스터리를 풀어내는** 행위 자체가 게임플레이의 전부다.

**핵심 크레딧**
- **디렉터·총괄 작가:** Sam Barlow — 《Silent Hill: Shattered Memories》(2009)의 수석 디자이너이자, 인디 FMV 르네상스를 이끈 《Her Story》(2015)·《Telling Lies》(2019)의 창작자. 한때 Square Enix에서 《Legacy of Kain》 신작을 개발하다 취소된 이력도 있다.
- **공동 각본:** Amelia Gray(소설가), Allan Scott(《Don't Look Now》 각본가, 본작에서 《Minsky》 집필), Barry Gifford(《Wild at Heart》·《Lost Highway》 원작·각본가)
- **프로듀서:** Natalie Watson, Jeff Petriello, Shyam S. Sengupta
- **프로그래머:** Connor Carson
- **작곡:** Nainita Desai — Emmy 2회 노미, Ivor Novello 노미, World Soundtrack Awards 2021 "Discovery of the Year" 수상자

**개발 규모와 일정.** Barlow는 이 프로젝트에 약 **1년 반의 기획·사유 기간**을 들인 뒤, **6개월의 프로덕션(촬영)**과 **6개월의 백엔드 개발**을 거쳤다고 밝혔다. 게임은 2020년 코드네임 "Project Ambrosio"로 처음 언급되었고, 2021년 E3에서 정식 공개되었다. 영화 촬영은 2021년 8월 로스앤젤레스 Arts District에서 약 **10주간**, 무려 **400페이지 분량의 대본**을 바탕으로 진행되었다. 당초 2022년 7월 26일 출시 예정이었으나 8월 30일로 연기되었고, 그에 앞서 2022년 6월 Tribeca Film Festival에서 프리미어 상영되어 게임으로는 이례적으로 **Official Mention**을 받았다.

**기술 스택.** 엔진은 **Unity**다. 본작의 가장 큰 기술적 도전은 후술할 "match cut" 시스템으로, 실사 영상 데이터베이스 안에서 인물·사물을 인식해 관련 클립으로 점프시키는 메커니즘을 구현하는 데 엔진과 자체 백엔드 파이프라인이 결합되었다.

---

## 2. 게임 설명 — 이 게임은 무엇인가

### 표면의 이야기

당신에게 주어지는 것은 단 하나의 영화 클립이다. 화면은 1960~90년대 영화 필름의 질감을 가진, 빛바랜 아날로그 영상이다. 이야기의 중심에는 **Marissa Marcel(마리사 마르셀)** 이라는 가공의 여배우가 있다. 그녀는 세 편의 영화에 주연으로 출연했지만, **세 편 모두 개봉되지 못했고**, 그녀 자신도 흔적 없이 사라졌다. 플레이어의 임무는 이 미공개 필름들의 본편·미사용 컷·비하인드 씬·TV 인터뷰·리허설 영상의 파편을 모으고 이어 붙여, 마리사에게 무슨 일이 있었는지를 스스로 추리하는 것이다.

게임 안에는 실제로 **세 편의 가상 영화**가 통째로 들어 있다.

**1) 《Ambrosio》 (1968) — 누나스플로이테이션 고딕 호러**
M.G. Lewis의 악명 높은 고딕 소설 《The Monk》을 각색한 작품. 마리사의 첫 주연작으로, 그녀는 경건한 수도사 Ambrosio를 유혹하기 위해 남장을 하고 수도원에 잠입하는 매혹적인 미녀 **Matilda(마틸다)** 역을 맡는다. 감독은 Arthur Fischer. 이 영화는 감독이 직접 네거티브 필름을 훔쳐 달아나면서 영원히 미개봉작이 된다. 마리사는 이 현장에서 촬영감독 **John Durick(존 듀릭)** 과 사랑에 빠진다.

**2) 《Minsky》 (1970) — 뉴욕 누아르 탐정극**
2년 뒤, 촬영감독이던 John Durick이 마리사를 위해 직접 감독·공동각본을 맡은 작품. 마리사는 뉴욕의 거물 예술가 Minsky의 뮤즈 **Franny(프래니)** 역을 연기한다. Minsky가 살해당하자 프래니가 유력 용의자가 되고, 사건을 수사하는 풋내기 형사와 격정적인 로맨스에 빠진다. **[스포일러]** 촬영 도중 배우 Carl Greenwood가 마리사가 든 소품 총에 근거리에서 피격당해 사망한다. 표면적으로는 비극적 사고로 처리되지만, 실은 의도적 살인이었음이 드러난다. 이 영화 역시 끝내 개봉되지 못한다.

**3) 《Two of Everything》 (1999) — 이중성의 전복적 스릴러**
팝스타 Maria와 그녀의 신체 대역 Heather 사이의 이중성을 다루는 스릴러. 마리사가 **1인 2역**을 소화한다. 극중극 구조에서, 빌리어네어의 부인이 Heather를 진짜 Maria로 착각해 살해한다. **[스포일러]** 촬영 도중 마리사가 원인 모를 출혈을 일으키며 쓰러지고, 제작은 중단된다.

세 영화는 1968년, 1970년, 1999년이라는 서로 다른 시대를 배경으로 하며, 마리사는 30여 년이 흘러도 거의 늙지 않은 모습으로 다시 나타난다. 이 "나이를 먹지 않는다"는 단서가 게임의 진짜 정체를 향한 첫 번째 균열이다.

### 표면 아래 — 진짜 이야기 [스포일러 전면]

《IMMORTALITY》의 제목이 가리키는 진실은 초자연적이다. 인류가 등장하기 이전부터 존재해 온 두 불멸의 존재가 있다. **"The One"** 과 **"The Other"** 다. 이들은 인간의 형상을 취하고 그 삶을 대신 살아감으로써 영원히 존재한다. 한 인간을 차지하면 사실상 그 인간은 죽지만, 죽은 인간의 인격과 기억의 파편이 불멸 존재의 인격·기억과 뒤섞여 남는다.

- **The One**(배우 Charlotta Mohlin)은 인간의 **창조성과 예술**에 매혹되어 있다.
- **The Other**(배우 Timothy Lee Depriest)는 인간을 열등한 존재로 경멸한다.

The One은 제2차 세계대전에서 사망한 한 여성을 흡수해 **Marissa Marcel**이 되고, Carl Greenwood에게 깃든 The Other를 화장(火葬)으로 살해한다. 이후 The One은 John의 형상까지 취한다. 1999년에 이르면 두 존재가 동시에 공존하며, The One은 카메라 앞에서 죽음으로써 **"영화적 불멸(cinematic immortality)"** 을 얻고자 한다. 영화 필름에 영원히 새겨지는 것이야말로 불멸이라는, 본작의 테마와 정확히 포개지는 욕망이다.

그리고 이 모든 것의 정점에 **게임의 가장 유명한 장치**가 있다. 클립을 특정 순간에 되감으면, 화면이 일순간 **제4의 벽 너머**로 넘어가 숨겨진 장면이 드러난다. 그 안에서 플레이어는 The One의 얼굴을 마주하게 되고, 마침내 클립들이 채워진 그리드가 서서히 사라지며 The One이 정면을 응시한다. 그녀(그것)는 말한다. **"I'm part of you now(나는 이제 너의 일부야)."** 이는 화면을 응시하던 플레이어 자신이 The One의 새로운 host가 되었음을 암시하는, 게임 매체만이 구사할 수 있는 메타적 충격이다.

### 무드·톤·아트 디렉션

본작의 미학은 철저히 **아날로그 영화 필름**의 물성에 헌정되어 있다. 1968년의 유럽 아트하우스, 1970년의 거칠고 그레인 가득한 뉴욕 누아르, 1999년의 차갑고 광택 있는 비디오 룩까지, 세 영화는 각기 다른 시대의 촬영 양식과 색 보정, 그레인, 필름 흠집을 정교하게 재현한다. 영화는 시간순으로(chronological) 촬영되어 배우들의 연기 성장이 실제로 화면에 새겨졌다.

### 사운드·음악

작곡가 **Nainita Desai**는 세 영화에 각각 대응하는 세 개의 음악 테마를 만들었다. 각 테마는 마리사의 이야기와 그녀가 죽음·필멸성과 대면하는 방식, 그리고 서로 다른 종류의 "마법"을 표상한다. 흥미롭게도 각 테마에는 **전복된 변주(subverted theme)** 가 짝지어져 있는데, 이 변주들은 마법이 사라지거나 실패할 때의 슬픔을 담는다. 사운드트랙은 출시 직전인 2022년 8월 26일 Lakeshore Records를 통해 디지털 발매되었고, 이후 2xLP 바이닐로도 출시되었다.

---

## 3. 핵심 시스템 / 메카닉 — "Match Cut으로 탐험하기"

### 코어 루프: 일시정지하고, 클릭하고, 점프한다

《IMMORTALITY》의 게임플레이는 단순하면서도 전례 없는 형태다. 플레이어는 하나의 클립을 본다. 영상을 일시정지한 뒤, 화면 속의 **인물이나 사물(얼굴·담배·그림·소품·조명 등)** 을 클릭한다. 그러면 게임은 그 이미지가 등장하는 **다른 클립으로 컷(cut)** 한다. 이것이 본작의 심장인 **"exploration by match cut(매치 컷에 의한 탐험)"** 메커니즘이다.

Barlow의 표현을 빌리면, 이것은 **"영화의 마법인 '컷'을 플레이어가 직접 휘두를 수 있는 도구로 만든 것"** 이다. 영화 편집의 핵심 기법인 매치 컷 — 한 장면의 형태·동작·소재가 다음 장면으로 시각적으로 이어지는 — 을 플레이어의 능동적 탐색 행위로 전환했다. 플레이어는 검색창에 단어를 타이핑하는 대신, 화면 속 이미지를 **응시하고 선택하는 것만으로** 자신의 관심사를 표현한다. 특정 인물의 얼굴을 클릭하면 그 배우가 다른 영화·다른 시대에 등장하는 클립으로, 특정 그림을 클릭하면 그 그림이 또 나타나는 클립으로 이동한다.

### 100만 개의 컷 — 손으로 깔 수 없는 그래프

이 시스템의 진정한 기술적 위업은 규모에 있다. Half Mermaid에 따르면, 출시 시점 《IMMORTALITY》에는 **100만 개가 넘는 가능한 컷(cut)** 이 존재한다. 이는 인간 디자이너가 일일이 손으로 연결할 수 있는 양을 압도적으로 초과하는 숫자다. 따라서 어떤 클립의 어떤 객체가 다른 어떤 클립의 객체와 연결되는지는 상당 부분 시스템이 자동으로 결정한다. 그 결과 플레이어는 정해진 정답 경로가 아니라, **자신의 호기심이 이끄는 비선형적이고 개인적인 탐색 여정**을 밟게 된다.

### 제4의 벽과 "되감기"의 발견

표면적 매치 컷 탐색만으로는 게임의 진짜 층위에 도달할 수 없다. 핵심은 영상을 **되감는(rewind)** 행위다. 특정 순간에 영상을 거꾸로 돌리면, 정상 재생에서는 보이지 않던 숨겨진 장면 — The One과 The Other가 등장하는, 제4의 벽을 깨는 시퀀스 — 이 드러난다. 이 "되감기로 숨겨진 진실을 캐낸다"는 발견은 게임이 직접 설명해 주지 않으며, 플레이어가 스스로 깨우쳐야 한다. Barlow는 이에 대해 **"게임플레이가 무언가를 알아내는 것에 관한 것이라면, 플레이어를 신뢰하고 정말 중요한 것들의 일부를 그들이 직접 발견하도록 남겨두어야 한다"** 고 말했다.

### 진행 구조 — 그리드와 클립 컬렉션

전통적인 챕터·레벨·맵 구조는 없다. 대신 플레이어가 발견한 클립들이 **그리드(grid) 형태의 컬렉션**으로 누적된다. 게임은 본편 영화 장면뿐 아니라 미사용 테이크, 리허설, 메이킹 필름, TV 출연·인터뷰 영상까지 모두 탐색 대상으로 제공한다. 진행도는 명시적 퍼센트가 아니라, 플레이어가 모은 파편들이 머릿속에서 하나의 그림으로 맞춰지는 정도로 측정된다. 엔딩 또한 단일하지 않으며, 무엇을 얼마나 발견했느냐에 따라 이해의 깊이가 달라진다.

### UI/UX 디자인 철학 — Moviola와 "Witnessing"

Barlow는 본작의 메타포를 찾는 과정에서 영화 편집기 **Moviola**에 도달했다. 흥미롭게도 그가 밝힌 첫 번째 디자인 문서는 **"Moviola를 든 피카츄" 그림**이었다. 이는 《Pokémon Snap》에서 영감을 받은 것으로, "사냥하거나 싸우는 대신 **응시하고 포착하는(witnessing)** 행위" 자체를 게임 메커니즘으로 삼는다는 발상이었다. Barlow는 GDC 2023 강연에서 본작의 성공이 부분적으로 《Pokémon Snap》의 존재 덕분이라고 농담 섞어 말하기도 했다.

UI는 의도적으로 미니멀하다. 영상을 스크럽(scrub)하는 타임라인, 일시정지·되감기 같은 비디오 컨트롤이 거의 전부다. 플레이어는 마치 실제 편집실에서 필름 릴을 다루듯 직관적으로 영상을 헤집는다.

### 접근성과 멀티

본작은 싱글플레이 전용으로 멀티플레이·협력·라이브 운영·시즌 패스·MTX가 일절 없다. 다만 본작의 비선형 구조와 발견 중심 설계는 자연스럽게 **커뮤니티 협업**을 유도했다 — 플레이어들이 서로 발견한 클립과 해석을 공유하며 집단적으로 미스터리를 풀어나갔다.

---

## 4. 평가

### 평론 점수

《IMMORTALITY》는 평단의 압도적 호평을 받았다.

- **Metacritic:** PC **87/100**, Xbox Series X/S **88/100** ("Generally Favorable~Universal Acclaim" 경계)
- **Edge: 10/10** — 마리사 역 연기를 "outstanding"으로 평하며 만점 부여
- **PC Gamer (US): 95/100**
- **The Guardian: 5/5**
- **Destructoid: 9/10**
- **GameSpot: 8/10**
- **IGN: 8/10**

여러 매체가 본작을 **"Sam Barlow의 magnum opus이자 지금까지 만들어진 최고의 FMV 게임"** 으로 규정했다. GamesRadar+는 "한 편의 아름다운 정신적 충격(one beautiful headf*ck)"이라 표현했다.

### 연기에 대한 찬사 — Manon Gage라는 발견

본작의 평가에서 가장 두드러진 것은 주연 **Manon Gage**의 연기에 대한 거의 만장일치의 극찬이다. 그녀는 Juilliard 졸업 후 3년 만의 복귀작으로, 2021년 초 Zoom 오디션을 통해 캐스팅되었다.

- **Roger Ebert(rogerebert.com):** "a mesmerizing breakout turn(매혹적인 출세작 연기)"
- **The New Yorker:** "subtle, layered performance(섬세하고 다층적인 연기)"
- **Vulture:** "a knockout performance(압도적인 연기)"
- **Vice(Cameron Kunzelman):** "Gage가 마리사를, 그리고 마리사가 연기하는 세 캐릭터를 연기하는 것을 보는 일은, 누군가 외발자전거를 타면서 저글링을 하는 걸 보는 것과 같다 — 그런데 그녀는 그걸 완벽하게 해낸다."

The One을 연기한 **Charlotta Mohlin** 역시 Edge로부터 "remarkable", IGN의 Tristan Ogilvie로부터 "spellbinding(넋을 빼앗는)"이라는 평을 받았다.

### 수상 이력

본작은 2022~2023 시상식 시즌의 주요 수상작이었다.

| 시상식 | 결과 | 부문 |
|---|---|---|
| BAFTA Games Awards 2023 | **수상** | Narrative (Barlow, Gray, Scott) |
| BAFTA Games Awards 2023 | 노미 | Performer in a Leading Role (Gage), Artistic Achievement, Technical Achievement 등 다수 |
| Golden Joystick Awards 2022 | **수상** | Best Performer (Manon Gage) |
| New York Game Awards 2023 | **수상** | Great White Way Award (Best Acting, Gage) |
| Game Developers Choice Awards 2023 | **수상** | Innovation Award |
| Independent Games Festival 2023 | **수상** | Excellence in Narrative |
| The Game Awards 2022 | 노미 | Best Narrative, Best Game Direction, Best Performance(Gage) |
| D.I.C.E. Awards 2023 | 노미 | 다수 부문 |
| Tribeca Festival 2022 | Official Mention | (게임으로는 이례적) |

### 상업·도달 지표

Half Mermaid는 구체적 판매량을 공개하지 않았다. 다만 본작은 **Xbox Game Pass 출시 당일 포함**과 이후 **Netflix Games(모바일) 독점 제공**이라는 두 개의 거대 구독 채널을 통해 광범위한 도달을 확보했다. 이는 작은 인디 스튜디오의 실험적 작품치고는 이례적으로 큰 노출이며, 평론 호평과 결합해 "비평적 성공이 곧 도달 성공으로 이어진" 사례로 평가된다. [추정] 정확한 판매·플레이어 수치는 비공개다.

### 유저 평가와 평론-유저 괴리

Steam 등에서의 유저 반응은 대체로 긍정적이되, 평론만큼 일치된 환호는 아니었다. 일부 플레이어는 비선형 탐색의 모호함과 후반부 초자연적 전환에 당황했고, 매치 컷의 비결정성에 좌절하기도 했다. 즉 본작은 "걸작이라는 데는 동의하지만 모두를 위한 게임은 아니다"라는, 예술 영화에 흔한 종류의 평가 분포를 보였다.

---

## 5. 성공 요인 분석

### (1) 디자인 — 매체의 본질을 메커니즘으로 번역

본작의 가장 큰 성취는 **영화의 문법을 게임의 동사로 변환**한 것이다. 매치 컷이라는 영화 편집 기법을, 플레이어가 직접 휘두르는 탐색 도구로 만들었다. 이는 단순히 신선한 기믹이 아니라, "영화란 무엇인가, 영화 속에 새겨진 인간은 불멸하는가"라는 게임의 주제를 **플레이 행위 그 자체로 체현**하게 만든다. 형식과 내용이 완전히 일치하는, 보기 드문 구조적 우아함이다.

### (2) Barlow의 "3 기둥" 방법론

Barlow는 자신의 모든 프로젝트가 **theme(테마)·emotion(감정)·metaphor(메타포)** 세 가지 기둥의 "sanity check"를 통과해야 한다고 말한다. 세 가지가 모두 갖춰지면 좋은 게임이 된다는 것이다. 《IMMORTALITY》에서 테마는 "예술을 통한 불멸", 감정은 사라진 여배우에 대한 매혹과 연민, 메타포는 "필름에 영원히 새겨지는 존재"다. 이 셋이 한 치의 어긋남 없이 맞물린 점이 작품의 밀도를 만들었다.

### (3) 진짜 영화를 만든다는 결단

Barlow는 게임 안의 "영화"를 흉내 내지 않고, **실제로 세 편의 영화를 끝까지 만들었다.** 《Don't Look Now》의 Allan Scott, 《Lost Highway》의 Barry Gifford 같은 진짜 영화·문학계 거장 작가들을 영입하고, 400페이지 대본을 10주에 걸쳐 시간순으로 촬영했다. 이 "진짜로 만든다"는 진정성이 화면의 설득력을 만들었고, 평단이 본작을 단순한 게임이 아닌 영화 예술로 다루게 만든 토대가 되었다.

### (4) 캐스팅의 성공

Manon Gage라는 신예를 발굴해 세 시대·세 영화·1인 다역이라는 가혹한 연기 과제를 맡긴 도박이 완벽히 적중했다. 그녀의 연기는 본작 평가의 절반을 책임졌다 해도 과언이 아니며, 거의 모든 시상식의 연기 부문에서 수상하거나 노미되었다.

### (5) 타이밍과 유통 전략

FMV 장르는 1990년대 조롱의 대상이었으나, Barlow가 《Her Story》(2015)로 이를 비평적으로 부활시킨 뒤 본작에서 정점을 찍었다. 동시에 **Game Pass·Netflix Games**라는 구독 플랫폼을 통한 무마찰 접근은, 실험적 작품에 대한 진입 장벽을 극적으로 낮췄다. "공짜로 한번 켜 보는" 진입이 입소문을 증폭시켰다.

### (6) 동시기 작품 대비 차별점

2022년은 《Elden Ring》, 《God of War Ragnarök》 등 대작의 해였다. 그 틈에서 《IMMORTALITY》는 **규모가 아니라 형식 혁신**으로 존재감을 확보했다. 어떤 AAA 게임도 흉내 낼 수 없는, 정의상 인디만이 시도할 수 있는 매체 실험이라는 점이 오히려 무기가 되었다.

---

## 6. 비평적 시각 / 한계 / 논란

### 매치 컷의 비결정성

본작 게임플레이 비판의 핵심은 **매치 컷이 무엇을 인식했는지 알려주지 않는다**는 점이다. 예컨대 램프를 클릭하면 의도와 달리 전혀 다른 광원이 등장하는 클립으로 점프하기도 한다. TheGamer는 "Immortality의 매치 컷 시스템에 더 많은 것이 있을 줄 알았다"며 《2001: A Space Odyssey》식의 정교한 형태적 매치를 기대했던 일부 플레이어의 실망을 전했다. 시스템의 광대함이 동시에 통제 불능의 모호함으로 느껴질 수 있다는 양면성이다.

### 초자연적 전환의 호불호

시대극 미스터리로 시작한 작품이 후반부에 흡혈·육체 강탈 존재라는 **초자연 호러로 급격히 선회**하는 데 대한 반응은 갈렸다. Medium의 한 평자(Reno Evangelista)는 "Immortality는 그것이 무엇인지 내게 말해주기 전까지는 흥미로웠다"며, 게임이 모든 것을 초자연적 설정으로 명시해버리는 순간 모호함이 주던 매력이 줄어든다고 비판했다. 즉 "신비를 신비로 남겨두지 않은 것"에 대한 아쉬움이다.

### 누드·성폭력 묘사 논란

본작은 상당량의 **누드와 성적 장면, 그리고 성폭력 묘사**를 담고 있다. 영상을 스크럽하는 플레이 행위 자체가 종종 성적 장면을 헤집게 만드는 구조여서, 일부 평자는 게임이 "착취적 이미지를 비판하는 척하면서 동시에 그 이미지를 전시한다 — 케이크를 가지고도 먹으려 한다(having its cake and eating it)"고 지적했다. 1970년대 "Brit perv" 영화에 대한 Barlow의 애정과, 그것을 비평적으로 다루려는 의도 사이의 긴장이 완전히 해소되지는 않았다는 평이다.

### 주인공·메시지에 대한 소수 비판

Slant Magazine 등 일부 매체는 다수 의견과 달리, 마리사를 "실망스러운 주인공"으로, 일부 구간의 Gage 연기를 "유감스럽게도 단조롭다(one-note)"고 평했다. post-MeToo 시대 할리우드의 착취 구조를 다루는 본작의 코멘터리가 "이미 더 잘 다뤄진 이야기를 상투구로 되풀이한다"는 비판도 있었다. 다만 이는 압도적 호평 속의 소수 의견이다.

### 진입장벽과 친절함의 부재

본작은 튜토리얼이 거의 없고, 핵심 메커니즘(되감기로 숨겨진 진실 발견)을 명시하지 않는다. 이는 발견의 쾌감을 위한 의도된 설계지만, 일부 플레이어는 "무엇을 해야 하는지 몰라" 이탈하기도 했다. "신뢰하는 플레이어"를 전제로 한 설계의 양날이다.

---

## 7. 영향과 유산

### FMV 장르에 대한 의미

《IMMORTALITY》는 Sam Barlow가 《Her Story》(2015) → 《Telling Lies》(2019)로 이어온 **FMV 3부작의 정점**이자, FMV가 1990년대 B급 키치의 잔재가 아니라 **진지한 예술 형식**일 수 있음을 결정적으로 입증한 작품이다. 본작이 받은 BAFTA Narrative, IGF Excellence in Narrative, GDC Innovation Award는 인디·실사 영상 게임이 산업 최고 권위의 인정을 받을 수 있음을 보여주었다.

### 산업적 의미

본작은 두 가지 산업적 메시지를 남겼다. 첫째, **구독 플랫폼(Game Pass·Netflix)이 실험적 인디 작품의 도달을 결정적으로 확장**할 수 있다는 것. 둘째, 게임 개발이 영화·문학계의 진짜 거장(Allan Scott, Barry Gifford)과 협업할 때 매체 간 경계를 허무는 결과물이 나올 수 있다는 것. Tribeca에서 게임이 상영되고 Official Mention을 받은 사실 자체가, 게임과 영화의 제도적 경계가 흔들리고 있음을 상징한다.

### 창작자의 다음 행보

흥미롭게도 Barlow는 본작으로 FMV의 정점을 찍은 뒤, 자신의 이름과 동의어가 된 FMV 3부작을 떠나 **"제대로 된 비디오 게임(proper video games)"** 으로 돌아가겠다고 밝혔다. 그는 게임을 **"불완전한 불멸의 기계(imperfect immortality machines)"** — 즉 창작자의 의도와 플레이어의 발견이 영원히 박제되는 장치 — 로 바라보는 관점을 견지한다. 이는 《IMMORTALITY》의 테마가 그의 창작론 자체와 맞닿아 있음을 보여준다.

### 문화적 의미

본작은 "관객/플레이어가 본다는 행위(witnessing)" 자체를 게임의 핵심 동사로 격상시켰다. 응시하고, 멈추고, 되감고, 연결하는 행위 — 이는 디지털 시대 우리가 영상 콘텐츠를 소비하는 방식 그 자체에 대한 메타적 성찰이기도 하다. 그리고 마지막에 화면이 플레이어를 마주 보며 "나는 이제 너의 일부야"라고 말할 때, 본작은 관음(觀淫)과 소비의 윤리를 플레이어 자신에게 되돌려준다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
|---|---|
| 개발 | Sam Barlow / Half Mermaid Productions |
| 디렉터 | Sam Barlow |
| 작가진 | Sam Barlow, Amelia Gray, Allan Scott, Barry Gifford |
| 작곡 | Nainita Desai |
| 엔진 | Unity |
| 최초 출시 | 2022-08-30 (Windows, Xbox Series X/S, Day 1 Game Pass) |
| 추가 플랫폼 | Netflix(모바일) 2022-11-16, macOS 2023-04-05, PS5 2024-01-23 |
| 주연 | Manon Gage (Marissa Marcel) |
| 가능한 match cut 수 | 100만+ |
| 대본 분량 | 약 400페이지 |
| 촬영 | LA Arts District, 약 10주 (2021-08), 시간순 촬영 |
| Metacritic | PC 87 / Xbox Series 88 |
| 대표 만점 | Edge 10/10, PC Gamer(US) 95, The Guardian 5/5 |
| 주요 수상 | BAFTA Narrative, GDC Innovation, IGF Narrative, Golden Joystick Best Performer |

### 게임 내 세 영화 요약

| 영화 | 연도 | 장르 | 마리사 배역 | 운명 |
|---|---|---|---|---|
| 《Ambrosio》 | 1968 | 고딕 누나스플로이테이션 | Matilda | 감독 Fischer가 네거티브 절도, 미개봉 |
| 《Minsky》 | 1970 | 뉴욕 누아르 탐정극 | Franny | 촬영 중 Carl Greenwood 총기 사망, 미개봉 |
| 《Two of Everything》 | 1999 | 이중성 스릴러 | Maria / Heather (1인 2역) | 마리사 출혈로 쓰러져 제작 중단 |

### 주요 인터뷰·강연

- Sam Barlow, "Breaks down the pillars of interactivity behind Immortality" — Game Developer (theme·emotion·metaphor 3기둥)
- Sam Barlow, GDC 2023 강연 — Moviola 메타포와 《Pokémon Snap》 영감, "witnessing" 메커니즘
- "The path to Immortality" — NME (FMV 부활, 70년대 영국 영화 영향)
- "Inside the mind of Sam Barlow" — The Washington Post 인터뷰
- Nainita Desai 작곡 인터뷰 — Screen Rant, Temple of Geek (세 테마와 전복된 변주)
- Origin Story Podcast — "Games as Imperfect Immortality Machines"

### 참고 자료 목록 (영어권 매체 중심)

- Wikipedia, "Immortality (video game)" — https://en.wikipedia.org/wiki/Immortality_(video_game)
- Metacritic — https://www.metacritic.com/game/immortality/
- OpenCritic — https://opencritic.com/game/13590/immortality
- Unity Blog, "How Half Mermaid designed IMMORTALITY's match cut mechanic" — https://blog.unity.com/games/how-half-mermaid-designed-immortalitys-match-cut-mechanic
- Game Developer, "Sam Barlow breaks down the pillars of interactivity" — https://www.gamedeveloper.com/marketing/sam-barlow-breaks-down-the-pillars-of-interactivity-behind-immortality
- Game Developer, "Why Sam Barlow says 'witnessing' can be a powerful game mechanic"
- NME, "The path to Immortality" — https://www.nme.com/features/the-path-to-immortality-sam-barlow-on-reviving-fmv-games-pokemon-snap-and-70s-brit-perv-filmmakers-3224955
- Roger Ebert, "Immortality review" — https://www.rogerebert.com/video-games/immortality-video-game-review
- Kotaku, "Immortality: The Kotaku Review" — https://kotaku.com/immortality-sam-barlow-horror-video-game-ps5-pc-1849470910
- The Washington Post, "Immortality review" — https://www.washingtonpost.com/video-games/reviews/immortality-game-review/
- GamesRadar+, "Immortality review: One beautiful headf*ck" — https://www.gamesradar.com/immortality-review/
- Slant Magazine, "Immortality Review: A Match to a Kill" — https://www.slantmagazine.com/games/immortality-review-sam-barlow/
- TheGamer, "I Thought There Would Be More To Immortality's Match Cut System" — https://www.thegamer.com/immortality-match-cut-disappointing-2001-a-space-odyssey/
- Screen Rant, "Composer Nainita Desai Interview: Immortality" — https://screenrant.com/immortality-game-composer-nainita-desai-interview/
- BAFTA, Narrative — https://www.bafta.org/games/narrative-0

---

*본 분석서는 영어권 매체·공식 인터뷰·위키 자료를 종합해 작성되었으며, 줄거리 핵심 반전에는 [스포일러] 표기를 두었다. 판매량 등 비공개 수치는 [추정]으로 명시했다.*
