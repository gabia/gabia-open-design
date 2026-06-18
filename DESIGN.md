# Design System Inspired by Gabia

> Category: IT Infrastructure & Cloud Services
> B2B/B2C Korean IT platform. Information-dense layout, trustworthy brand blue, clear service taxonomy.

## 1. Visual Theme & Atmosphere

가비아의 웹 디자인 언어는 신뢰성과 실용성을 우선하는 정보 중심 시스템입니다. 한국 SMB와 기업 고객을 대상으로 하며, 도메인·호스팅·클라우드·그룹웨어를 한 곳에서 제공하는 통합 IT 인프라 허브로서의 역할을 수행합니다.

상단의 네이비 유틸리티 바와 흰 배경의 GNB가 명확한 계층을 형성하고, 서비스 카테고리 중심의 내비게이션이 사용자를 빠르게 원하는 서비스로 안내합니다. 메인 히어로는 도메인 검색 바를 중심으로 구성되어, 가비아의 핵심 비즈니스를 즉시 액션 가능한 형태로 제시합니다.

**Key Characteristics:**
- 흰 배경(`#ffffff`) + 연한 파란 회색 서피스(`#f4f7fb`)의 명료한 2단계 라이트 레이어
- 가비아 브랜드 블루(`#0067CC`)를 액션과 링크에 일관되게 사용
- 상단 네이비 유틸리티 바(`#1a2d4e`) + 흰 GNB의 2단 내비게이션 구조
- 도메인 검색 바가 히어로의 핵심 인터랙션 요소
- 서비스 카드 4열 그리드 — 명확한 아이콘 + 서비스명 + 한 줄 설명 구조
- 신뢰 지표(등록 도메인 수, 운영 연수, SLA) 수치로 브랜드 신뢰성 강화
- 고객 지원 섹션에 전화번호·운영 시간을 네이비 패널로 명확히 표시
- 정보 밀도 높은 레이아웃, 과도한 여백 없이 실용적인 컴팩트 구성

## 2. Color Palette & Roles

> **Source:** `https://www.gabia.com/`

### Primary
- **가비아 블루** (`#0067CC`): 브랜드 컬러. 주요 액션 버튼, 링크, 강조 요소.
- **가비아 네이비** (`#1a2d4e`): 상단 유틸리티 바, 지원 패널, 깊이감이 필요한 다크 섹션.
- **Near-Black** (`#111827`): 기본 텍스트.

### Secondary & Accent
- **블루 호버** (`#0058b0`): 블루 버튼 호버 상태.
- **블루 액티브** (`#004a94`): 블루 버튼 클릭/눌림 상태.
- **블루 라이트** (`#e8f1fb`): 아이콘 배경, 배지 배경, 서브 강조 표면.
- **가비아 오렌지** (`#f97316`): NEW 배지, 이벤트 강조 포인트 (절제하여 사용).

### Surface & Background
- **Pure White** (`#ffffff`): 기본 페이지 배경, 카드 배경.
- **Soft Blue-Gray** (`#f4f7fb`): 기능 섹션, 서비스 그리드 배경.
- **Near-White Warm** (`#f9fafb`): 폼 섹션, 조용한 거래 표면.

### Neutrals & Text
- **Body Gray** (`#374151`): 보조 본문 텍스트.
- **Muted Gray** (`#6b7280`): 설명 문구, 헬퍼 텍스트.
- **Meta Gray** (`#9ca3af`): 플레이스홀더, 최하위 메타 정보.
- **Border** (`#e5e7eb`): 기본 구분선, 카드 테두리.
- **Soft Border** (`#f0f2f5`): 아주 연한 구분선.

### Semantic
- **Success** (`#16a34a` / bg: `#dcfce7`): 정상 운영 상태, 완료 메시지.
- **Warning** (`#f59e0b` / bg: `#fef3c7`): 주의 배지.
- **Danger** (`#ef4444`): 오류 메시지, 필드 에러.

## 3. Typography Rules

### Font Family
- **Primary:** `Pretendard`, `Apple SD Gothic Neo`, `Noto Sans KR`, `-apple-system`, `sans-serif`
- **Mono:** `JetBrains Mono`, `SF Mono`, `ui-monospace`

