# 《Dispatch》 (2025) 심층 분석

> "We've been going to all these conferences for seven years looking for money and trying to make the next six months work. It's been hell." — Nick Herman (창립자 겸 크리에이티브 디렉터, The GameBusiness 인터뷰)
> (7년 동안 온갖 컨퍼런스를 돌며 돈을 구하고, 앞으로 6개월을 버틸 방법을 찾으려 애썼다. 그야말로 지옥이었다.)

7년간 폐업의 벼랑 끝을 오가던 30인 규모의 신생 스튜디오가, 2025년 가을 단 한 달 만에 200만 장을 팔아 치우고 "에피소드형 내러티브 게임은 죽었다"는 업계의 통념을 정면으로 뒤집었다. 《Dispatch》는 Telltale Games 출신 개발자들이 만든 슈퍼히어로 직장 코미디로, "선택 기반 어드벤처"라는 장르가 모바일과 무료 게임에 잠식되어 한물갔다고 여겨지던 시기에 등장해 그 장르를 부활시켰다는 평가를 받는다. 이 분석서는 《Dispatch》가 무엇이며, 어떤 메카닉으로 작동하고, 왜 거의 모든 예측을 거슬러 성공했는지를 영어권 자료를 토대로 정밀하게 다룬다.

---

## 1. 게임 개요

### 기본 정보

- **제목**: 《Dispatch》
- **개발사**: AdHoc Studio (미국, 로스앤젤레스)
- **퍼블리셔**: AdHoc Studio (자체 퍼블리싱)
- **장르**: 에피소드형 내러티브 어드벤처 / 슈퍼히어로 직장 코미디 / 실시간 디스패치 시뮬레이션 하이브리드
- **엔진**: Unreal Engine 4
- **플랫폼 및 출시**:
  - PlayStation 5, Windows (PC) — 2025년 10월 22일 ~ 11월 12일, 8개 에피소드 단계 출시
  - Nintendo Switch / Switch 2 — 2026년 1월 28일 (전 에피소드 일괄)
  - Xbox Series X/S — 2026년 출시 예정

### 에피소드 출시 일정 (PC / PS5)

《Dispatch》는 한 번에 전편이 나온 것이 아니라, 2주에 걸쳐 매주 두 편씩 공개되는 "프레스티지 TV" 방식의 일정을 택했다.

| 에피소드 | 출시일 | 제목 |
|---|---|---|
| Ep. 1-2 | 2025-10-22 | "Pivot", "Onboard" |
| Ep. 3-4 | 2025-10-29 | "Turnover", "Restructure" |
| Ep. 5-6 | 2025-11-05 | "Team Building", "Moving Parts" |
| Ep. 7-8 | 2025-11-12 | "Retrospective", "Synergy" |

에피소드 제목이 전부 기업 경영·인사 용어("피벗", "온보딩", "이직률", "구조조정", "팀 빌딩", "시너지")라는 점은 이 작품의 정체성, 즉 슈퍼히어로 세계를 직장 시트콤의 틀로 비트는 풍자 의도를 단적으로 보여준다.

### 주요 크레딧

- **디렉터**: Nick Herman, Dennis Lenart, Chris Rebbert
- **프로듀서**: Natalie Herman
- **수석 작가/내러티브**: Pierre Shorette (집필진: Suzee Matson, Ashley Jeffalone, Chad Rhiness, Chris Rebbert)
- **디자이너**: Charles Marcolim
- **프로그래머**: Seth Kingsley
- **아티스트**: Derek Stratton
- **작곡**: Andrew Arcadi (추가 음악 Skyler Barto)
- **CEO/공동창립자**: Michael Choung

AdHoc Studio는 2018년 Michael Choung, Nick Herman, Dennis Lenart, Pierre Shorette 등이 설립했다. 이들은 Telltale Games 시절 《The Wolf Among Us》와 《Tales from the Borderlands》의 핵심 크리에이티브였다. 특히 Pierre Shorette는 《The Wolf Among Us》와 《Batman: The Telltale Series》의 리드 작가 중 한 명이었고, Herman과 Lenart는 《The Wolf Among Us》 1화를 만든 디렉팅 라인이었다. 즉 《Dispatch》는 "선택 기반 내러티브 어드벤처"라는 형식을 발명한 사람들이, 자신들이 만든 회사가 무너진 뒤 직접 세운 스튜디오에서 그 형식을 다시 정의하려 한 작품이다.

### 개발 규모

The GameBusiness 인터뷰에 따르면, 2024년 기준 AdHoc은 약 **30명** 규모였고, 애니메이션은 외주 파트너와 협업했다. CEO Michael Choung은 예산을 "AA 영역의 중하단"(middle, lower-end of the AA space)으로 표현했다. 즉 트리플 A급 블록버스터 예산이 아니라, 검증된 배우와 협업하면서도 파트너들의 "데뷔작에 대한 호의"로 통제된 비용 구조로 만든, 전형적인 AA·인디 사이의 작품이다. 개발 기간은 라이브 액션 시도까지 포함하면 7년, 애니메이션 본격 제작으로는 코로나 이후 수년에 걸친 장기 프로젝트였다(자세한 개발사는 5장에서 다룬다).

