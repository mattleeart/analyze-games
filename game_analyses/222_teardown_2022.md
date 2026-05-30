# Teardown (2022) — 한 명의 프로그래머가 부순 물리 샌드박스의 천장

> "파괴가 먼저였고, 세팅은 기술에 맞춰 나중에 끼워 맞췄다." — Dennis Gustafsson

《Teardown》은 게임 디자인의 정석적 순서를 뒤집은 작품이다. 보통은 "어떤 게임을 만들 것인가"를 먼저 정하고 그것을 구현할 기술을 찾지만, 《Teardown》은 정반대였다. 한 명의 스웨덴 프로그래머가 "완전히 파괴 가능한 voxel 세계를 실시간 레이트레이싱으로 굴릴 수 있다"는 기술적 가능성을 먼저 증명했고, 그 기술을 게임으로 만들 명분을 나중에 찾았다. 그 결과물은 2020년 얼리 액세스 출시 직후 Steam 베스트셀러에 올랐고, 2022년 4월 정식 출시 이후 "Garry's Mod 이후 가장 창의적인 샌드박스"라는 평가와 함께 인디 물리 게임의 새로운 천장을 세웠다.

이 글은 《Teardown》이 무엇이고, 어떻게 동작하며, 왜 성공했는지를 영어권 자료를 토대로 깊이 분석한다.

---

## 1. 게임 개요

### 개발사·퍼블리셔

《Teardown》은 스웨덴 인디 스튜디오 **Tuxedo Labs**가 개발·자체 퍼블리싱했다. 결정적인 점은 게임의 핵심 엔진과 기술 전체를 사실상 **한 사람**, 즉 프로그래머 **Dennis Gustafsson**이 구현했다는 것이다. Game Developer 인터뷰에서 정리된 바에 따르면, Gustafsson은 《Teardown》의 원래 컨셉을 직접 구상했고 게임에 들어가는 모든 핵심 기술을 직접 개발했다. 게임플레이 컨셉 작업에는 옛 동료인 디자이너 **Emil Bengtsson**이 협업했다.

Gustafsson은 신인이 아니었다. 그는 2010년 모바일 게임 스튜디오 **Mediocre**를 공동 창업해 《Smash Hit》, 《PinOut》, 《Sprinkle》 같은 히트 모바일 작품을 만들었다. Mediocre를 2017년에 정리한 뒤, 그는 voxel 기반 파괴 환경 기술 개발에 착수했고 그것이 《Teardown》의 토대가 되었다. 흥미롭게도 게임 내 연기(smoke) 효과는 과거 《Sprinkle》을 위해 만들었던 유체 애니메이션 시스템을 재활용한 것이다 — 즉 《Teardown》은 그의 10여 년 기술 자산이 누적된 결과물이기도 하다.

### 출시일 (플랫폼별)

| 플랫폼 | 출시일 |
|---|---|
| Windows (Steam 얼리 액세스) | 2020년 10월 29일 |
| Windows (정식 1.0 출시) | 2022년 4월 21일 |
| PlayStation 5 | 2023년 11월 15일 |
| Xbox Series X/S | 2023년 11월 15일 |

얼리 액세스는 "Part 1"으로 시작했고, "Part 2"가 2021년 12월 2일에 추가되며 새로운 미션·도구·로봇·토네이도 등이 들어왔다. 약 1년 반의 얼리 액세스를 거쳐 2022년 4월 21일에 1.0 정식 출시를 맞았다.

### 장르

1인칭 시점의 **물리 기반 샌드박스**로, 퍼즐과 액션 요소가 결합되어 있다. 표면적으로는 "하이스트(강도) 게임"의 옷을 입고 있지만, 본질은 "모든 것을 부술 수 있는 세계에서 창의적 경로를 직접 만드는 문제 해결 게임"이다.

### 엔진·기술 스택

《Teardown》의 심장은 **자체 제작 proprietary 엔진**이다. C++로 작성되었고, 두 가지 기술을 한 화면에서 결합한 것이 핵심이다.

1. **Voxel 기반 파괴**: 세계 전체가 파괴 가능한 voxel(작은 정육면체 블록)로 구성된다. 물 표면과 전선 정도를 제외하면 게임 안에 삼각형(polygon) 지오메트리가 없다 — 전부 volumetric 데이터다.
2. **실시간 레이트레이싱 전역 조명(GI)**: 라이팅·그림자·반사·앰비언트 오클루전이 실시간 레이트레이싱으로 계산된다. 덕분에 화면이 깨지고 무너지는 와중에도 빛이 사실적으로 반응한다.

