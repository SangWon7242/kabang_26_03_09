# 카카오뱅크 (KakaoBank) - 퍼블리싱 클론 프로젝트

> 카카오뱅크 공식 홈페이지를 참고하여 제작한 퍼블리싱 클론 프로젝트입니다.

## 📋 프로젝트 소개

카카오뱅크 공식 웹사이트의 메인 페이지를 HTML, SCSS, JavaScript로 퍼블리싱한 프로젝트입니다.  
다양한 인터랙션과 애니메이션을 구현하여 실제 사이트와 유사한 사용자 경험을 제공합니다.

## 🛠️ 기술 스택

| 분류           | 기술                      |
| -------------- | ------------------------- |
| **마크업**     | HTML5, 시맨틱 태그        |
| **스타일**     | SCSS, Tailwind CSS (CDN)  |
| **스크립트**   | Vanilla JavaScript (ES6+) |
| **라이브러리** | Swiper.js, Font Awesome   |
| **폰트**       | Pretendard (@font-face)   |

## 📁 프로젝트 구조

```
kabang_26_03_09/
├── index.html           # 메인 HTML 파일
├── README.md
├── assets/
│   ├── images/          # 이미지 리소스 (SVG, PNG)
│   └── videos/          # 비디오 리소스 (MP4)
├── css/
│   ├── style.css        # 컴파일된 CSS
│   └── style.css.map    # 소스맵
├── js/
│   ├── script.js        # 메인 스크립트 (인터랙션, 애니메이션)
│   └── data.js          # 데이터 관리 (스토리 콘텐츠 등)
└── scss/
    ├── style.scss       # SCSS 엔트리 포인트
    ├── _base.scss       # 기본 스타일
    ├── _reset.scss      # 리셋 스타일
    ├── _fonts.scss      # 폰트 설정 (Pretendard)
    ├── _variables.scss  # SCSS 변수
    ├── _mixins.scss     # SCSS 믹스인
    └── _layout.scss     # 레이아웃 & 컴포넌트 스타일
```

## ✨ 주요 기능

### 🔹 헤더 (Header)

- **고정 헤더** : 스크롤 시 상단 고정
- **스크롤 방향 감지** : 스크롤 다운 시 헤더 숨김, 스크롤 업 시 헤더 표시
- **다단계 메뉴 (Depth2)** : 소개, 투자정보 hover 시 하위 메뉴 Fade-In 효과
- **언어 선택** : 한국어 / English 전환 메뉴

### 🔹 섹션 1 - 메인 비주얼

- 배경 **비디오 자동 재생** (muted, loop, autoplay)
- 타이틀 텍스트 애니메이션
- 스크롤 다운 안내 버튼

### 🔹 섹션 2 - 금융 서비스 소개

- **Swiper 슬라이더**로 서비스 카드 구성
- 스크롤 **15% 도달 시 슬라이드 펼침** 애니메이션

### 🔹 섹션 3 - 오늘의 뉴스

- 뉴스 카드 레이아웃 (좌측 대표 뉴스 + 우측 리스트)
- **오늘 날짜 자동 표시** (자정 시 자동 업데이트)

### 🔹 섹션 4 - 주요 경영 정보

- **CSS Grid** 기반 카드 레이아웃
- Hover 시 화살표 아이콘 인터랙션

### 🔹 섹션 5 - 금융 이야기

- **Swiper 슬라이더** (프로그레스 바 + 이전/다음 버튼)
- 슬라이드 변경 시 **좌측 콘텐츠 동적 업데이트** (YouTube, Blog, Instagram 등)

### 🔹 섹션 6 - 바로가기 링크

- **Flexbox** 기반 바로가기 버튼 그리드

### 🔹 푸터 (Footer)

- 사이트맵 네비게이션
- 인증 배지 (웹 접근성, 개인정보 보호)
- 이용약관 링크
- **Top 버튼** (페이지 상단으로 스무스 스크롤)

## 🚀 실행 방법

### 1. 프로젝트 클론

```bash
git clone https://github.com/SangWon7242/kabang_26_03_09.git
cd kabang_26_03_09
```

### 2. 로컬 서버 실행

별도의 패키지 설치 없이, **Live Server** 등을 사용하여 `index.html`을 열어 확인할 수 있습니다.

- **VS Code** : Live Server 확장 프로그램 사용
- **직접 실행** : `index.html` 파일을 브라우저에서 직접 열기

### 3. SCSS 컴파일 (수정 시)

SCSS 파일 수정 시, SCSS 컴파일러를 사용하여 CSS로 변환합니다.

```bash
# Sass 설치 (글로벌)
npm install -g sass

# SCSS → CSS 컴파일 (watch 모드)
sass --watch scss/style.scss:css/style.css
```

## 📱 지원 환경

- **데스크탑** : Chrome, Firefox, Safari, Edge (최신 버전)
- 모바일 대응은 포함되어 있지 않습니다 (데스크탑 퍼블리싱 중심)

## 📌 참고 사이트

- [카카오뱅크 공식 홈페이지](https://www.kakaobank.com)

---

© 2026 KakaoBank Clone Project. 본 프로젝트는 학습 목적으로 제작되었습니다.