---

## 2. 게임 설명: 이 게임이 무엇인가

### 컨셉과 세계관

《Dispatch》는 초능력자(supers)가 흔한 대체 세계의 로스앤젤레스를 배경으로 한다. 사회는 초능력을 가진 "수퍼(supers)"와 그렇지 않은 "노미(normies)"로 나뉘어 있고, 많은 히어로들은 **Superhero Dispatch Network(SDN)**라는 조직에 고용되어 도시 곳곳의 사건에 출동한다. 한마디로, 슈퍼히어로 활동이 공공 서비스이자 직장 노동으로 제도화된 세계다. 911 신고 센터가 슈퍼히어로 출동 콜센터가 되었다고 생각하면 정확하다.

핵심 컨셉은 "당신은 영웅이 아니라, 영웅들을 현장에 배치하는 디스패처(관제사)"라는 데 있다. 화려한 액션의 주체가 아니라, 책상 앞 모니터에서 누구를 어디로 보낼지를 결정하는 관리자의 시점에서 슈퍼히어로 서사를 본다.

### 줄거리 (스포일러 포함 — [스포일러] 표기)

주인공은 **Robert Robertson III**(애런 폴 분), 3대째 이어진 슈퍼히어로 가문의 아들이자 메카 슈트를 입는 영웅 **Mecha Man**이다. 그는 초능력 자체는 없지만, 할아버지가 만든 다양한 무기를 갖춘 기계 슈트를 물려받아 활동해 왔다. 게임은 그가 아버지를 죽인 슈퍼빌런 **Shroud**(매튜 머서 분, 본명 Elliot Connors)를 추적하면서 시작한다.

[스포일러] Robert는 Shroud의 갱단 **Red Ring**의 함정에 빠져, 그의 상징과도 같은 메카 슈트에 폭탄이 설치되고 슈트가 파괴된다. 수리 비용을 감당할 수 없게 된 그는, 생계를 위해 SDN의 디스패처 자리를 받아들인다. 그가 맡게 되는 팀이 바로 **Z-Team** — 갱생 프로그램을 밟고 있는 전직 빌런들로 구성된, 조직의 가장 밑바닥 부서다. Robert는 이 부적응자 집단을 관리하며 슈트를 다시 만들어 나가는데, 그 과정에서 팀원 중 한 명인 **Invisigal(Courtney)**이 과거 Shroud 밑에서 일했다는 사실이 드러난다. 서사는 결국 Red Ring과의 대결로 치닫고, 플레이어가 누구를 신뢰하고 어디까지 폭력을 허용하는가에 따라 결말이 분기한다.

### 주요 캐릭터

- **Robert Robertson III / Mecha Man** (애런 폴) — 능력 없는 3세대 영웅. 가문의 유산인 메카 슈트가 정체성의 전부였으나 그것을 잃고 책상 앞에 앉게 된다. 자조와 책임감 사이에서 흔들리는 인물.
- **Courtney / Invisigal** (로라 베일리) — 천식을 앓는 반항적 전직 빌런이자 Z-Team의 최하위 멤버. 숨을 참는 동안만 투명해질 수 있다는 한계를 가진 능력. 주요 로맨스 노선 중 하나이자, Shroud와의 과거가 후반부 갈등의 핵.
- **Chase / Track Star (Starblazer)** (제프리 라이트) — 스피드스터. 전직 Brave Brigade 소속이자 Robert의 디스패칭 멘토. 능력의 부작용으로 일반인보다 50배 빠르게 늙어가는 탓에 강제로 은퇴해 SDN에서 일한다. 게임에서 가장 비극적이고 따뜻한 무게중심.
- **Elliot Connors / Shroud** (매튜 머서) — 전직 Brave Brigade에서 빌런으로 돌아선 Red Ring의 수괴이자 Robert 아버지의 살해자. 미래 예측 능력을 주는 가면과 사이버네틱 증강을 지녔다.
- **Mandy / Blonde Blazer** (에린 이베트) — 또 다른 로맨스 노선의 핵심 인물.
- **Katon-Ur / Phenomaman** (트래비스 윌링엄) 등 다양한 Z-Team·SDN 인물들이 직장 시트콤의 앙상블을 구성한다.

### 무드 / 톤 / 아트 디렉션

비평가들이 가장 자주 동원한 비교 대상은 《The Boys》, 《Invincible》, 《BoJack Horseman》, 그리고 시트콤 《The Office》와 영화 《Thunderbolts》다. 즉 "성인용 슈퍼히어로 풍자"의 거친 에지와 "직장 시트콤"의 일상성·관계극을 결합한 톤이다. The VanCougar는 이 작품을 "슈퍼히어로가 The Office를 만나는 곳"이라 요약했다. 비주얼은 셀 셰이딩 스타일의 성인 애니메이션 룩으로, 프레스티지 TV 애니메이션(《Invincible》류)의 질감을 게임으로 옮긴 것이 특징이다.