기술적으로 더 들어가면, Gustafsson은 voxel을 일반적인 방식처럼 하나의 거대한 axis-aligned 볼륨에 담지 않았다. 수십억 개 voxel을 가진 단일 볼륨 대신, **수천 개의 작은 볼륨**을 만들고 각각을 voxel로 채우는 구조를 택했다. 충돌 검출(collision)은 CPU에서 voxel 대 voxel로 처리하고, 렌더링은 GPU에서 담당한다. 각 voxel은 8비트 컬러 팔레트로 재질 속성을 인코딩해, 나무·금속·콘크리트·유리가 서로 다르게 부서지고 타도록 했다.

왜 polygon이 아니라 voxel이었나? Gustafsson은 임의의 형태로 부서지는 지오메트리에서 **충돌 검출의 복잡성**을 polygon으로 감당하기가 너무 어렵기 때문이라고 설명했다. 정육면체 격자라는 단순한 단위로 세계를 표현하면, 그 단위를 떼어내고 무너뜨리는 물리 연산을 현실적인 성능으로 굴릴 수 있다. 즉 "완전 파괴"라는 목표가 기술 선택을 강제했다.

---

## 2. 게임 설명 — 이게 대체 무슨 게임인가

### 컨셉과 세계관

《Teardown》은 가상의 지자체 **Löckelle Municipality**를 무대로 한다. 플레이어는 영세한 **철거 회사 사장**을 연기한다. 처음에는 평범한 철거·해체 의뢰를 받지만, 점점 수상한 일들에 휘말린다. 한쪽에서는 기업 비리를 수사하는 경찰에 협조하라는 요청이 오고, 다른 한쪽에서는 점점 더 의심스러운 철거 일감이 들어온다. [스포일러] 이야기의 중심에는 에너지 드링크 회사 **BlueTide**와 거대 쇼핑몰 **Evertides Mall** 건설을 둘러싼 음모가 있다. 플레이어는 이 두 세계 사이를 오가며 결국 더 큰 부패의 실체에 다가간다.

다만 솔직히 말하면 스토리는 《Teardown》의 핵심이 아니다. 서사는 "왜 내가 이 건물을 부수고 물건을 훔치는가"에 대한 가벼운 동기 부여 장치에 가깝다. Gustafsson 본인도 인정했듯, **파괴 기술이 먼저 있었고 하이스트라는 설정은 그 기술을 게임답게 정당화하기 위해 나중에 끼워 맞춘 것**이다. 그는 이 게임을 만든 과정을 "지금까지 중 단연 가장 좌절스러운 경험(by far the most frustrating experience yet)"이라 표현했는데, 가장 큰 이유가 바로 이것이었다 — 슈터나 폭력적 게임플레이에 의존하지 않으면서 "이 엄청난 파괴 능력"을 쓸 명분을 찾는 일이 너무 어려웠다는 것이다. 하이스트는 그 답이었다. 알람이 울리기 전에 짧은 시간 안에 탈출해야 한다는 설정은, "벽을 부수고 지름길을 만든다"는 파괴 행위에 게임적 목적과 긴장을 부여한다.

### 무드·톤·아트 디렉션

《Teardown》의 미감은 독특하다. voxel로 만들어진 세계는 어딘가 장난감스럽고 미니어처 디오라마 같은 느낌을 주지만, 그 위에 얹힌 실시간 레이트레이싱 조명이 이 세계를 놀랍도록 사실적이고 분위기 있게 만든다. 황혼이 깔린 부둣가, 비 내리는 밤의 주차장, 햇살이 비스듬히 드는 창고 — voxel의 거친 입자감과 photorealistic한 빛이 충돌하면서 오히려 인상적인 비주얼을 만든다. Shacknews는 이 레이트레이싱 구현을 "an absolute stunner(완전히 압도적)"라고 평했고, 불이 번지는 방식이 《Far Cry 2》의 그 유명한 화염 전파를 능가한다고 했다.

