# Just Cause 4 (2018) 심층 분석

> "우리는 역대 최고의 오픈월드 샌드박스를 만들고 싶었고, 물리를 한계까지 밀어붙이고 싶었다." — Francesco Antolini, 게임 디렉터

《Just Cause 4》는 시리즈가 도달한 "장난감 상자(toybox)"로서의 정점인 동시에, 그 장난감을 둘러싼 모든 것 — 이야기, 미션 구조, 비주얼 완성도, 라이브 운영 — 이 어떻게 한 작품을 상업적 실패로 끌어내릴 수 있는지를 보여주는 교과서적 사례다. 이 분석서는 《Just Cause 4》가 무엇을 시도했고, 무엇에서 빛났으며, 어디에서 무너졌는지를 게임 디자인의 관점에서 정밀하게 해부한다. 폭발과 토네이도 같은 "스펙터클"이 어떻게 코어 게임플레이가 될 수 있는지, 그리고 그 스펙터클만으로는 왜 충분하지 않은지를 함께 다룬다.

---

## 1. 게임 개요

### 기본 정보

| 항목 | 내용 |
|------|------|
| 정식 명칭 | 《Just Cause 4》 |
| 개발사 | Avalanche Studios (스웨덴 스톡홀름 / 뉴욕) |
| 퍼블리셔 | Square Enix |
| 장르 | 3인칭 액션 어드벤처 / 오픈월드 샌드박스 |
| 출시일 | 2018년 12월 4일 |
| 플랫폼 | PlayStation 4, Xbox One, Microsoft Windows(PC) |
| 엔진 | APEX 엔진(신버전) |
| 시리즈 | 《Just Cause》 4번째 정식 넘버링 |