작가진은 라이트 코미디와 도를 넘는 에지(edgy) 사이의 선을 능란하게 탄다는 평을 받았다. GameSpew는 이 작품을 두고 "지금까지 만들어진 최고의 슈퍼히어로 게임 중 하나"라 했고, 동시에 Kotaku는 톤이 때때로 "거슬릴 정도로 의도적으로 도발적(obnoxious)"이며 강도의 진폭이 채찍질처럼 급변한다고 지적했다 — 이 양면성이 작품의 톤을 가장 정확히 설명한다.

### 사운드 / 음악

작곡은 Andrew Arcadi(추가 음악 Skyler Barto)가 맡았으며, 사운드트랙은 다수 리뷰에서 호평받았다. 그러나 《Dispatch》에서 음향의 진짜 무기는 음악보다 **보이스 캐스팅**이다. 《Breaking Bad》의 애런 폴, 《The Last of Us》·《Marvel's Spider-Man 2》의 로라 베일리, 《West World》의 제프리 라이트, 그리고 인기 TTRPG 방송 Critical Role의 핵심 성우 매튜 머서·트래비스 윌링엄·에린 이베트가 주역을 맡았다. 여기에 jacksepticeye, MoistCr1TiKaL(Cr1TiKaL), Joel Haver, Alanah Pearce 같은 크리에이터와 래퍼 Yung Gravy, Thot Squad까지 카메오로 참여했다. 다수 매체가 "완벽에 가까운 보이스 연기"를 작품의 핵심 강점으로 꼽았다.

---

## 3. 핵심 시스템 / 메카닉 (가장 자세하게)

《Dispatch》의 디자인적 정체성은 두 개의 이질적인 게임을 하나로 봉합한 데 있다. 하나는 Telltale식 **선택 기반 내러티브 어드벤처**, 다른 하나는 **실시간 디스패치(관제) 시뮬레이션**이다.

### 코어 루프 1 — 디스패칭 (실시간 관리)

게임플레이의 절반은 책상 앞 모니터다. 도시 곳곳에서 SDN 가입자(subscriber)의 신고 콜이 들어온다. 규모는 천차만별이다. "나무에 걸린 풍선 빼기" 같은 사소한 일부터 "화재 현장 인명 구조" 같은 대형 사건까지.

작동 방식은 다음과 같다.

1. **콜 수신과 시간 압박**: 콜이 뜨면 이를 열어 히어로를 배정하기까지 제한 시간이 있다. 콜을 클릭하면 시간이 일시 정지되어 브리핑을 읽을 수 있다.
2. **스탯 매칭**: 디스패치 시스템은 한 명 이상의 히어로를 콜에 배정하고, 그들의 **스탯 프로필**을 미션의 숨겨진 요구 프로필과 비교해 겹치는 정도로 성공 확률을 계산한다. 다섯 스탯은 **Combat(전투), Vigor(체력/활력), Mobility(기동성), Charisma(카리스마), Intellect(지력)**이다. 어떤 사건은 전투가, 어떤 사건은 카리스마(설득)나 지력이 요구된다 — 사건의 성격에 맞는 히어로 조합을 골라야 한다.
3. **상태 전이와 쿨다운**: 배정된 히어로는 현장으로 이동하며 "busy"(출동 중), 임무 후엔 "returning"(복귀 중), 본부 복귀 후엔 "resting"(휴식)으로 상태가 바뀐다. 휴식 중에는 재배정이 불가능하고, 프로필 위의 초록색 게이지가 줄어들며 재출동 가능 시점을 알린다. 즉 한정된 인력 풀을 시간 축 위에서 회전시키는 자원 관리 게임이다.
4. **랭크 진척**: 히어로들이 임무에 성공할수록 디스패처로서 Robert의 랭크가 오른다. 높은 랭크는 부상당한 히어로를 치료하는 붕대, 쓰러진 히어로를 회복시키는 제세동기 같은 도구 접근권 등의 혜택을 준다.

이 모드는 실시간으로 동시다발 콜을 곡예하듯 처리해야 하므로, 비평가들이 "스트레스 받고 도전적"이라 표현하는 긴장감을 만든다. 한정된 히어로를 어디에 쓰고 어디를 포기할지, 쿨다운 타이밍을 어떻게 짜낼지를 즉석에서 판단해야 한다.

### 코어 루프 2 — 내러티브 / 선택 (Telltale 계보)

나머지 절반은 정통 내러티브 어드벤처다. 다이얼로그 트리, 시간 제한이 걸린 선택지, 캐릭터 관계 형성이 핵심이다. 다만 AdHoc은 Telltale의 전통 한 가지를 의도적으로 폐기했는데, 바로 화면에 큼지막하게 뜨던 "[캐릭터] will remember that"(그 캐릭터가 이를 기억할 것이다) 알림이다. 개발진은 이 장치가 선택의 무게를 인위적으로 강조해 몰입을 깬다고 보고 제거했다(ingamenews 등 보도).

선택은 히어로의 충성도, 미션 성공률, 그리고 Robert의 개인적 여정에 파문처럼 번진다. 즉 디스패칭(시스템)과 내러티브(드라마)가 분리된 두 게임이 아니라, 어떤 히어로를 신뢰하고 키워주느냐가 곧 인간관계의 선택이 되도록 설계되어 있다.