톤은 전반적으로 경쾌하고 코믹하다. 폭력적인 게임이라기보다는, 거대한 디지털 장난감 상자를 던져주고 "마음껏 부숴봐"라고 말하는 쪽에 가깝다. 음악과 사운드 디자인은 파괴의 쾌감을 보조한다 — 나무가 쪼개지고 콘크리트가 갈라지고 유리가 산산조각 나는 소리, 그리고 그 위로 깔리는 긴장감 있는 하이스트 BGM이 60초 카운트다운의 아드레날린을 끌어올린다.

---

## 3. 핵심 시스템 / 메카닉 — 가장 자세하게

《Teardown》의 진가는 게임플레이 메카닉에 있다. 여기를 깊이 들여다보자.

### 코어 게임플레이 루프 — 2단계 하이스트

가장 대표적인 미션 유형인 하이스트는 명확한 2단계 구조를 갖는다.

1. **준비 단계 (시간 무제한)**: 알람에 연결되지 않은 모든 행동에는 시간 제한이 없다. 플레이어는 레벨을 자유롭게 돌아다니며 벽을 부수고, 나무판자로 램프를 만들고, 차량을 적절한 위치에 배치하고, 폭탄을 설치하는 등 **자신만의 탈출·수집 경로를 직접 건설**한다. 목표물(귀중품, 금고, 특정 오브젝트)들의 위치를 파악하고, 그것들을 가장 효율적으로 잇는 동선을 머릿속에 그린다.
2. **실행 단계 (60초)**: 알람에 연결된 첫 오브젝트를 건드리거나 탈취하는 순간 **60초 타이머**가 작동한다. 이제부터는 앞서 만들어 둔 경로를 따라 미친 듯이 달려 모든 목표물을 회수하고 도주 차량에 도달해야 한다.

이 구조의 천재성은 "느린 창의적 설계"와 "빠른 액션 실행"을 한 미션 안에 결합했다는 데 있다. 준비 단계는 퍼즐이자 건축이고, 실행 단계는 레이싱이자 액션이다. 같은 레벨을 여러 번 플레이하면 더 영리한 지름길을 발견하게 되고(《NME》는 이 재플레이 발견의 쾌감을 4/5 리뷰에서 칭찬했다), 그래서 "완벽한 단 한 번의 질주"를 다듬는 self-imposed 최적화 게임으로도 즐길 수 있다.

### 도구와 장비

플레이어는 점진적으로 도구를 해금하고 업그레이드한다.

- **시작 도구**: 썰매망치(sledgehammer, 근접 파괴), 소화기, 스프레이캔(마킹용)
- **해금 도구**: 블로토치(금속 절단), 샷건, 폭탄, 로켓런처
- **건설 자원**: 나무판자 — 램프·다리·구조물을 즉석에서 지어 차량 통로나 점프대를 만든다

수집한 귀중품을 현금화해 도구를 업그레이드할 수 있다. 도구 강화는 곧 더 빠른 파괴, 더 넓은 폭발 범위, 더 다양한 경로 설계를 의미한다.

### 차량

자동차, 트럭, 크레인, 굴착기, 보트 등 다양한 차량을 운전할 수 있다. 차량에 탑승하면 시점이 3인칭으로 전환된다. 굴착기로 벽을 밀어버리거나, 트럭으로 금고를 실어 나르거나, 크레인으로 구조물을 무너뜨리는 등 차량 자체가 거대한 파괴·운반 도구가 된다.

### 진행 구조

스토리 캠페인은 **40개 미션**, **9개의 파괴 가능 voxel 레벨**로 구성된다. 모든 미션이 60초 하이스트는 아니다. 미션 유형에는 다음이 있다.

- 표준 하이스트 (알람·타이머)
- 타이머 없는 하이스트
- 레이싱 미션
- 스텔스 미션
- 추격(쫓기는) 미션

후에 추가된 무료/유료 콘텐츠도 각자의 미션 세트를 갖는다 — 예를 들어 《Art Vandals》는 5개 미션, 《Time Campers》는 9개 미션으로 구성된다.

### 추가 모드 — 게임의 수명을 늘린 진짜 핵심

캠페인은 사실 《Teardown》이 제공하는 즐거움의 절반도 안 된다.

