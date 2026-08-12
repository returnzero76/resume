# 강지환 이력서 — 마스터 콘텐츠 (모든 디자인 변형의 단일 소스)

> 공개 범위: 이메일 + GitHub만. 전화번호/생년월일/주소 제외.
> 사진: assets/profile_4.png (세로 700x872), assets/profile_2.jpg (와이드 고해상 3681x4471)

## Bio

**강지환 (Jihwan Kang)**
Software Engineer — Android · Cross-platform · AI Agent Platform

- Live in Seoul
- E. jihwan76@gmail.com
- GitHub. github.com/returnzero76

2011년부터 Android Application을 개발해왔습니다. Native(Kotlin/Compose)와 Cross-platform(React Native) 개발부터 CI/CD 인프라, AI 자동화 커맨드까지 — 기능 개발과 개발 흐름 개선을 함께 하는 개발자입니다.

AI, Mobility, E-commerce, Multimedia 등 다양한 도메인을 경험했고, JAVA로 시작해 Kotlin 중심으로, 최근에는 TypeScript(React Native)와 Go(백엔드 플랫폼)까지 스택을 넓히고 있습니다. 현재보다는 미래를 위한, 다른 사람도 이해하기 쉬운 코드를 만드는 것을 좋아합니다.

## Career Timeline (요약)

| 회사 | 기간 | 직급/역할 |
|---|---|---|
| SK Telecom | 2018.04 ~ 현재 | Manager — 에이닷(A.) Client 개발 |
| Tmon | 2017.06 ~ 2018.03 | Assistant Manager — Android 앱 개발 |
| Titan Platform | 2017.01 ~ 2017.06 | Manager — Android 서비스 앱 개발 |
| Tmon | 2015.06 ~ 2017.01 | Assistant Manager — Android 앱 개발 |
| Pantech | 2011.01 ~ 2015.05 | 전임연구원 — Android Music 앱 개발 |
| LG Electronics | 2010.09 ~ 2010.12 | 인턴 — Blu-ray player SW 개발 |

## Education & Certification

- 광운대학교 전자통신공학 (2004.03 ~ 2011.02) — 3.64/4.5
- 정보통신기사 (한국산업인력공단, 2010)

## Skills

**Languages**: Kotlin, TypeScript, Java, Go
**Android**: Jetpack Compose, Coroutines/Flow, Hilt/Koin, 멀티모듈 Clean Architecture(MVVM+UseCase), WorkManager, Navigation/DeepLink, ExoPlayer, Room, Paging
**Cross-platform**: React Native (New Architecture — TurboModule/Codegen), Expo, react-native-gesture-handler, feature-sliced design-system
**Voice AI**: NUGU SDK(ASR/TTS/Directive/Agent), Wake-up Word 엔진, VoiceChrome UI
**Web/Backend(최근)**: Next.js, Go(Huma API), Langfuse 관측성 연동
**CI/CD & Quality**: GitLab CI, Jenkins, Fastlane, Kover(coverage), detekt, JUnit/MockK/Espresso, ProGuard, Gradle Version Catalog
**AI Developer Tools**: Claude Code 커스텀 파이프라인(JIRA→코드수정→MR 자동화), 모듈 인덱스 시스템, Speckit 스펙 주도 개발
**Tools**: Git, GitLab/GitHub/Bitbucket, JIRA, Firebase, Figma, Slack

## Work Experience (상세, 최신순)

### Agent OS — AI Agent 거버넌스 플랫폼 (2026.06 ~ 현재) · SK Telecom
조직 내 흩어진 AI Agent들을 한 곳에서 등록·추적·통제하는 거버넌스 플랫폼 개발 (Go + Next.js 모노레포).
- Go 백엔드(control-plane) observability pod 개발: Langfuse/Pathfinder trace 조회 연동 — cursor 페이징, 오류 계약 매핑, 지수 백오프 재시도, BDD tests-first(20 스펙)
- Next.js 콘솔 model-evaluation 화면 개발 및 리팩토링, flaky test 근본 해결
- Speckit 기반 스펙 주도 개발 문화 실천: spec→plan→tasks→구현, GitLab 이슈/Epic 양방향 연결 자동화
- agent-os-skills: 팀 생산성 자동화 스킬 개발 — daily-briefing(Slack Block Kit 발송), spec-tracker(스펙 번호 충돌 자동 재번호) 등 (49 커밋)