### 하이브리드 시퀀스와 미니게임

두 루프는 종종 한 장면 안에서 겹쳐진다. 대표적인 예가 2화 말미의 도넛 가게 강도 사건이다. 플레이어는 약 5분간 진행되는 이 장면에서, 현장의 직원을 어떻게 지원할지 결정을 내리는 **동시에** 스프링클러 시스템에 침투하는 **해킹 미니게임**을 병행 플레이한다. 즉 드라마틱한 컷신을 수동적으로 보는 것이 아니라, 그 안에서 실시간 판단과 미니게임을 동시에 굴려야 한다. 이 해킹 미니게임은 QTE(퀵타임 이벤트) 성격을 띤다.

### 진행 구조

8개 에피소드의 선형 서사를 따라가되, 각 에피소드 안에 디스패칭 근무 "교대(shift)" 세션이 배치되는 구조다. 즉 TV 시리즈의 에피소드 골격(드라마 진행) 위에, 회마다 직장 업무 시뮬레이션(디스패칭)이 얹히고, 그 성과와 선택이 다음 회 드라마에 반영된다.

### UI/UX 철학과 접근성

UI는 관제 콘솔 컨셉을 그대로 살려, 콜 목록·히어로 카드·맵을 한 화면에 띄우는 대시보드형이다. 게임은 "보는 재미"와 "관리하는 재미"를 분리하지 않고, 모니터 화면 자체가 게임플레이 무대가 되게 했다. 다만 핵심 비평(4·6장 참조)은 이 디스패칭 레이어가 내러티브 결과에 충분히 깊게 연결되지 못한다는 점, 그리고 해킹 미니게임이 단조롭다는 점에 모인다.

---

## 4. 평가

### 평론 종합 점수

- **Metacritic**: PC 87/100(약 70개 리뷰), PS5 89/100(약 31개 리뷰), Nintendo Switch 2 85/100(약 8개 리뷰) 수준으로 집계되었다. (출처: Wikipedia 종합)
- **OpenCritic**: 약 119~120개 비평 기준 "Mighty" 등급, 추천율 97%, 약 98 백분위수.

### 주요 매체 리뷰

| 매체 | 점수 | 요지 |
|---|---|---|
| IGN | 9/10 | 강력한 각본과 캐스트. 다만 해킹 미니게임의 스릴 부족 지적. |
| Game Informer | 9/10 | 서사와 선택을 호평. |
| GameSpot | 8/10 | "환상적인 슈퍼히어로 TV". 글쓰기·연기 호평, "내러티브 결과(consequence)의 부족" 지적. |
| PC Gamer | 8.9/10 | Fraser Brown, 캐릭터와 각본을 극찬하되 상호작용성 강화를 아쉬워함. |
| Push Square | 8/10 | — |
| Nintendo Life | 9/10 | — |
| GamesRadar+ | 호평 | "Critical Role 팬들이여 기뻐하라 — 에피소드형 게임이 이 매력적인 부적응자 무리에 의해 영웅적으로 구원받았다." |
| Kotaku | 양가적 호평 | "재미있지만 때로 거슬리는 슈퍼히어로 활극." Invisigal 구원 서사·각본·연기를 최고의 슈퍼히어로 드라마로 평가하면서도 톤의 급변을 지적. |

비평의 공통분모는 명확하다. **각본·캐릭터·보이스 연기는 동시대 최고 수준**이라는 합의, 그리고 **게임플레이(디스패칭·미니게임)의 상호작용 깊이와 선택의 실질적 결과는 다소 얕다**는 공통된 단서다.

### 상업 지표

- **출시 10일 내 100만 장 돌파.**
- **출시 첫 달 200만 장 돌파.**
- 이후 **누적 400만 장** 판매(AdHoc 공동창립자 확인, ThisWeekInVideoGames 보도). 3년 판매 목표를 약 3개월 만에 초과 달성할 궤도라는 보도가 나왔다.
- **Steam 동시접속 최고치**: 2025년 11월 12일(최종 에피소드 출시일) **220,060명**. 내러티브 어드벤처 장르 데뷔작으로는 이례적인 수치다.

### 유저 평가

Steam에서 압도적 호평을 유지했다. 한 시점 기준 총 리뷰 약 103,816개 중 97% 긍정, 최근 30일 약 2,841개 중 95% 긍정으로 집계되었다. 즉 평론(80~90점대)보다 유저 반응이 더 뜨거운, 전형적인 "컬트·입소문" 곡선을 그렸다.

### 수상 이력

- **The Steam Awards 2025**: "Outstanding Story-Rich Game"(스토리가 풍부한 게임 부문) 수상. Game of the Year 부문 후보에도 올랐다.
- **The Game Awards 2025**: Best Debut Indie Game, Players' Voice 후보. (단, 에피소드형 일정이 심사 컷오프를 가로질러 대부분 부문에서 자격을 얻지 못했다 — 6장 참조.)
- 이후 NAVGTR, BAFTA, D.I.C.E., GDCA 등에서 다수 수상·후보 보도가 이어졌다(연기·각본·애니메이션·음향 등 — 일부는 후속 시상 시즌 진행형).