- **Sandbox(샌드박스) 모드**: 캠페인의 각 레벨을 목표 없이, 무제한 자원으로 자유롭게 가지고 논다. 캠페인을 클리어하지 않아도 모든 레벨과 도구를 열어 샌드박스에서 쓸 수 있는 옵션이 있다. 순수한 파괴 놀이터다.
- **Creative(크리에이티브) 모드**: 게임 월드 안에서 voxel을 직접 칠해 3D 오브젝트를 만든다. PS5·Xbox 버전에서도 작동한다.
- **챌린지 모드**: Mayhem(60초 안에 최대한 많이 파괴), Hunted(쫓기면서 아이템 수집), Fetch(60초 안에 최대한 많이 수집).

### 멀티플레이

출시 시점에는 싱글 전용이었으나, 멀티플레이가 오래 요청되어 왔다. PC 멀티플레이는 2026년 3월 12일에 정식 출시되었고, 최대 12인 협동 또는 경쟁(deathmatch, team deathmatch, capture the flag)을 지원한다. 출시 당시 동시접속 피크 15,172명을 기록했다.

### 모딩 — UGC 생태계

《Teardown》의 장기 생명력을 결정한 시스템이다.

- **MagicaVoxel 연동**: 외부 voxel 에디터로 만든 모델을 커스텀 레벨로 가져올 수 있다.
- **Steam Workshop + 내장 레벨 에디터 + Lua 스크립팅**: 맵, 도구, 차량은 물론 **완전히 새로운 게임 모드**까지 만들 수 있다.
- **인게임 모드 로더**: 수천 개의 커뮤니티 모드를 게임 안에서 바로 불러온다.

모드 수의 성장세는 가팔랐다 — 2022년 5월 약 1,100개, 2023년 3월 5,000개 이상, 2023년 9월 6,000개 이상. Tuxedo Labs는 연 2회 모딩 대회를 열어 커뮤니티를 독려했고, 콘솔판에는 큐레이션된 "Mod Pack"을 제공했다. 평론가들은 이 모드 지원을 게임 장기 수명의 핵심 요인으로 꼽았다.

### UI/UX 디자인 철학

《Teardown》의 인터페이스는 의도적으로 미니멀하다. 플레이어를 방해하지 않고 세계와의 상호작용에 집중하게 만드는 것이 목표다. 다만 모든 면에서 매끄럽지는 않았다 — 일부 평론은 점프 컨트롤이 "floaty(붕 뜬다)"하고 오브젝트 상호작용이 "finicky(까다롭다)"하다고 지적했다(GamingBolt).

---

## 4. 평가

### Metacritic / OpenCritic

《Teardown》은 전 플랫폼에서 "generally favorable(대체로 호평)" 평가를 받았다.

| 플랫폼 | Metacritic |
|---|---|
| PC | 80 / 100 |
| PlayStation 5 | 78 / 100 |
| Xbox Series X/S | 85 / 100 |

흥미롭게도 늦게 나온 콘솔판, 특히 Xbox Series 버전(85)이 PC 원판(80)보다 높은 점수를 받았다. 이는 정식 출시 후 수년간 콘텐츠와 완성도가 누적된 효과로 볼 수 있다.

### 주요 평론 인용

- **PC Gamer (90/100)**: "Garry's Mod 이후 가장 창의적인 샌드박스 플랫폼(the most creative sandbox platform since Garry's Mod)"이라 평하며 "끝없이 즐거운 파괴 샌드박스(endlessly delightful destruction sandbox)"라 요약했다. PC Gamer는 이 게임을 그해 최고의 샌드박스 게임으로 꼽았다.
- **GameSpot (7/10, Alessandro Barbosa)**: 물리를 "superb(탁월하다)"라 칭하며 "그 물리의 혼돈스러운 본성은 한결같은 즐거움의 원천(the chaotic nature of its physics are a consistent source of joy)"이라 했다. 다만 "독창적인 아이디어와 만족스러울 만큼 단순한 전제로 가득하지만, 페이싱이 나쁜 캠페인에 발목 잡혔다"고 단서를 달았다. 리뷰 제목은 마일리 사이러스 노래를 빌린 "Came In Like A Wrecking Ball".
- **Rock Paper Shotgun (Graham Smith)**: voxel 파괴 메카닉과 그것이 게임플레이에 갖는 본질적 가치를 높이 사며, 그 파괴 기술이 《Red Faction: Guerrilla》 같은 이전 파괴 중심 게임들을 능가한다고 평했다.
- **Eurogamer**: "상호작용의 최고봉, 결코 질리지 않는 그 비뚤어진 만족감(the interactive fulcrum par excellence, that twisted gratification that never tires)".
- **Shacknews (9/10)**: 레이트레이싱 구현이 "an absolute stunner", 불 전파가 《Far Cry 2》를 능가.
- **CD-Action (9/10)**: 불과 폭발과의 상호작용을 "mesmerising(넋을 잃게 한다)"이라 표현.
- **NME (4/5)**: 다시 플레이할 때 새로운 지름길을 발견하는 데서 오는 만족.