### 에이닷 A. Android 앱 (2022.05 ~ 현재) · SK Telecom
SKT AI 개인비서 '에이닷' Android 클라이언트. 대규모 멀티모듈(app/feature/domain/data/core) 프로젝트, 4년간 2,990 커밋(기여 2위권).
- **AI 노트 도메인 리드 (2025.08~)**: 통화녹음/파일 기반 노트 생성 파이프라인, 폴더/휴지통/공유 노트 체계 신규 구축, WorkManager 백그라운드 처리, 파일 공유 인텐트 수신 개발
- **React Native 하이브리드 전환 (2026)**: New Architecture TurboModule 브릿지 아키텍처 설계·구현(EventFlow+ReactViewModel+ReactFragment+라우팅), 전환 후 레거시 Native 코드 정리
- **게임 서비스 (2022~2024, 최대 기여 영역)**: 게임홈/리스트/상세/리더보드 전체 개발, XML→Compose 전면 전환(Material3 제약 해결, Foldable 대응 nestedScroll 경합 회피)
- **AI 포토 (2024)**: 프로필 이미지 생성 플로우, 외부 이미지 생성 SDK 연동, UiState 세분화
- **A.tv (2022~2025)**: 외부 AAR SDK v0.0.7→v244+ 수십 차례 통합, 본인인증 flow, PIP/폴더블/멀티윈도우 대응
- **WebView 플랫폼 공통화**: webkit 모듈 설계(WebResultProvider, permission/activity result), 영어학습 JS Bridge, 딥링크 도메인 검증 등 보안 이슈 해결
- **테스트 인프라 구축 (2024.11~2025.03)**: UnitTest report 통합 시스템, Kover coverage 룰셋, CI 파이프라인 테스트 옵션, Slack 알림 연동
- **CI 자동화 (2026)**: js submodule pointer 무결성 검사, 자동 bump Pipeline Schedule, Debug 빌드 API 프록시 개발자 메뉴
- **AI 개발 워크플로 도입 (2026)**: Claude Code 모듈 인덱스 시스템 설계(대규모 멀티모듈을 LLM이 탐색 가능하게), JIRA→수정→MR 자동화 bugfix 파이프라인 커맨드 개발

### adot-react-native — 에이닷 공용 RN 워크스페이스 (2026.03 ~ 2026.05) · SK Telecom
Android/iOS 본체에 submodule로 embed되는 크로스플랫폼 공용 코드베이스 (TypeScript). 167 커밋.
- Auto(차량 연동) RN 화면 3종 전면 구현: OTP/차량리스트 — TurboModule Spec 설계, first-mount race 해결
- AI 노트 RN 전환: 공용 noteList 컴포넌트/훅 설계(NotePagingList, SwipeableNoteRow, useNoteListPaging)
- Pull-to-Refresh 제스처 경합 해결: RNGH PanGestureHandler 기반 재구현 → design-system 공용 컴포넌트로 승격
- Native Compose 화면과의 pixel parity 검증, 다크모드 토큰, 접근성(a11y) lint 게이트 대응, Expo SDK 55 도입

### Tmap x Adot 음성비서 마이그레이션 (2025.03 ~ 2025.08) · SK Telecom
Tmap 앱 탑재 음성비서를 NUGU→에이닷 기반으로 마이그레이션하는 프로젝트의 레퍼런스 샘플 앱. Initial commit부터 시작한 리드 개발 (240 커밋, 전체의 41%).
- 신규 프로젝트 0→1 부트스트랩: core/presentation 모듈 아키텍처 설계, Adot Login SDK 인증 통합
- NUGU SDK 통합·커스터마이징: SpeechRecognizer trigger, AudioSpeaker custom, 멀티턴 상태머신 이슈 해결
- Wake-up Word 엔진 적용(멀티 트리거 모델), EPD Timeout 튜닝
- VoiceChrome(음성 UI) 구현: Lottie 상태별 애니메이션, 유지 정책, TmapCommand Directive viewer, 발화가이드 Chips
- 5개월간 v0.3.0→v1.12.0 10회+ 배포, 파트너사 참조용 코드 품질 관리 + Confluence 연동 가이드 문서 저술 (Sample Guide 위키 10여 페이지)

### TimeTree x Adot Android 샘플 (2025.03 ~ 2025.10) · SK Telecom
TimeTree 제휴 서비스용 Android 샘플 앱 (272 커밋).
- 채팅 화면 개발: Reactive 메시지 연결, Streaming 로딩 뷰, 채팅방 enter/exit 애니메이션