---

## 5. 성공 요인 분석 (핵심)

《Dispatch》의 성공은 단순한 "잘 만든 게임"의 결과가 아니다. 모든 신호가 "실패할 것"이라 말하던 조건에서 거둔 성공이기에, 그 요인을 분해하면 동시대 게임 비즈니스의 통념 여러 개가 깨지는 지점을 볼 수 있다.

### (1) "코미디 게임은 안 팔린다"는 통념의 정면 돌파

The GameBusiness 인터뷰에서 가장 인상적인 대목은, 투자자들이 반복적으로 코미디 요소를 만류했다는 증언이다. Nick Herman은 그들의 오해를 이렇게 정리했다 — 투자자들은 "진짜로 웃긴 게임"과 "웃기려다 실패한 게임"을 혼동했다는 것이다. Herman의 반박은 날카롭다: "엄청나게 웃기는데 아무도 안 사는 게임 같은 건 없다"(It's not like there's all these incredible, hilarious games that no-one is buying). 즉 시장에 코미디 게임이 적은 건 수요가 없어서가 아니라 잘 만들기가 어려워서이며, 잘 만들면 팔린다는 가설을 《Dispatch》가 입증했다. CEO Michael Choung 역시 코미디를 "또 하나의 리스크 요인"으로 얹는 데 신중했다고 인정했다.

### (2) 형식 자체의 부활 — 에피소드형 내러티브 게임의 재발명

Telltale이 2018년 붕괴한 뒤, "선택 기반 에피소드 어드벤처"는 한물간 형식으로 취급받았다. 《Dispatch》는 이 형식을 그대로 답습하지 않고 두 가지로 재정의했다.

첫째, **TV 편성식 주간 출시 전략**이다. 8화를 매주 두 편씩 4주에 걸쳐 공개하는 방식은, 《Invincible》 같은 프레스티지 애니메이션의 주간 시청 리듬을 차용한 것이다. 이는 "매주 다음 화를 기다리는" 화제성과 커뮤니티 토론(누구와 로맨스했나, 누구를 신뢰했나)을 매주 재점화시켜, 출시 기간 내내 화제성을 지속시켰다. Steam 동접 최고치가 마지막 에피소드 출시일에 찍힌 것이 그 증거다.

둘째, **디스패칭이라는 게임플레이 레이어 추가**다. 순수 클릭형 내러티브였던 Telltale 게임과 달리, 실시간 관제 시뮬레이션을 얹어 "게임으로서 할 것"을 만들었다. 이는 "보기만 하는 게임"이라는 Telltale식 비판을 일부 흡수한 디자인적 응답이다.

### (3) 보이스 캐스팅과 Critical Role 효과

애런 폴·로라 베일리·제프리 라이트라는 A급 보이스 캐스트는 작품의 프레스티지 톤을 단숨에 끌어올렸다. 그러나 마케팅·자금 양면에서 더 결정적이었던 것은 **Critical Role**과의 결합이다. Critical Role의 핵심 성우(매튜 머서·트래비스 윌링엄·에린 이베트)가 출연했고, 2025년 7월 Critical Role Productions가 파트너십을 발표하며 개발 막바지 자금을 댔다(자세히는 아래). 수백만 규모의 충성도 높은 Critical Role 팬덤은 출시와 동시에 강력한 초기 관객층이 되어 주었다. Variety는 이를 Critical Role의 "첫 비디오 게임" 진출로 보도했다.

### (4) The Game Awards 2024라는 변곡점

이 게임의 운명을 바꾼 단일 사건은 **2024년 The Game Awards 공개**다. Choung의 회고: "우리는 거래(딜)도 없이 The Game Awards에 있었다"(We were at The Game Awards without a deal). TGA 노출 직후 위시리스트가 급증했고, 그 데이터가 투자자 신뢰를 만들었다. Herman은 단언한다 — Critical Role의 지원과 2024 TGA 출연이 없었다면 "《Dispatch》가 세상에 나올 수 있었을지 모르겠다"(I don't know that Dispatch would've made it). 즉 쇼케이스 노출 → 위시리스트 스파이크 → 투자 확보라는 현대 인디 게임의 생존 메커니즘이 교과서적으로 작동한 사례다.

### (5) 자체 퍼블리싱과 통제권

AdHoc은 Telltale 시절 "외주(work for hire)"와 창작 통제권 상실의 좌절을 겪었고, Telltale Games와 《The Wolf Among Us 2》를 협업하다 창작 통제권 분쟁으로 결별했다. 《Dispatch》는 자체 퍼블리싱으로 통제권을 지켰다. Herman은 "왜 우리가 다시 퍼블리셔와 일하겠는가"라며 자체 퍼블리싱 기조를 분명히 했다(단, 그는 자체 퍼블리싱이 예상보다 훨씬 복잡했다고도 인정했다 — Telltale 경험이 오히려 오판을 낳았다는 솔직한 술회).