### 수상 이력

- **수상**: Independent Games Festival(IGF) 2021 "Excellence in Design"
- **노미네이트**: Game Developers Choice Awards 2023 "Best Technology"(honourable mention), Golden Joystick Awards 2022 "Best Indie Game" 및 "PC Game of the Year", Steam Awards 2022 "Most Innovative Gameplay", D.I.C.E. Awards 2023 "Outstanding Technical Achievement", IGF 2021 Seumas McNally Grand Prize
- **매체 선정**: Shacknews는 2020년 최고의 얼리 액세스 게임이자 2022년 최고의 PC 게임으로 선정. Rock Paper Shotgun과 GameSpot은 각각 그해 최고의 게임 중 하나로 꼽음. PC Gamer "top 100 PC games"에서 2022년 25위, 2023년 95위.

### 상업 지표

- 얼리 액세스 출시 첫 며칠간 **Steam 베스트셀러** 상위권에 올랐다.
- 얼리 액세스 단계에서 1,800개 이상 리뷰, **96% 긍정**.
- **2022년 8월 기준 110만 카피** 판매.
- **2023년 12월(콘솔 출시 후) 250만 플레이어** 도달.
- 가격은 출시 시 $20였으나 2023년 3월 멀티플레이 발표와 함께 $30로 인상되었다.

### 평론-유저 괴리

《Teardown》은 평론과 유저 평가가 비교적 일치한 케이스다. 평론은 80점대, 유저는 96% 긍정으로 둘 다 강한 호평이었다. 다만 강조점에 미묘한 차이는 있었다 — 평론은 "캠페인 페이싱"의 약점을 자주 지적한 반면, 유저들은 샌드박스·모드·파괴 그 자체의 순수한 재미에 더 무게를 두었다. 즉 유저에게 캠페인은 부수적이었고, 진짜 게임은 "무제한 파괴 놀이터"였다.

---

## 5. 성공 요인 분석 — 핵심

《Teardown》은 거대 자본도, 마케팅 예산도, 큰 팀도 없이 성공했다. 그 비결을 분해해 보자.

### (1) 기술이 곧 게임플레이가 된 희귀한 케이스

대부분의 게임에서 그래픽 기술은 "껍데기"다. 더 예쁜 그림을 위한 것이지 게임플레이 자체를 바꾸지는 않는다. 《Teardown》은 다르다. 완전 파괴 voxel 시스템은 단순한 시각 효과가 아니라 **게임의 핵심 메카닉 그 자체**다. 벽을 부수는 것이 곧 지름길을 만드는 것이고, 건물을 무너뜨리는 것이 곧 퍼즐을 푸는 것이다. Gustafsson은 인터뷰에서 "파괴가 단순한 이펙트가 아니라 실제 게임플레이로 쓰이는 것이 중요했다"고 강조했다. 이 통합이 《Teardown》을 다른 모든 "파괴가 되는 게임"과 구별 짓는다.

### (2) "선(先)기술, 후(後)디자인"의 역발상

보통은 위험한 접근이다 — 기술을 만들어 놓고 게임이 안 나올 수 있다. 실제로 Gustafsson은 그 과정이 "가장 좌절스러웠다"고 했다. 하지만 그가 만든 기술이 워낙 강력하고 독창적이었기에, 그 위에 얹은 하이스트라는 단순한 프레임만으로도 충분히 새로운 게임이 되었다. 파괴 기술의 차별성이 게임 전체의 차별성을 떠받친 셈이다.

### (3) 마케팅 없이 이긴 바이럴 — Twitter 영상