### Hierarchy
| Role | Size | Weight | Line Height | Notes |
|------|------|--------|-------------|-------|
| Hero Display | 52px | 700 | 1.2 | 히어로 메인 타이틀 |
| Section Display | 38px | 700 | 1.25 | 섹션 헤딩 |
| Card Title | 22px | 600 | 1.35 | 서비스/카드 제목 |
| Sub Heading | 18px | 600 | 1.4 | 서브 헤딩 |
| Lead Text | 18px | 400 | 1.65 | 히어로 본문 |
| Body | 15px | 400 | 1.6 | 기본 본문 |
| UI Body | 16px | 400–600 | 1.5 | 버튼, 입력 UI |
| Small UI | 13px | 400–600 | 1.5 | 내비게이션, 라벨, 헬퍼 |
| Micro | 12px | 400–600 | 1.5 | 배지, 법적 고지 |

### Principles
- `word-break: keep-all` 적용 — 한국어 단어 중간 줄바꿈 방지
- 헤딩에 `letter-spacing: -0.02em` 적용으로 화면에서 자연스럽게 읽히도록
- 폰트 굵기 700(헤딩), 600(서브/버튼), 500(라벨), 400(본문)의 4단계 계층

## 4. Component Stylings

### Buttons
- **Primary:** `#0067CC` 배경, `#ffffff` 텍스트, `6px` 라디우스. 메인 CTA.
- **Secondary:** 흰 배경 + `#0067CC` 테두리 + `#0067CC` 텍스트. 보조 액션.
- **Ghost:** 흰 배경 + `#e5e7eb` 테두리 + `#374151` 텍스트. 중립 액션.
- **Pill CTA:** `100px` 라디우스 캡슐형. 히어로 영역 주요 CTA.
- **Large:** `btn-lg` 확장 — `padding: 13px 28px`, `font-size: 16px`. 폼 제출 버튼.

### Cards
- **기본 카드:** 흰 배경, `#e5e7eb` 테두리, `12px` 라디우스. 호버 시 블루 그림자.
- **서비스 카드:** 중앙 정렬, 아이콘 + 제목 + 설명 구조. 호버 시 `translateY(-2px)`.
- **Feature 카드:** 블루 그라디언트 배경(`#e8f4ff → #f0f7ff`), `16px` 라디우스, 기본 그림자.
- **지원 패널:** 네이비(`#1a2d4e`) 배경, 2열 그리드 레이아웃. 전화번호 강조 표시.

### Navigation
- **상단 유틸리티 바:** 네이비 배경 34px. 로그인/회원가입/고객센터 링크.
- **GNB:** 흰 배경 60px. 가비아 블루 로고 + 서비스 메뉴 + 로그인/회원가입 버튼.
- 메뉴 호버: 연한 서피스 배경 + 블루 텍스트 전환.

### Domain Search Bar
- 가비아의 시그니처 인터랙션 요소.
- `#0067CC` 2px 테두리 박스, 좌측 `WWW.` 접두사, 검색 버튼.
- `max-width: 560px` 제한, 모바일에서도 전체 너비 활용.

### Inputs & Forms
- `border: 1px solid #e5e7eb`, 호버 시 `#9ca3af`, 포커스 시 `#0067CC` + 3px 블루 포커스 링.
- 라벨 `font-weight: 600`, 헬퍼 텍스트 `font-size: 12px` `#6b7280`.

### Badges
- `badge-success`: 짙은 초록 텍스트 + 연초록 배경.
- `badge-info`: 블루 텍스트 + 연파란 배경.
- `badge-warn`: 황갈색 텍스트 + 연노란 배경.
- `badge-new`: 흰 텍스트 + 오렌지 배경. 신규 서비스 강조.

## 5. Spacing & Layout

### Section Rhythm
- Desktop: `80px` 상하 패딩.
- Tablet: `56px`.
- Mobile: `40px`.

### Service Grid
- Desktop 4열, Tablet 2열, Mobile 2열.
- 아이콘 48×48px, `#e8f1fb` 배경, `8px` 라디우스.

### Container
- `max-width: 1200px`, 좌우 거터 24px(desktop) / 20px(tablet) / 16px(mobile).

### Whitespace
- 정보 밀도를 중시하는 레이아웃. 섹션 간 대비를 위해 배경색 전환 사용.
- 과도한 여백보다 명확한 정보 구조를 우선.