(출처: [Wikipedia — Just Cause 4](https://en.wikipedia.org/wiki/Just_Cause_4), [Variety](https://variety.com/2018/gaming/news/just-cause-4-announced-1202839540/))

### 주요 크레딧

- **게임 디렉터: Francesco Antolini** — 《Just Cause 4》의 물리 시뮬레이션과 날씨 시스템을 핵심 비전으로 설정한 인물. 그는 "《Just Cause 3》에서 잃어버렸던 다양성과 발견의 감각을 되찾고 싶었다"고 밝혔다.
- **디자이너: Joe Ishikura**
- **작곡: Zach Abramson**

(출처: [Wikipedia](https://en.wikipedia.org/wiki/Just_Cause_4), [Avalanche Studios — Bring the Thunder](https://avalanchestudios.com/stories/bring-the-thunder))

### 개발사와 시리즈 배경

Avalanche Studios는 2006년 초대 《Just Cause》로 "거대한 오픈월드 + 그래플링 훅 + 무한 폭발"이라는 자사의 정체성을 확립했고, 2010년 《Just Cause 2》로 이 공식을 컬트적 인기로 끌어올렸으며, 2015년 《Just Cause 3》로 그래플링 훅에 무한 테더(tether)와 윙슈트를 더해 시리즈 메카닉의 완성형에 근접했다. 그러나 《Just Cause 3》는 출시 당시 콘솔 버전의 심각한 프레임 드랍과 긴 로딩으로 기술적 평판에 타격을 입었다.

《Just Cause 4》는 이 기술적 부채를 청산하고 시리즈를 한 단계 도약시키기 위해, Avalanche가 자체 개발한 신형 **APEX 엔진**을 전면에 내세웠다. APEX의 핵심 자랑거리는 단 하나, **"역대 비디오게임에서 본 적 없는 극한의 날씨 시뮬레이션"**이었다. 토네이도, 모래폭풍, 눈보라, 폭우를 완전히 물리화(fully physicalized)하여 게임플레이에 실제로 영향을 주도록 만든다는 것이 4편의 출발점이자 마케팅의 전부였다.

(출처: [PlayStation LifeStyle — Apex Engine Dev Diary](https://www.playstationlifestyle.net/2018/07/19/just-cause-4-apex-engine-video/), [TweakTown](https://www.tweaktown.com/news/62461/cause-4s-sandbox-aims-biggest/index.html))

### 엔진/기술 스택

APEX 엔진은 다음을 가능케 한다고 설명되었다.

- **바람과 파티클 시스템**이 플레이어의 이동(traversal)에 직접 영향을 줌
- **체적 구름(volumetric clouds)** 과 동적 기상
- **더 정교한 파괴(destruction)** 와 물리 시뮬레이션
- 풍속·기압을 변수로 한 토네이도/사이클론의 실시간 물리 연산

디렉터 Antolini는 "역대 최대 규모의 샌드박스"를 목표로 솔리스(Solís)라는 약 1,024㎢ 규모의 맵을 설계했다고 밝혔다. 그러나 후술하듯, 이 야심찬 엔진 비전은 출시 시점 **비주얼 완성도(특히 텍스처·물 표현)의 후퇴**라는 역설적 결과로 이어졌다.

(출처: [GameSpot — Lethal Weather Demo](https://www.gamespot.com/articles/just-cause-4s-demo-showcases-its-extremely-lethal-/1100-6459626/))

---

## 2. 게임 설명

### 컨셉

《Just Cause 4》는 한 문장으로 요약하면 **"중력과 물리 법칙을 무기로 쓰는 1인 군대(army of one) 시뮬레이터"**다. 플레이어는 시리즈의 영원한 주인공 **Rico Rodríguez(리코 로드리게스)**가 되어, 그래플링 훅·윙슈트·낙하산이라는 3종 이동 도구와, 거기에 부착하는 **테더(tether)·리트랙터(retractor)·부스터(booster)·에어 리프터(air lifter, 풍선)** 라는 물리 장난감을 조합해 독재 정권의 인프라를 산산조각 낸다. 명확한 서사적 목표(정권 타도)가 있지만, 게임의 진짜 본질은 "이 장난감들로 무엇을 부술 수 있는가"라는 창발적 실험에 있다.

### 세계관과 무대: 솔리스(Solís)

무대는 가공의 남미 국가 **솔리스(Solís)**다. 솔리스는 단일 맵 안에 우림·초원·고산·설원·사막을 모두 품은 극단적 지리를 가지며, 무엇보다 **세계에서 가장 변덕스럽고 치명적인 날씨**를 자랑한다. 사막 지대에는 모래폭풍이, 고산 지대에는 눈보라가, 평원에는 거대한 토네이도가 상시 발생한다. 이 날씨는 단순한 배경이 아니라 게임의 주제 그 자체다 — 솔리스의 폭정은 곧 **날씨를 무기화한 폭정**이기 때문이다.

(출처: [Just Cause Wiki — Just Cause 4](https://justcause.fandom.com/wiki/Just_Cause_4), [TV Tropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/JustCause4))

### 줄거리 [스포일러 포함]

《Just Cause 3》의 사건 이후, 리코는 솔리스 출신 여성 **Mira Morales(미라 모랄레스)**로부터 충격적인 증거를 받는다. 리코의 죽은 아버지 **Miguel Rodríguez(미겔 로드리게스)**가 생전에 **일라파 프로젝트(Illapa Project)** — 날씨를 통제하는 기상 병기 — 에 관여했다는 것이다. [스포일러] 일라파는 본래 미겔과 동료들, 그리고 **Leon Espinosa(레온 에스피노사)**가 "사람들의 이익을 위해 날씨를 통제한다"는 선의로 시작한 연구였다.

그러나 레온이 급사한 뒤, 그의 아들 **Oscar Espinosa(오스카 에스피노사)**가 프로젝트를 장악한다. 오스카는 아버지가 가문의 재산을 낭비한다고 여겼고, 일라파를 최고 입찰자에게 팔 무기로 전용하려 했다. 이에 환멸을 느낀 미겔은 프로젝트를 떠나지만, 오스카는 (《Just Cause 3》의 메디치 독재자 Sebastiano Di Ravello와 Agency 내부 연줄을 이용해) 미겔을 살해한다.

리코는 아버지의 진실과 솔리스 해방을 위해, 시리즈 전통의 저항군 **'Army of Chaos(혼돈의 군대)'**를 다시 조직한다. 적은 세계 최강의 민간 군사 기업 **Black Hand(블랙 핸드)**이며, 이를 이끄는 인물이 새 등장인물 **Gabriela Morales(가브리엘라 모랄레스)**다. [스포일러] 가브리엘라는 리코의 "어두운 거울상(dark reflection)"으로 설계되었다 — 그녀 역시 유능하고 거침없으나, 결국 오스카가 자신의 이익을 위해 블랙 핸드 병력을 소모품처럼 희생시킨다는 것을 깨닫고 그에게 등을 돌린다.

(출처: [Wikipedia](https://en.wikipedia.org/wiki/Just_Cause_4), [Just Cause Wiki — Gabriela Morales](https://justcause.fandom.com/wiki/Gabriela_Morales), [Destructoid — Gabriela Morales 인터뷰](https://www.destructoid.com/just-cause-4-villain-gabriela-morales-is-ricos-dark-reflection/))

### 주요 캐릭터

- **Rico Rodríguez** — 시리즈의 변함없는 주인공. 라틴계 액션 히어로의 전형으로, 이번엔 아버지의 유산이라는 개인사가 더해졌다.
- **Gabriela Morales** — 블랙 핸드 사령관. 리코의 라이벌이자 대칭점. 서사적으로 가장 흥미로운 신규 캐릭터로 의도되었다.
- **Mira Morales** — 솔리스 토박이로 리코의 조력자. (가브리엘라와 성이 같으나 직접적 혈연 관계는 서사에서 핵심이 아니다.)
- **Oscar Espinosa** — 일라파를 무기화한 독재 정권의 수장. 전형적 악당.
- **Army of Chaos 멤버들** — Luis "Sargento", Izzy, Garland King, Javi Huerta 등 저항군 동료.

### 무드/톤/아트 디렉션

시리즈는 일관되게 **"진지함을 거부하는 B급 액션 영화"**의 톤을 유지한다. 리코는 헬리콥터 위에서 윙슈트로 뛰어내려 적 기지를 풍선으로 하늘에 띄우는 동안에도 결코 비장하지 않다. 남미를 모티프로 한 화려한 색감, 폭발의 오렌지빛, 그리고 토네이도의 회색 소용돌이가 시각적 대비를 이룬다. 다만 4편의 아트 디렉션은 "스펙터클의 야심"과 "텍스처 디테일의 후퇴"가 충돌하는 지점에서 평가가 갈렸다(6장 참조).

### 사운드/음악

작곡은 **Zach Abramson**이 맡았다. 사운드트랙은 라틴 퍼커션과 오케스트라, 액션 신스를 결합한 트랙들로, 토네이도·폭발의 카오스에 박진감을 더한다. 음악은 평론에서 게임의 강점 중 하나로 자주 거론되었으며, 본작은 **G.A.N.G. Awards의 Best Original Instrumental** 부문 후보에 올랐다.

(출처: [Wikipedia](https://en.wikipedia.org/wiki/Just_Cause_4))

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

《Just Cause 4》의 진짜 게임은 서사가 아니라 **그래플링 훅의 모듈식 물리 시스템**에 있다. 이 챕터를 가장 깊게 다루는 이유는, 본작의 모든 성취와 한계가 여기에서 출발하기 때문이다.

### 코어 게임플레이 루프 (모먼트-투-모먼트)

1. **이동(Traversal)** — 그래플링 훅으로 표면을 당겨 자신을 끌어올린다 → 낙하산을 펼친다 → 윙슈트로 활공한다. 이 3종 도구는 매끄럽게 연결되어, 숙련된 플레이어는 땅에 발을 거의 대지 않고 맵 전체를 누빈다. 4편에서는 **바람(기류, air flow)을 타고 윙슈트로 그래플 없이 체공**할 수 있게 되어, 이동의 유려함이 한층 강화되었다.
2. **카오스 유발(Chaos)** — 적 기지·정유소·통신탑·동상 등 "파괴 가능한 오브젝트"를 부순다. 시리즈 전통의 "빨간색=폭발물" 시각 언어가 유지된다.
3. **테더 실험(Tether Play)** — 여기가 4편의 정수다. 두 오브젝트를 케이블로 묶어 충돌시키거나, 풍선으로 띄우거나, 부스터로 날려버린다.
4. **반복** — 위 루프를 무한히 변주하며 영토를 해방한다.

(출처: [GamesRadar — 핸즈온 프리뷰](https://gamesradar.com/uk/just-cause-4-hands-on-preview), [Square Enix — 윙슈트 팁](https://www.square-enix-games.com/en_US/news/just-cause-4-wingsuit-tips))

### 그래플링 훅: 모듈식 물리 장난감 시스템

4편의 가장 큰 메카닉적 혁신은 그래플링 훅에 **세 가지 모듈식 부착물**을 추가하고, 이를 **로드아웃(loadout)으로 커스터마이즈**할 수 있게 한 것이다.

- **리트랙터(Retractor)** — 강력한 모터 달린 테더. 부착한 두 대상을 극단적인 힘으로 서로 끌어당긴다. 적 병사를 폭발 배럴에 묶어 충돌시키거나, 헬리콥터를 지면에 박아버리는 식.
- **에어 리프터(Air Lifter, 풍선)** — 부착한 대상에 강력한 풍선을 달아 공중으로 띄운다. 군용 지프조차 하늘로 올릴 수 있고, 여러 개를 부착하면 양력이 가산된다. 상승 고도, 정점에서의 동작(호버 / 폭발), 풍선의 내구도까지 세밀하게 설정 가능하다.
- **부스터(Booster)** — 부착한 대상에 마이크로 제트 엔진을 달아 미친 듯한 속도로 날려버린다. 차량을 미사일처럼 발사하거나, 적 탱크를 스스로 회전시켜 파괴할 수 있다.

핵심은 이 세 효과를 **단일 테더에 중첩(stack)** 할 수 있다는 점이다. 예컨대 "풍선으로 띄우면서 부스터로 회전시키고, 정점에서 폭발"하는 식의 복합 장치를 만들 수 있다. 동시에 **최대 10개의 테더**를 발사할 수 있고, 개별 해제 또는 일괄 해제가 가능하다. 또한 **3개의 로드아웃 슬롯**을 두어 전투 중 실시간으로 셋업을 전환할 수 있다.

이 시스템의 디자인 철학은 명확하다: **개발자가 정해둔 "옳은 플레이"를 제거하고, 플레이어를 물리 엔진의 작가로 만드는 것.** 풍선 + 부스터 + 리트랙터의 순열 조합은 사실상 무한하며, 유저들은 이를 이용해 발사형 폭탄, 인간 새총, 공중 회전목마 같은 자작 메카닉을 만들어냈다.

(출처: [GameWith — Gadgets & Grappling Hook Upgrades](https://gamewith.net/justcause4/article/show/2073), [PCGamesN — 차에 풍선 매달기](https://www.pcgamesn.com/just-cause-4/just-cause-4-grappling-hook), [Just Cause Wiki — Airlifter mods](https://justcause.fandom.com/wiki/Airlifter_mods))

### 진행 구조: 프론트라인(Frontline) 팩션 시스템

4편은 시리즈의 영토 해방을 **프론트라인(Frontline)이라는 줄다리기식 전선 시스템**으로 재설계했다. 솔리스 맵은 여러 지역(region)으로 나뉘며, 각 지역은 블랙 핸드와 Army of Chaos가 영토를 두고 다투는 전선으로 표현된다.

- 플레이어가 카오스를 일으키고 거점을 점령하면 **Army of Chaos의 병력(squad)이 증가**하고, 전선이 적진으로 밀려난다.
- 새 지역을 해방하려면 일정량의 카오스/스쿼드가 필요하다 — 이것이 진행의 게이팅 역할을 한다.
- 전선이 밀리면 **AI 동료 병력**이 플레이어를 따라 전투에 가담한다.

이 시스템은 전작들의 "퍼센티지 청소(맵의 모든 오브젝트를 부수기)"보다 목적 지향적이지만, 동시에 "카오스 유발 → 스쿼드 충전 → 전선 밀기"의 반복이 후반부에 단조로워진다는 비판도 받았다.

(출처: [Wikipedia](https://en.wikipedia.org/wiki/Just_Cause_4), [GameSpot 리뷰](https://www.gamespot.com/reviews/just-cause-4-review-mildly-wild-ride/1900-6417049/))

### 날씨: 코어 메카닉으로서의 기상

APEX 엔진이 자랑한 **물리화된 날씨**는 단순 연출이 아니라 게임플레이 변수다.

- **토네이도** — 4편의 시그니처. 차량·구조물·적·심지어 리코까지 빨아들이는 거대한 물리 소용돌이. 평론가들조차 "토네이도 시스템은 예술 작품(a work of art)"이라 인정했다. 특정 스토리 미션은 토네이도 한가운데를 돌파하는 스펙터클로 구성된다.
- **모래폭풍/눈보라** — 시야를 가리고 이동을 방해하며, 일라파 병기로 인공적으로 발생시킬 수 있다.
- **번개 폭풍** — 후술할 번개건과 연계된다.

이 날씨는 솔리스의 정권이 일라파로 "날씨를 무기화"했다는 서사와 메카닉을 결합시키는 장치다. 다만 토네이도를 제외한 대부분의 날씨는 "구경거리"에 머물고 게임플레이 깊이로 충분히 전환되지 못했다는 지적이 있다.

(출처: [PlayStation LifeStyle — Tornado Trailer](https://www.playstationlifestyle.net/2018/08/20/just-cause-4-gameplay-trailer-tornado/), [GameSpot](https://www.gamespot.com/articles/just-cause-4s-demo-showcases-its-extremely-lethal-/1100-6459626/))

### 이색 무기와 보급 시스템

- **윈드 건(Wind Gun)** — 압축 공기로 적을 날려버리는 무기. 대체 발사 모드 보유.
- **라이트닝 건(Lightning Gun)** — 번개를 유도/발사하는 이색 무기.
- **보급 드랍(Supply Drop)** — 시리즈 전통대로, 무기·차량을 전장에 즉시 호출하는 시스템. 진척에 따라 호출 가능 목록이 확장된다.

### 난이도/접근성과 UI/UX

본작은 표준적인 난이도 옵션을 제공하지만, 접근성 측면에서 특별히 주목받지는 못했다. 오히려 **UI/UX는 본작의 약점**으로 거듭 지적되었다 — 메뉴 구조가 번잡하고 정보 전달이 비효율적이라는 평이 많았다. "끔찍한 UI(terrible UI)"라는 표현이 유저 리뷰에 반복적으로 등장한다.

(출처: [COGconnected 리뷰](https://cogconnected.com/review/just-cause-4-review/), [Metacritic 유저 리뷰](https://www.metacritic.com/game/just-cause-4/user-reviews/))

---

## 4. 평가

### Metacritic / OpenCritic

| 플랫폼 | Metacritic 점수 | 평가 |
|--------|----------------|------|
| Xbox One | 70 / 100 | 혼합~평균 |
| PC | 68 / 100 | 혼합~평균 |
| PlayStation 4 | 65 / 100 | 혼합~평균 |

전체적으로 "혼합 또는 평균(mixed or average)" 평가를 받았다. 오픈월드 게임플레이·조작감·물리·사운드트랙은 호평받았으나, **이야기·미션 디자인·컷신·성우 연기·UI·기술적 완성도**가 비판의 표적이 되었다.

(출처: [Metacritic — Just Cause 4](https://www.metacritic.com/game/just-cause-4/), [OpenCritic](https://opencritic.com/game/6220/just-cause-4))

### 주요 평론 점수

| 매체 | 점수 |
|------|------|
| IGN | 7.9 / 10 |
| Game Informer | 8 / 10 |
| PC Gamer (US) | 73 / 100 |
| GameSpot | 6 / 10 |
| Eurogamer | "Recommended" |

**IGN(7.9)**은 그래플링 훅의 창의적 자유와 이동의 즐거움을 높이 샀다. **Game Informer(8)**도 샌드박스의 카오스를 긍정했다. 반면 **GameSpot(6)**의 리뷰 제목은 "Mildly Wild Ride(적당히 거친 놀이기구)"로, "기발한 도구는 즐겁지만 그것을 둘러싼 미션과 세계가 그 잠재력을 살리지 못한다"는 취지였다. **COGconnected**는 더 가혹하게 "An Explosive Mess(폭발적인 엉망진창)"라 평했다.

(출처: [IGN 리뷰 via N4G](https://n4g.com/news/2223483/just-cause-4-review-ign), [GameSpot 리뷰](https://www.gamespot.com/reviews/just-cause-4-review-mildly-wild-ride/1900-6417049/), [COGconnected](https://cogconnected.com/review/just-cause-4-review/))

### 상업 지표

《Just Cause 4》는 **상업적으로 명백한 실패**였다.

- **개발비 회수 실패**: Square Enix는 본작의 판매가 개발 비용을 충당하지 못했다고 명시했다. 사장 Yosuke Matsuda는 2018년 회사의 저조한 영업이익의 중요한 원인으로 《Just Cause 4》의 부진을 직접 지목했다.
- **전작 대비 급락**: 출시 직후 물리(패키지) 판매량이 《Just Cause 3》 대비 **약 61.5% 감소**했고, 대략 50만 장가량 적게 팔렸다.
- **영국 차트**: 출시 주 영국 차트에서 고전했다.
- **일본**: PS4판 첫 주 16,100장으로 전체 차트 7위.

Square Enix는 부진의 주된 이유로 **"동시기 출시된 다른 AAA 타이틀과의 경쟁"**과 **"유저가 자사 게임을 선택할 만큼 충분히 새로운 경험을 제공하지 못한 것"**을 들었다. 같은 분기 《Shadow of the Tomb Raider》와 함께 "약하고 기대 이하(weak and below expectations)"로 묶여 보고되었다.

(출처: [DSOGaming](https://www.dsogaming.com/news/just-cause-4-performed-below-expectations-we-sold-fewer-units-on-launch-than-we-had-anticipated/), [WCCFtech](https://wccftech.com/tomb-raider-just-cause-4-weak-below-expectations/), [TweakTown](https://www.tweaktown.com/news/64921/cause-4-sales-fail-square-enix-blames-aaa-titles/index.html), [Wikipedia](https://en.wikipedia.org/wiki/Just_Cause_4))

### 수상 이력

- **2019 Webby Awards** — Action Game 부문 **수상**
- **2019 NAVGTR Awards** — Control Design, Franchise Adventure 부문 후보
- **2019 G.A.N.G. Awards** — Best Original Instrumental 부문 후보

본작의 수상이 주로 "조작/컨트롤"과 "음악"에 집중된 점은 시사적이다 — 즉, 평단조차 본작의 강점이 **메카닉과 사운드**에 있고 서사·연출에 있지 않다고 본 것이다.

(출처: [Wikipedia](https://en.wikipedia.org/wiki/Just_Cause_4))

### 평론-유저 괴리

평론(60대 후반~70대)과 유저 평가 사이에는 흥미로운 괴리가 있다. 코어 팬층은 그래플링 훅 시스템의 자유도와 토네이도 스펙터클을 높이 평가하며 "역대 최고의 샌드박스 도구"라 부르는 반면, 다수 유저 리뷰는 **비주얼 후퇴·UI·빈약한 미션·기술 문제**를 들어 실망을 표했다. 결과적으로 본작은 "좋아하는 사람은 깊게 좋아하지만, 폭넓은 대중을 설득하지 못한" 전형적 니치 작품의 평가 곡선을 그렸다.

---

## 5. 성공 요인 분석 — 그리고 그 한계

《Just Cause 4》는 상업적으로 실패했으므로, 이 챕터는 "왜 성공했는가"보다 **"무엇이 성공할 자질을 가졌고, 왜 그것이 성공으로 전환되지 못했는가"**를 분석하는 것이 정직하다.

### 디자인 측면의 강점 (성공 자질)

1. **모듈식 물리 장난감의 완성** — 리트랙터·풍선·부스터를 단일 테더에 중첩하고 로드아웃으로 커스터마이즈하는 시스템은, 시리즈가 10년 넘게 다듬어온 "그래플링 훅 샌드박스"의 논리적 정점이다. 이는 *Garry's Mod*, *Teardown* 같은 "물리 창작 도구" 계열의 즐거움을 메인스트림 액션게임에 이식한 것으로, 본질적으로 강력한 디자인 자산이다.
2. **토네이도 = 메카닉화된 스펙터클** — 완전 물리화된 토네이도는 당시 어떤 오픈월드 게임도 보여주지 못한 기술적 쇼케이스였다. "날씨를 무기화한 독재"라는 서사와 메카닉을 묶은 발상도 영리했다.
3. **이동의 유려함** — 그래플 + 낙하산 + 윙슈트 + 기류 활공의 연계는 시리즈 최고 수준으로 매끄러웠다.

### 왜 성공으로 전환되지 못했나

1. **출시 타이밍의 자멸** — 2018년 12월은 《Red Dead Redemption 2》, 《Spider-Man》, 《Assassin's Creed Odyssey》 등 그 해 최강의 AAA들이 쏟아진 직후였다. Square Enix 스스로 "다른 AAA와의 경쟁"을 패인으로 꼽았다.
2. **"충분히 새롭지 않다"는 인식** — 퍼블리셔조차 인정했듯, 핵심 루프(폭발·해방·반복)는 《Just Cause 2》(2010) 이래 본질적으로 동일하다. 토네이도와 모듈 테더는 멋졌으나, 시리즈에 무관심하던 대중을 새로 끌어올 "결정적 새로움"으로 인식되지 못했다.
3. **비주얼 후퇴라는 치명적 첫인상** — 신엔진을 내세웠음에도, 출시판은 3년 전 《Just Cause 3》보다 물·텍스처·폭발 디테일에서 후퇴한 것으로 비교 영상에 적나라하게 드러났다. "신기술"을 마케팅하고 "구작보다 못한 비주얼"을 내놓은 모순은 신뢰에 직격탄이었다.
4. **장난감을 담을 그릇의 부재** — 도구는 천재적인데, 그 도구를 의미 있게 쓰게 만드는 미션·세계·서사가 빈약했다. "기발한 장치를 만들어도 그것을 쓸 흥미로운 이유가 없다"는 것이 다수 평론의 공통된 결론이었다.

### 비교: 동시기 작품 대비

같은 "물리·파괴·이동의 쾌감"을 파는 작품으로 《Saints Row IV》, 후일의 《Teardown》(2020), 《Rage 2》(2019, 역시 Avalanche 공동개발) 등이 있다. 《Just Cause 4》는 "도구의 깊이"에서는 이들을 능가했으나, "콘텐츠의 밀도와 연출의 다듬음"에서 동시기 AAA들에 명백히 뒤처졌다. 즉 본작의 실패는 **아이디어의 실패가 아니라 패키징과 마감의 실패**였다.

(출처: [TweakTown](https://www.tweaktown.com/news/64921/cause-4-sales-fail-square-enix-blames-aaa-titles/index.html), [Gamepur — 그래픽 다운그레이드 비교](https://www.gamepur.com/news/just-cause-4-vs-just-cause-3-graphics-downgrade))

---

## 6. 비평적 시각 / 한계 / 논란

### 디자인적 약점

- **반복성** — 프론트라인 시스템은 "카오스 유발 → 스쿼드 충전 → 전선 밀기"의 단조로운 사이클로 귀결되어, 후반부 동기 부여가 급격히 빠진다.
- **장난감과 목적의 괴리** — 가장 자주 인용된 비판. 그래플 시스템은 무한히 창의적인데, 게임은 그 창의성을 "필요"로 만드는 설계(퍼즐, 도전, 보상)를 거의 제공하지 않는다. 유저들이 직접 동기를 만들어야 한다.
- **빈약한 적 AI와 전투** — 도구의 화려함에 비해 적의 반응과 전투 깊이는 단순하다.

### 기술적 논란: 비주얼 다운그레이드

본작의 가장 큰 출시 논란은 **그래픽 후퇴**다. 신형 APEX 엔진을 대대적으로 홍보했음에도, 출시판은 다음에서 전작·동세대 작품에 못 미쳤다.

- **물 표현**: "어이없을 만큼 형편없는(laughably poor)" 물 효과. 3년 전 《Just Cause 3》보다도 명백히 나쁘다는 비교가 확산됐다.
- **텍스처**: 극도로 흐릿한 텍스처.
- **폭발**: 시리즈의 간판인 폭발조차 전작보다 디테일이 떨어진다는 평.
- **콘솔 성능**: PS4 Pro·Xbox One X에서도 "눈에 띄는 다운그레이드"로 분석됐다.

역설은, **토네이도와 날씨 시스템만은 진짜로 인상적**이었다는 점이다. 즉 엔진의 연산 자원이 날씨 시뮬레이션에 집중되면서 정작 일상적 비주얼(텍스처·물)이 희생된 듯한 인상을 준다.

(출처: [Gamepur](https://www.gamepur.com/news/just-cause-4-vs-just-cause-3-graphics-downgrade), [GamingBolt — 플랫폼 비교](https://gamingbolt.com/just-cause-4-ps4-pro-vs-xbox-one-x-vs-pc-comparison-a-noticeable-downgrade), [TechSpot 벤치마크](https://www.techspot.com/review/1762-just-cause-4-benchmarks/))

### 서사의 한계

이야기는 "시리즈 최저 수준 중 하나"라는 평가를 받았다. 가브리엘라 모랄레스를 "리코의 거울상"으로 야심차게 설계했음에도, 컷신 연출·성우 연기·페이싱이 이를 살리지 못했다. 유저 리뷰는 "주 스토리가 프랜차이즈에 아무것도 더하지 못한다(adds almost nothing to the franchise)"고 혹평했다. 본작은 결국 **"서사를 보러 오는 게임이 아니다"**라는 시리즈의 정체성을 재확인시켰을 뿐이다.

### 라이브 운영/DLC 논란

출시 후 세 개의 유료 확장팩이 나왔으나 반응은 엇갈렸다.

- **Dare Devils of Destruction** (2019.4.30) — 무기화 차량·도전 모드. **가장 부정적** 평가. "포인트-투-포인트 레이스만 괜찮고 나머진 별로"라는 평이 지배적.
- **Los Demonios** (2019.7.3) — 악마적 식물·생물 침공 미션. **창의적이고 독특하다는 호평**. "이상한 식물과 생물을 부수는 게 만족스럽다"는 반응.
- **Danger Rising** (2019.9.5) — Agency 미션 8종과 파괴용 장난감, 특히 **호버보드** 추가. "정작 본편보다 더 많은 걸 부술 수 있어 즐겁다"는, 본편을 향한 역설적 칭찬을 받았다.

DLC 전반은 "세일 때 사라"는 정도의 평가로, 본작의 부진한 상업 성과를 만회하지는 못했다.

(출처: [Just Cause Wiki — DLC](https://justcause.fandom.com/wiki/Downloadable_content_for_Just_Cause_4), [Game Informer — Danger Rising](https://gameinformer.com/dlc/2019/08/08/just-cause-4-danger-rising-dlc-gets-release-date-in-bombastic-new-trailer), [Windows Central — Los Demonios](https://www.windowscentral.com/just-cause-4-los-demonios-dlc-worth-it))

### 평가가 갈리는 지점

본작에 대한 평가는 결국 **"무엇을 게임의 본질로 보는가"**에 달려 있다. "장난감 상자"를 본질로 보는 플레이어에게 4편은 시리즈 최고작이다. "잘 만든 액션 어드벤처 패키지"를 기대한 플레이어에게는 시리즈 최악 중 하나다. 이 양극성이 본작의 정체성이다.

---

## 7. 영향과 유산

### 장르와 시리즈에 미친 영향

《Just Cause 4》는 **"물리 시뮬레이션을 코어 마케팅 포인트로 내세운 AAA"**의 한 사례로 남았다. 완전 물리화된 토네이도는 이후 게임들이 동적 날씨를 단순 연출이 아닌 게임플레이 변수로 진지하게 고민하게 만든 기술적 레퍼런스가 되었다.

동시에 본작은 **반면교사**로서 더 큰 교훈을 남겼다: **"기술적 야심(엔진·날씨)을 비주얼 기본기(텍스처·물) 희생으로 사면 출시 첫인상에서 자멸한다"**는 것, 그리고 **"창발적 도구는 그것을 의미 있게 쓰게 만드는 콘텐츠 그릇이 없으면 빈 장난감으로 남는다"**는 것이다. 이 두 교훈은 이후 물리 샌드박스 디자인 논의에서 반복 인용된다.

### 시리즈의 향방

《Just Cause 4》의 상업적 실패는 시리즈 자체에 무거운 그림자를 드리웠다. 개발비 회수 실패가 퍼블리셔 영업이익에 직접 타격을 줬다는 공식 인정은, 이후 시리즈가 새 정식 넘버링을 받기까지 오랜 공백을 겪는 한 배경이 되었다. Avalanche Studios는 이후 《Rage 2》(2019) 등 다른 프로젝트로 전환했다.

### 산업적/문화적 의미

- **산업적**: 본작은 "연말 AAA 격전기에 차별화 없이 출시한 중견 IP의 위험"을 보여주는 케이스 스터디다. Square Enix가 패인을 공개적으로 분석한 보기 드문 사례라는 점에서, 퍼블리싱 전략 논의의 자료로 가치가 있다.
- **문화적**: 그럼에도 《Just Cause 4》는 "풍선으로 소를 하늘에 띄우고, 부스터로 차를 발사하는" 유튜브/스트리밍 클립 문화의 단골 소재로 살아남았다. 게임의 진지한 평가와 별개로, **"창발적 카오스 클립의 공급원"**으로서의 문화적 수명은 결코 짧지 않았다. 이는 본작의 메카닉이 실제로 유효했음을 역설적으로 증명한다.

---

## 8. 부록

### 핵심 통계 표

| 지표 | 수치/내용 |
|------|----------|
| 출시일 | 2018년 12월 4일 |
| 플랫폼 | PS4, Xbox One, PC |
| Metacritic | Xbox One 70 / PC 68 / PS4 65 |
| IGN | 7.9 / 10 |
| GameSpot | 6 / 10 |
| Game Informer | 8 / 10 |
| 전작 대비 물리 판매 | 약 -61.5% |
| 전작 대비 추정 판매 격차 | 약 -50만 장 |
| 일본 PS4 첫 주 | 16,100장 (전체 7위) |
| DLC | Dare Devils of Destruction, Los Demonios, Danger Rising |
| 주요 수상 | 2019 Webby Awards Action Game 부문 수상 |

### 핵심 메카닉 요약 표

| 도구 | 기능 |
|------|------|
| 리트랙터(Retractor) | 두 대상을 강력히 끌어당기는 모터 테더 |
| 에어 리프터(Air Lifter) | 풍선으로 대상을 공중에 띄움(고도/폭발/내구도 설정 가능) |
| 부스터(Booster) | 마이크로 제트로 대상을 가속/발사 |
| 윙슈트 | 기류를 타고 그래플 없이 체공 가능 |
| 테더 중첩 | 단일 테더에 세 효과 스택, 최대 10개 동시 운용, 로드아웃 3슬롯 |

### 주요 인터뷰 / 개발 자료

- Avalanche Studios, "Bring the Thunder" (APEX 엔진·날씨 시스템 개발기) — https://avalanchestudios.com/stories/bring-the-thunder
- PlayStation LifeStyle, "Apex Engine Dev Diary" — https://www.playstationlifestyle.net/2018/07/19/just-cause-4-apex-engine-video/
- GameRevolution, 내러티브 디렉터 인터뷰 — https://www.gamerevolution.com/originals/433711-we-talked-to-just-cause-4s-narrative-director-about-the-games-story-the-sexy-grappling-hook-and-more-interview
- Destructoid, 가브리엘라 모랄레스 캐릭터 인터뷰 — https://www.destructoid.com/just-cause-4-villain-gabriela-morales-is-ricos-dark-reflection/

### 참고 자료 목록 (영어권 매체 중심)

- [Wikipedia — Just Cause 4](https://en.wikipedia.org/wiki/Just_Cause_4)
- [Variety — Just Cause 4 Comes Out December 4](https://variety.com/2018/gaming/news/just-cause-4-announced-1202839540/)
- [Metacritic — Just Cause 4](https://www.metacritic.com/game/just-cause-4/)
- [OpenCritic — Just Cause 4](https://opencritic.com/game/6220/just-cause-4)
- [GameSpot — "Mildly Wild Ride" 리뷰](https://www.gamespot.com/reviews/just-cause-4-review-mildly-wild-ride/1900-6417049/)
- [IGN 리뷰 (via N4G)](https://n4g.com/news/2223483/just-cause-4-review-ign)
- [COGconnected — "An Explosive Mess"](https://cogconnected.com/review/just-cause-4-review/)
- [DSOGaming — 판매 부진 보도](https://www.dsogaming.com/news/just-cause-4-performed-below-expectations-we-sold-fewer-units-on-launch-than-we-had-anticipated/)
- [WCCFtech — 약한 판매 분석](https://wccftech.com/tomb-raider-just-cause-4-weak-below-expectations/)
- [TweakTown — Square Enix의 패인 분석](https://www.tweaktown.com/news/64921/cause-4-sales-fail-square-enix-blames-aaa-titles/index.html)
- [Gamepur — JC4 vs JC3 그래픽 다운그레이드](https://www.gamepur.com/news/just-cause-4-vs-just-cause-3-graphics-downgrade)
- [GamingBolt — 플랫폼 비교](https://gamingbolt.com/just-cause-4-ps4-pro-vs-xbox-one-x-vs-pc-comparison-a-noticeable-downgrade)
- [TechSpot — PC 그래픽 벤치마크](https://www.techspot.com/review/1762-just-cause-4-benchmarks/)
- [GamesRadar — 핸즈온 프리뷰](https://gamesradar.com/uk/just-cause-4-hands-on-preview)
- [PCGamesN — 그래플링 훅 기능](https://www.pcgamesn.com/just-cause-4/just-cause-4-grappling-hook)
- [GameWith — Gadgets & Grappling Hook Upgrades](https://gamewith.net/justcause4/article/show/2073)
- [Just Cause Wiki — Just Cause 4](https://justcause.fandom.com/wiki/Just_Cause_4)
- [Just Cause Wiki — DLC](https://justcause.fandom.com/wiki/Downloadable_content_for_Just_Cause_4)

---

*본 분석서는 영어권 매체·공식 자료·위키 자료를 종합해 작성되었으며, 모든 수치와 인용은 위 출처에 근거한다. 판매량 등 일부 지표는 퍼블리셔 공식 발표와 매체 분석을 바탕으로 한 것으로, 정확한 누적 판매 총량은 공개되지 않았다.*