Gustafsson은 전통적 마케팅 기법을 일절 쓰지 않았다고 밝혔다. 대신 그는 개발 과정에서 **파괴 장면을 담은 짧은 영상을 Twitter에 꾸준히 올렸고**, 그 영상들이 입소문을 타며 출시 전 인지도를 폭발적으로 키웠다. voxel이 산산조각 나며 실시간 빛이 반응하는 장면은 GIF·짧은 클립으로 공유하기에 완벽했다 — "보면 바로 이해되고, 직접 해보고 싶어지는" 콘텐츠였다. 그는 초기 성공을 바로 이 Twitter 영상의 인기 덕으로 돌렸다. 즉 게임의 시각적 매력 자체가 마케팅이었다.

### (4) 얼리 액세스를 통한 점진적 완성과 커뮤니티 동반 성장

2020년 10월 얼리 액세스로 출시해 2022년 4월 정식 출시까지 약 1년 반 동안, 플레이어와 함께 게임을 키웠다. Part 1 → Part 2(2021년 12월)로 콘텐츠를 늘려가며 초기 96% 긍정이라는 강한 신뢰를 쌓았고, 이 기간 동안 모딩 생태계가 자생적으로 성장했다.

### (5) 모딩 생태계 — 콘텐츠를 외주화한 무한 수명

내장 레벨 에디터, Lua 스크립팅, Steam Workshop, MagicaVoxel 연동은 커뮤니티가 게임 콘텐츠를 무한히 생산하게 만들었다. 출시 1년 만에 5,000개 넘는 모드가 쌓였다. 이는 작은 스튜디오가 감당할 수 없는 콘텐츠 양을 커뮤니티가 대신 채워준다는 의미였고, 그만큼 재구매·재플레이 이유가 계속 생겼다.

### (6) 비교 가능한 동시기 작품 대비 차별점

파괴를 내세운 게임은 과거에도 있었다 — 《Red Faction: Guerrilla》(2009)의 GeoMod, 《Battlefield》의 Levolution 등. 하지만 이들은 대개 "정해진 방식으로 정해진 구조물만" 부서졌다. 《Teardown》은 **세계의 거의 모든 것을 임의의 형태로** 부술 수 있었고, 그 파괴를 게임의 핵심 동사(verb)로 만들었다. Rock Paper Shotgun이 그 파괴 기술이 《Red Faction: Guerrilla》를 능가한다고 평한 이유다.

---

## 6. 비평적 시각 / 한계 / 논란

호평 일색은 아니었다. 평론가들이 짚은 약점들은 분명했다.

### 캠페인 페이싱과 미션 다양성

가장 자주 지적된 문제다. GameSpot은 캠페인 진행 구조가 오히려 "맵을 마음껏 부수는 능력"을 제한한다고 봤고, 미션 다양성이 부족하다고 평했다. Push Square 역시 캠페인 전반부가 목표 다양성이 부족하다(후반부에서 개선됨)고 지적했다. 즉 게임의 가장 큰 매력(자유로운 파괴)을 캠페인의 규칙(60초 제한, 정해진 목표)이 종종 억누른다는 역설이다. 많은 유저가 결국 샌드박스와 모드로 옮겨간 이유이기도 하다.

### 물리의 비현실성

PC Games와 Eurogamer.it 등은 건물이 소수의 voxel만으로 비현실적으로 지탱되는 점을 지적했다 — 구조물의 대부분을 부숴도 몇 개의 voxel이 남아 전체가 공중에 떠 있는 듯한 비논리적 상황이 나온다. 완전 시뮬레이션이 아니라 "게임적 타협"이 있는 물리라는 점이 드러나는 지점이다.

### 컨트롤의 거칠음

GamingBolt는 오브젝트 상호작용이 "finicky(까다롭다)"하고 점프 컨트롤이 "floaty(붕 뜬다)"하다고 했다. 정밀한 조작이 필요한 순간에 답답함을 줄 수 있다.

### 출시 시 멀티플레이·콘솔 모드 부재

여러 매체가 출시 시점의 멀티플레이 부재를 아쉬워했다. "친구와 함께 부수고 싶다"는 자연스러운 욕구를 오랫동안 채워주지 못했고, PC 멀티플레이는 2026년에야 정식 출시되었다. 콘솔판은 모드 접근이 제한적(큐레이션된 Mod Pack만 제공)이라는 한계도 있었다.

### 가격 인상 논란