### (6) 동시기 작품 대비 차별점

2025년 슈퍼히어로 콘텐츠는 포화 상태였고 "히어로 피로증(superhero fatigue)"이 회자되던 시기다. 《Dispatch》는 정면 액션 영웅물이 아니라 **영웅을 "배치하는 관리자"의 시점**, 즉 액션 바깥의 노동·관계·관료제를 그림으로써 차별화했다. ComicBook은 이 작품이 자신의 "슈퍼히어로 피로증을 완화시켰다"고 적었다. 게임 시장에서도, 같은 시기의 대형 내러티브 게임들이 대부분 일괄 출시 형태였던 반면, 주간 TV 편성 방식을 채택한 거의 유일한 사례였다.

### 개발사(struggle)와 방법론 — 7년의 생존

이 모든 성공 요인은 7년간의 생존 위에 서 있다. AdHoc은 2018년 설립 후, 처음엔 ESPN의 "This Is SportsCenter" 광고에서 영감받아 《Dispatch》를 **라이브 액션**으로 기획했고 2020년 3월 제작에 들어갔으나 코로나로 중단되었다. 이후 애니메이션으로 방향을 틀었고, 그 사이 퍼블리셔가 프로젝트를 손에서 놓아 자금줄이 끊기는 위기도 있었다. CEO Choung은 위기의 연속을 두고 "《Final Destination》 시리즈를 통째로 만들 수 있을 정도"라고 농담했다. 창립자들은 30명의 직원을 지키기 위해 6개월간 자신들의 급여를 포기하기도 했다(Wikipedia). Critical Role CEO이자 성우인 Travis Willingham이 (출연 배우 Laura Bailey를 통해 프로젝트를 접하고) 파트너십을 제안했고, TGA 이후 협상이 가속되어 막바지 자금이 들어왔다. "지난 7년간 컨퍼런스를 돌며 다음 6개월을 버틸 돈을 찾았다… 지옥이었다"는 Herman의 문장이 이 작품의 진짜 배경이다.

---

## 6. 비평적 시각 / 한계 / 논란

### 디자인적 약점

비평가들이 가장 일관되게 짚은 약점은 **상호작용성과 선택 결과의 얕음**이다.

- GameSpot은 글쓰기·연기를 칭찬하면서도 "내러티브 결과(consequence)의 부족"을 단점으로 들었다. 즉 선택이 드라마틱하게 느껴지지만, 실제로 분기가 깊거나 결과가 크게 갈리지는 않는다는 비판이다.
- IGN은 해킹 미니게임에 "스릴이 부족하다"고 지적했고, PC Gamer의 Fraser Brown도 캐릭터·각본을 극찬하면서 상호작용성이 더 강했으면 좋았겠다고 아쉬워했다.
- Kotaku는 톤의 진폭이 채찍질처럼 급변(whiplash-inducing)하며 일부 코미디가 "거슬릴 정도로 도발적"이라고 보았다. 작품의 에지(edgy) 유머는 호불호가 갈리는 지점이다.

요약하면 《Dispatch》는 "게임으로서의 깊이"보다 "인터랙티브 드라마로서의 완성도"로 사랑받는 작품이며, 디스패칭 시뮬레이션 레이어가 서사 결과와 더 단단히 맞물렸다면 더 완전했으리라는 데 이견이 적다.

### 논란 1 — Nintendo Switch 검열 사태

2026년 1월 28일 Switch / Switch 2 eShop 출시판에서, 누드·성적 묘사·외설적 제스처가 포함된 일부 장면이 **기본값으로 검열(검은 가림막)**되었고, **이를 끌 토글이 없었다**. PS5·PC판에서는 선택 가능한 옵션이었던 검열이 Switch판에서는 강제되었던 것이다. 두 로맨스 대상 Invisigal과 Blonde Blazer 관련 장면이 가려졌고, 가운뎃손가락 제스처까지 가림막 처리되었다는 보도가 있었다(Nintendo Life). 사전에 고지되지 않았다는 불만 속에 eShop 환불 요청이 대거 발생했다.

AdHoc은 처음 검열을 "Nintendo의 콘텐츠 기준" 탓으로 돌렸으나, Nintendo는 자신들이 게임 콘텐츠를 직접 수정하지 않는다고 해명했고, 이후 정황상 검열 결정의 책임이 AdHoc 측에 있다는 보도가 이어졌다(The Escapist, VGC). AdHoc은 결국 "사람들이 화낼 권리가 있다", "우리는 배울 게 많다"는 취지로 사과했고, 고의로 숨길 의도는 없었다고 해명했다. 2026년 2월 15일 검열된 장면 중 하나(Invisigal의 꿈 시퀀스)를 복원했고, 3월에도 Nintendo와 복원 작업을 계속 중이라 재확인했다. 한편 Xbox Series X/S판은 PS5·PC와 동일한 무검열판으로 출시될 것이라고 밝혔다.

### 논란 2 — 비동의 키스(non-consensual romance) 논란