### Border Radius Scale
- `4px`: 아주 작은 태그/구분 요소.
- `6px`: 기본 버튼, 인풋 필드.
- `8px`: 도메인 검색바, 서비스 아이콘.
- `12px`: 카드 기본.
- `16px`: 피처 카드, 지원 패널.
- `100px`: 캡슐형 CTA 버튼.

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Level 0 | Flat (`#ffffff`, `#f4f7fb`) | 기본 페이지 표면 |
| Level 1 | `0 1px 3px rgba(0,0,0,0.08)` | 내비게이션, 기본 카드 |
| Level 2 | `0 4px 16px rgba(0,103,204,0.10)` | 호버 카드, 피처 카드 |
| Focus | `0 0 0 3px rgba(0,103,204,0.25)` | 키보드 포커스, 선택 상태 |

그림자는 블루 톤(`rgba(0,103,204,...)`)으로 브랜드 컬러와 일관성 유지.

## 7. Do's and Don'ts

### Do
- 가비아 블루(`#0067CC`)를 액션과 링크에 일관되게 사용.
- 도메인 검색 바를 히어로의 핵심 인터랙션으로 배치.
- 서비스 카드는 아이콘 + 제목 + 한 줄 설명의 명확한 3단 구조 유지.
- 신뢰 지표(숫자/통계)를 적극 노출하여 브랜드 신뢰도 강화.
- 고객 지원 연락처를 네이비 패널로 눈에 띄게 표시.
- `word-break: keep-all` 필수 적용.

### Don't
- 블루 외 보조 액센트 컬러를 과도하게 사용하지 않는다.
- 과도한 여백으로 정보 밀도를 해치지 않는다.
- 서비스 메뉴를 모호하게 표시하지 않는다; 카테고리 명칭을 명확히 한다.
- 히어로에서 도메인 검색 바를 생략하지 않는다 — 핵심 전환 요소.
- 오렌지 액센트를 남용하지 않는다; NEW/이벤트 전용으로 절제하여 사용.

## 8. Responsive Behavior

### Breakpoints
| Name | Width | Key Changes |
|------|-------|-------------|
| Mobile | ~639px | 유틸리티 바 숨김, 메뉴 숨김, 히어로 1열 |
| Tablet | 640px–1023px | 서비스 그리드 2열, 히어로 1열 |
| Desktop | 1024px+ | 서비스 그리드 4열, 히어로 2열 분리 |

### Korean UX Notes
- 한국어 특성상 `word-break: keep-all` 필수.
- 전화번호는 `-webkit-text-size-adjust` 고려, 자동 링크 변환 방지.
- 한국어 폰트 로딩을 위해 Pretendard 서브셋 또는 Google Fonts의 Noto Sans KR 사용 권장.

## 9. Agent Prompt Guide

### Quick Color Reference
- 브랜드 블루: `#0067CC`
- 네이비: `#1a2d4e`
- 블루 라이트 표면: `#e8f1fb`
- 소프트 서피스: `#f4f7fb`
- 기본 텍스트: `#111827`
- 보조 텍스트: `#6b7280`
- 테두리: `#e5e7eb`

### Example Component Prompts
- "가비아 스타일 히어로 섹션 — 흰 배경, 도메인 검색 바(#0067CC 테두리), 헤딩 52px Pretendard 700, 캡슐 CTA 2개."
- "서비스 카드 4열 그리드 — 48px 아이콘 (#e8f1fb 배경), 제목 22px/600, 설명 13px/muted, 블루 링크."
- "신뢰 지표 패널 — 수치 28px/700/#0067CC, 레이블 12px/muted, 흰 카드에 소프트 섀도."
- "고객 지원 패널 — #1a2d4e 배경, 흰 텍스트, 전화번호 22px/700, 2열 그리드 레이아웃."
- "가비아 GNB — 34px 네이비 유틸리티 바 + 60px 흰 메뉴 바, 블루 로고, 서비스 메뉴 5개."

### Iteration Guide
1. 가비아 블루(`#0067CC`)와 네이비(`#1a2d4e`)를 기반으로 팔레트를 구성.
2. 도메인 검색 바를 히어로의 핵심 인터랙션으로 고정.
3. 서비스 카드는 항상 아이콘 중심 + 명확한 서비스명 구조 유지.
4. 신뢰 지표 수치는 가능한 한 실제 데이터를 사용.
5. 한국어 최적화: `word-break: keep-all`, `Pretendard` 폰트 적용.
6. 정보 밀도 우선 — 불필요한 여백보다 명확한 서비스 구조가 중요.