2023년 3월, 멀티플레이 개발 발표와 함께 게임 가격이 $20에서 $30으로 인상되었다. 추가 콘텐츠를 위한 결정이었지만, 일부 신규 구매자에게는 진입 장벽이 높아진 셈이었다.

---

## 7. 영향과 유산

### 장르에 미친 영향

《Teardown》은 "완전 파괴"가 시각 효과를 넘어 게임의 핵심 메카닉이 될 수 있음을, 그것도 한 명의 개발자가 만든 인디 규모에서도 가능함을 증명했다. 이는 voxel·파괴 기술에 도전하는 후속 인디 개발자들에게 강력한 레퍼런스이자 영감이 되었다. "물리 샌드박스 인디"라는 카테고리에서 《Teardown》은 사실상 새로운 기준점을 세웠다.

### 산업적 의미 — 대기업의 주목

기술의 가치는 업계 거물들의 행보로 증명되었다. 2022년 7월 1일, Tuxedo Labs는 **Embracer Group**(스웨덴 거대 게임 지주사)의 자회사 **Saber Interactive**에 100% 인수되었다. 이는 Embracer가 Tripwire Interactive, Limited Run Games, 《반지의 제왕》 IP 권리 등을 사들이던 대규모 인수 행렬의 일부였다. 주목할 점은 Saber의 인수 명분이었다 — 그들은 《Teardown》의 기술을 **《Minecraft》·《Roblox》와 경쟁할 수 있는 더 큰 플랫폼**으로 확장할 수 있다고 봤다. 즉 이 voxel 엔진을 단일 게임이 아니라 UGC 플랫폼의 토대로 평가한 것이다.

인수는 Gustafsson에게도 의미가 컸다. 그는 인수 후 "이건 정말 안도감이다. 이제 다시 진짜 작업(개발)으로 돌아갈 수 있으니까(it is such a relief because I can go back to doing actual work)"라고 했다. 1인 핵심 개발자가 사업·운영 부담에서 벗어나 기술에 집중할 환경을 얻었다는 뜻이다. 인수 후 스튜디오는 6인으로 확대되었고 Marcus Dawson이 CEO로 합류했다.

소유권은 이후로도 변동을 겪었다. 2024년 3월 Embracer가 Saber를 분리할 때 Tuxedo Labs는 Embracer에 남았고, 2025년 5월에는 **Coffee Stain Group**의 일부로 분사되었다. 《Goat Simulator》·《Valheim》으로 유명한 Coffee Stain의 우산 아래 들어간 것이다.

### AI 연구에 쓰인 게임

특이한 유산도 있다. **Google DeepMind**는 게임 월드를 탐색하는 머신러닝 모델 **SIMA**를 학습시키는 데 《Teardown》을 사용했다. 풍부하게 상호작용 가능한 3D 환경이라는 점이 AI 에이전트 훈련 환경으로 가치가 있었던 것이다.

### 지속되는 생명력

《Teardown》은 출시 후에도 꾸준히 진화했다. 2022년 12월 무료 확장 《Art Vandals》(모딩 시스템 시연 목적), 2024년 6월 《Folkrace》 DLC, 2025년 6월 《The Greenwash Gambit》(세 번째 DLC 팩), 2026년 3월 PC 멀티플레이 정식 출시, 그리고 네 번째 DLC 팩 《Relics of Barkuna》가 2026년 6월 예정되어 있다. 2024년 1월 Wired는 이 게임을 PS Plus 베스트 게임 중 하나로 꼽기도 했다. 한 명이 시작한 기술 데모가, 수년에 걸쳐 살아 숨 쉬는 플랫폼으로 성장한 것이다.

### 문화적 의미