2025년 11월 12일 7·8화 출시 후, 7화에서 Invisigal이 Robert에게 동의 없이 키스를 시도하는 장면이 "비동의 로맨스"라며 일부 플레이어의 항의를 받았다. 특히 Blonde Blazer 로맨스 노선을 택한 플레이어들에게 이 장면이 강제되는 점이 문제로 지적되었다. AdHoc은 11월 19일 패치 1.0.16409를 내, 특정 조건이 충족되지 않으면 해당 장면이 발생하지 않도록 "조건부 결과 조정(conditional outcome tuning)"을 적용했고, 이는 플레이어들에게 긍정적으로 받아들여졌다.

### 논란 3 — The Game Awards 자격 논란

에피소드형 출시 일정의 부작용도 있었다. 2025년 출시작임에도, 8화 전체가 TGA 심사 투표 기간 컷오프를 가로질러 공개되는 바람에, 《Dispatch》는 2025 TGA의 대부분 부문에서 후보 자격을 얻지 못하고 Best Debut Indie와 Players' Voice 두 부문에만 올랐다. 개발진은 "사람들이 절반만 플레이한 상태에서 투표가 진행됐고, 그 절반만 본 사람들이 Best Debut Indie 후보로 올려줬다"고 토로했다. 결국 작품은 2026 TGA에서 다시 자격을 얻게 되어, 출시 시기와 시상 제도의 불일치라는 구조적 문제를 드러냈다(Push Square, Dexerto).

---

## 7. 영향과 유산

### 장르에 미친 영향 — 에피소드형 내러티브 게임의 부활 선언

《Dispatch》의 가장 큰 산업적 의미는, "선택 기반 에피소드 어드벤처는 죽었다"는 통념을 상업적으로 반증했다는 데 있다. Telltale 붕괴 이후 7년, 그 형식을 만든 사람들이 같은 형식으로 데뷔작 400만 장을 팔았다. GamesRadar+가 "에피소드형 게임이 영웅적으로 구원받았다"고 쓴 것은 과장이 아니다. Inverse 등은 이 작품이 "Telltale 게임이 얼마나 그리웠는지 깨닫게 했다"고 적었다. 향후 내러티브 어드벤처 장르가 "주간 편성형 출시 + 가벼운 게임플레이 레이어 + 프레스티지 보이스 캐스트"라는 《Dispatch》 모델을 참조점으로 삼을 가능성이 크다.

### 인디·AA 비즈니스에 주는 교훈

이 작품은 동시대 인디·AA 게임 비즈니스의 여러 통념을 동시에 반박한 사례로 인용된다.

- **코미디 게임도 잘 만들면 팔린다.**
- **에피소드형 내러티브 게임은 끝나지 않았다.**
- **쇼케이스(TGA) 노출 → 위시리스트 → 투자**라는 인디 생존 공식이 실제로 작동한다.
- **자체 퍼블리싱으로도 글로벌 메가히트가 가능하다** — 단, 자체 퍼블리싱의 운영 복잡성은 별개의 난제다.

특히 "7년간 폐업 직전에서 자급여 포기로 버틴 30인 스튜디오"라는 서사는, 신생 스튜디오의 생존 전략 사례로 두고두고 회자될 만하다.

### Critical Role의 미디어 확장과 후속 전개

Critical Role Productions에게 《Dispatch》는 게임 사업 진출의 교두보다. 두 회사는 《Dispatch》뿐 아니라 Critical Role 세계관 기반의 **첫 비디오 게임**을 함께 개발 중이라고 발표했다(Variety). 또한 《Dispatch》 자체에 대해서도 머천다이즈, 테이블탑 게임, 애니메이션 시리즈 등 미디어 확장이 Critical Role과의 파트너십 아래 논의되고 있다. 창립자 Nick Herman과 Pierre Shorette는 **두 번째 시즌** 가능성을 검토 중이며, 애런 폴도 추가 시즌에 대한 의욕을 밝혔다. 즉 《Dispatch》는 단발 게임을 넘어 IP·프랜차이즈로 확장될 잠재력을 가진다.

### 문화적 의미

"슈퍼히어로 피로증"이 만연하던 2025년, 《Dispatch》는 액션 영웅이 아니라 영웅을 "배치하는 직장인"의 시점으로 슈퍼히어로 장르를 재해석함으로써 신선함을 회복시켰다. 《The Boys》·《Invincible》이 그래픽 노블·TV에서 한 일(영웅 신화의 탈신화화)을, 게임은 "관료제·노동·번아웃"이라는 직장 시트콤의 렌즈로 수행했다. 슈퍼히어로 서사를 노동 서사로 비틀었다는 점에서, 장르 비평으로서도 의미가 있다.

---

## 8. 부록

### 핵심 통계 표