### Btv NUGU Android (2020.11 ~ 2022.04) · SK Telecom
Btv 내 NUGU 사용을 위한 Android 앱. UHD/AI/Smart 등 모든 Btv 디바이스에 NUGU 탑재.
- 신규 디바이스 출시(AI2 MAX, AI2 AndroidTv) & 유지보수, 백그라운드 service component MVVM 적용
- 15개+ model flavor 빌드 효율화: Fastlane 작성 & Jenkins 연동, 개발자 Debug mode 개발

### Tmap Taxi Android (2020.03 ~ 2020.11) · SK Telecom
택시 승객앱 신규 기능 개발 & 유지보수.
- 업무용 택시/법인카드 결제, SK pay 가입·카드연동·결제, 쿠폰 적용 개발
- 승객 호출 화면 전면 Renewal(첫화면/출발지/목적지/경로/결제), Java→Kotlin 전환, MVVM 적용
- Base/Tmap SDK/Network 모듈화, Fastlane build script + Slack 연동

### NUGU AI Mobile Android (2018.04 ~ 2020.11) · SK Telecom
NUGU AI 서비스용 3rd party 서비스 연결·디바이스 연결을 지원하는 Android 앱.
- App Renewal 2.0: 처음부터 재개발, Java→Kotlin 전환
- 디바이스 연결(Bluetooth/AP/OTP/Broadcast) — AI Speaker, Btv 등, TID 연동
- Melon/Flo/오디오북 등 멀티미디어·쇼핑·금융 서비스 도메인 연결, Tmap 인터페이스 협의/개발
- Base/Call/App 모듈 분리, 전 화면 MVVM(RxKotlin, LiveData), DI(Koin), MockK 도입 & 유닛테스트
- 2019 Google I/O 참여 & 사내 공유

### Tmon Android (2015.06 ~ 2017.01, 2017.06 ~ 2018.03) · Tmon
소셜커머스 Tmon Android 앱 전반 개발.
- 쇼핑 카테고리 구조 개편 Renewal(3개월), 메인 첫화면(추천탭) Renewal(3개월) — lazy loading으로 진입 속도 개선
- Time Attack deal, 배송 상태 AppWidget, Custom view(Expandable GridView, Pull to Refresh 등)
- Jenkins+Instrumentation test+Slack 자동화 테스트(원클릭 결과 공유), EventBus 자체 개발
- SharedPreference 분리·commit 최소화, 7개 tracking module 통합 리팩토링, ListView→RecyclerView 등 컴포넌트 현대화

### Winvention US/KR (2017.01 ~ 2017.06) · Titan Platform
멀티미디어(Video/Webtoon) 서비스 US향 앱을 개발 초기부터 참여.
- 단일 Activity + 전 화면 Fragment 구조(like YouTube), 화면 이동 Movement 모듈 개발
- File upload Background Service, Jsoup+Volley 문서 파싱, ExoPlayer custom + 자체 DRM(TCI) 적용
- KR향: 검색 WebView→Data binding Native 전환(속도 개선), Firebase/FCM/IGAWorks 연동

### Music Player & Audio Effect (2011.01 ~ 2015.05) · Pantech
Pantech Android 디바이스 preload Music Player 앱 개발.
- Android Media Provider Framework 분석, Music DB/Albumart cache 구조, AppWidget 2종 + U+Box 위젯
- Melon/OllehMusic/YouTube 온라인 서비스 연동, 국내 전모델 + 일본/베트남/대만 preload, Android 2.2~5.0 OS 업그레이드 대응
- Audio Effect 앱: 사용자 설정 Equalizer, 장르별 Auto Preset, QSound/NXP 3rd party 통합
- Tag Editor Java Library 자체 개발: MP3(ID3)/FLAC(Vorbis) spec 분석, TEXT/LYRICS/ALBUMART read/write, charset encoding 자동 분석

### Blu-ray Player (2010.09 ~ 2010.12) · LG Electronics (인턴)
- Blu-ray player device SW: Text 표시 UI 개발(C), 다국어 지원 추가, Turnkey base 모델 작업

## Highlights (숫자로 보는 경력 — 히어로/통계 섹션용)

- 15+ 년 소프트웨어 개발 (Android 2011~)
- 3,700+ 커밋 (최근 4년, 에이닷 관련 repo 합산)
- 7개 서비스 도메인 리드 (게임/포토/노트/Auto/음성비서/TV/교육)
- 4번의 기술 전환 주도: XML→Compose, Native→RN 하이브리드, 무테스트→커버리지 체계, 수동 개발→AI 파이프라인