《Teardown》은 "인디 개발자 1인의 기술 집념이 어디까지 갈 수 있는가"를 보여준 상징적 사례다. Mediocre 시절부터 누적된 Gustafsson의 그래픽 프로그래밍 역량이 voxel 파괴 + 레이트레이싱이라는 한 점에서 결실을 맺었고, 그것이 Twitter 바이럴 → 얼리 액세스 히트 → 대기업 인수라는 인디 성공 신화의 교과서적 경로를 밟았다. 화려한 마케팅이 아니라 "보면 바로 이해되는 압도적인 게임플레이 영상" 하나가 게임을 팔 수 있다는 것을, 《Teardown》은 가장 순수한 형태로 증명했다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 내용 |
|---|---|
| 개발사/퍼블리셔 | Tuxedo Labs (스웨덴) |
| 핵심 개발자 | Dennis Gustafsson (엔진·핵심 기술 1인 구현) |
| 디자인 협업 | Emil Bengtsson |
| 엔진 | 자체 C++ proprietary 엔진 (voxel 파괴 + 실시간 레이트레이싱 GI) |
| 얼리 액세스 | 2020-10-29 (Windows/Steam) |
| 정식 출시 | 2022-04-21 (Windows) |
| 콘솔 출시 | 2023-11-15 (PS5, Xbox Series X/S) |
| 캠페인 분량 | 40 미션, 9개 voxel 레벨 |
| Metacritic | PC 80 / PS5 78 / Xbox Series 85 |
| 판매량 | 110만 카피 (2022-08) |
| 플레이어 수 | 250만 명 (2023-12) |
| 모드 수 | 6,000개+ (2023-09) |
| 멀티플레이(PC) | 2026-03-12 정식 출시, 동접 피크 15,172 |
| 인수 | Saber Interactive(Embracer) 100% 인수 (2022-07-01) → Coffee Stain Group 분사 (2025-05) |
| 주요 수상 | IGF 2021 "Excellence in Design" |

### 주요 인터뷰·강연 자료

- **GDC Plays Teardown with Dennis Gustafsson** (GDC Twitch / YouTube): 게임 제작 과정에 대한 Bryant Francis와의 대담. https://www.youtube.com/watch?v=Z8QbY-xmbUQ
- **Game Developer — "How beautiful voxels laid the way for Teardown's heist-y framework"**: voxel 엔진 구조와 하이스트 메카닉의 기원. https://www.gamedeveloper.com/design/how-beautiful-voxels-laid-the-way-for-i-teardown-s-i-heist-y-framework
- **Game Developer — "Combining bombastic heists with a fully destructible voxel world in Teardown"**: https://www.gamedeveloper.com/design/combining-bombastic-heists-with-a-fully-destructible-voxel-world-in-i-teardown-i-
- **PC Gamer — "Teardown dev on the 'frustrating experience' of developing the breakout hit"**: 개발의 좌절과 디자인 고충. https://www.pcgamer.com/teardown-dev-on-the-frustrating-experience-of-developing-the-breakout-hit/
- **PC Gamer — "One million copies and 5000 mods later, Teardown's creator is just getting started"**: 판매·모딩 성과. https://www.pcgamer.com/one-million-copies-and-5000-mods-later-teardowns-creator-is-just-getting-started/
- **80.lv — "Teardown Developer Breaks Down Multiplayer and Voxel Destruction Tech"**: 멀티플레이와 voxel 기술 해설. https://80.lv/articles/teardown-developer-breaks-down-multiplayer-and-voxel-destruction-tech
- **Voxagon Blog** (Dennis Gustafsson의 기술 블로그): https://blog.voxagon.se/

### 참고 자료 목록 (영어권 매체 중심)

- Wikipedia — Teardown (video game): https://en.wikipedia.org/wiki/Teardown_(video_game)
- Metacritic — Teardown: https://www.metacritic.com/game/teardown/
- OpenCritic — Teardown: https://opencritic.com/game/13035/teardown
- PC Gamer — Teardown review (90/100): https://www.pcgamer.com/teardown-review/
- GameSpot — Teardown Review: Came In Like A Wrecking Ball (7/10): https://www.gamespot.com/reviews/teardown-review-came-in-like-a-wrecking-ball/1900-6417871/
- Worthplaying — Embracer Group Acquires Teardown Developer Tuxedo Labs: https://worthplaying.com/article/2022/8/17/news/133194-embracer-group-acquires-teardown-developer-tuxedo-labs/
- Teardown 공식 사이트: https://www.teardowngame.com/
- Steam — Teardown: https://store.steampowered.com/app/1167630/Teardown/

---

*본 분석서는 영어권 매체·개발자 인터뷰·공식 자료를 토대로 작성되었으며, 모든 판매·평가 수치는 출처에 명시된 시점 기준이다. 일부 사후 콘텐츠(2026년 멀티플레이 등) 정보는 출시 로드맵·공식 발표에 근거한다.*