| 항목 | 수치 / 내용 | 출처 |
|---|---|---|
| 개발사 / 퍼블리셔 | AdHoc Studio (자체 퍼블리싱) | Wikipedia |
| 엔진 | Unreal Engine 4 | Wikipedia |
| 출시 (PC/PS5) | 2025-10-22 ~ 11-12, 8화 주간 단계 출시 | Wikipedia / Game8 |
| 팀 규모 | 약 30명 (2024 기준) | The GameBusiness |
| 예산 등급 | "AA 영역 중하단" | The GameBusiness |
| Metacritic | PC 87 / PS5 89 / Switch2 85 | Wikipedia |
| OpenCritic | "Mighty", 추천율 97%, 약 98 백분위 | OpenCritic |
| Steam 유저 평가 | 누적 약 97% 긍정(약 10.4만 리뷰) | Steam |
| Steam 최고 동접 | 220,060명 (2025-11-12) | SteamDB |
| 판매량 | 10일 100만 / 1달 200만 / 누적 400만 | ThisWeekInVideoGames 등 |
| 주요 수상 | Steam Awards 2025 Outstanding Story-Rich Game | The Steam Awards |
| Critical Role 파트너십 발표 | 2025-07-21 | Variety |

### 디스패칭 5대 스탯

| 스탯 | 역할 |
|---|---|
| Combat | 전투형 사건 대응 |
| Vigor | 체력/지속력 |
| Mobility | 기동성/속도 |
| Charisma | 설득/사회적 사건 |
| Intellect | 지능/기술 사건 |

### 주요 보이스 캐스트

| 캐릭터 | 성우 |
|---|---|
| Robert Robertson III / Mecha Man | Aaron Paul |
| Courtney / Invisigal | Laura Bailey |
| Chase / Track Star (Starblazer) | Jeffrey Wright |
| Elliot Connors / Shroud | Matthew Mercer |
| Mandy / Blonde Blazer | Erin Yvette |
| Katon-Ur / Phenomaman | Travis Willingham |
| 카메오 | jacksepticeye, MoistCr1TiKaL, Joel Haver, Alanah Pearce, Yung Gravy, Thot Squad |

### 주요 인터뷰 / 참고 자료 (영어권 중심)

- The GameBusiness, "Dispatch developer: We were told comedy games don't sell" — 개발 7년, 코미디 통념, TGA 2024, Critical Role 자금. https://www.thegamebusiness.com/p/dispatch-developer-we-were-told-comedy
- Variety, "Critical Role to Start Development on Their First Video Game in Partnership With AdHoc Studio (EXCLUSIVE)" — 파트너십 보도. https://variety.com/2025/digital/news/critical-role-first-video-game-development-adhoc-studio-1236463963/
- Inverse, "The Best Superhero Game Of The Year Succeeded Against All Odds" — 개발자 인터뷰. https://www.inverse.com/gaming/dispatch-developer-interview
- ThisWeekInVideoGames, "Dispatch Has Now Sold 4 Million Copies, AdHoc Studio Co-Founder Confirms" — 누적 판매. https://thisweekinvideogames.com/news/dispatch-has-now-sold-4-million-copies-adhoc-studio-confirms/
- Wikipedia, "Dispatch (video game)" — 크레딧·줄거리·출시·논란 종합. https://en.wikipedia.org/wiki/Dispatch_(video_game)
- Kotaku, "Dispatch Review: A Fun, Sometimes Obnoxious Superhero Romp." https://kotaku.com/dispatch-review-adhoc-studios-all-8-episodes-finale-2000644106
- GameSpot, "Dispatch Review - Fantastic Superhero TV." https://www.gamespot.com/reviews/dispatch-review-fantastic-superhero-tv/1900-6418442/
- GamesRadar+, "Dispatch review." https://www.gamesradar.com/games/adventure/dispatch-review/
- Nintendo Life, "PSA: Dispatch's 'Visual Censorship' Settings Can't Be Removed On Switch." https://www.nintendolife.com/news/2026/01/psa-dispatchs-visual-censorship-settings-cant-be-removed-on-switch
- VGC, "Dispatch is censored on Nintendo Switch and Switch 2, and this might be the reason why." https://www.videogameschronicle.com/news/dispatch-is-censored-on-nintendo-switch-and-switch-2-and-this-might-be-the-reason/
- Push Square, "Episodic Sensation Dispatch Will Be Eligible for The Game Awards 2026." https://www.pushsquare.com/news/2025/12/episodic-sensation-dispatch-will-be-eligible-for-the-game-awards-2026
- SteamDB, Dispatch Charts (동접 통계). https://steamdb.info/app/2592160/charts/
- Dispatch Wiki (Fandom), "Dispatching" — 디스패칭 메카닉 상세. https://dispatch.fandom.com/wiki/Dispatching

### GDC / 포스트모템

본 분석 시점(2026년 6월) 기준 공식 GDC 포스트모템 강연은 확인되지 않았으나, The GameBusiness·Inverse 등의 개발자 인터뷰가 사실상의 포스트모템 역할을 한다. 7년 개발사·코미디 게임 통념·자체 퍼블리싱·TGA 효과·Critical Role 자금에 관한 1차 증언은 위 인터뷰들에 집중되어 있다.

---

*본 분석서는 영어권 매체·공식 인터뷰·위키 자료를 토대로 작성되었다. 판매·동접 수치와 점수는 보도 시점 기준이며, 일부 시상 결과는 후속 시즌 진행형이다.*
