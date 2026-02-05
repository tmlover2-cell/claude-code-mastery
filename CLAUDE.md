# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 프로젝트 개요

개발자 웹 이력서 프로젝트 - HTML, CSS, JavaScript, TailwindCSS를 사용한 반응형 포트폴리오 웹사이트

## 언어 및 커뮤니케이션 규칙

- **기본 응답 언어**: 한국어
- **코드 주석**: 한국어로 작성
- **커밋 메시지**: 한국어로 작성
- **문서화**: 한국어로 작성
- **변수명/함수명**: 영어 (코드 표준 준수)

## 기술 스택

- HTML5 (시맨틱 마크업)
- CSS3 (스타일링 및 애니메이션)
- JavaScript (인터랙션 및 동적 기능)
- TailwindCSS (CDN 방식 사용)

## 프로젝트 구조

```
/
├── index.html          # 메인 페이지
├── css/
│   └── styles.css     # 커스텀 스타일
├── js/
│   └── main.js        # 메인 JavaScript
├── images/            # 이미지 파일
├── ROADMAP.md         # 개발 로드맵
└── README.md          # 프로젝트 문서
```

## 개발 환경

정적 웹사이트이므로 별도의 빌드 과정이 필요 없습니다.

### 로컬 개발 서버 실행

Python 3:
```bash
python3 -m http.server 8000
```

Python 2:
```bash
python -m SimpleHTTPServer 8000
```

Node.js (http-server):
```bash
npx http-server -p 8000
```

브라우저에서 `http://localhost:8000` 접속

## 주요 섹션 구조

index.html은 다음 섹션들로 구성됩니다:

1. **Navigation** - 고정 네비게이션 바 (다크모드 토글, 모바일 메뉴)
2. **Header** - 프로필 정보, 이름, 직책, 연락처
3. **About** - 자기소개
4. **Skills** - 기술 스택 (Frontend, Backend, Database, Tools)
5. **Experience** - 경력 타임라인
6. **Projects** - 프로젝트 포트폴리오 (카드 형식)
7. **Education** - 학력
8. **Contact** - 연락처 정보
9. **Footer** - 저작권 정보

## JavaScript 기능 (js/main.js)

구현해야 할 주요 기능:

1. **부드러운 스크롤**: 네비게이션 링크 클릭 시 해당 섹션으로 스무스 스크롤
2. **다크모드 토글**: localStorage를 사용한 테마 저장 및 복원
3. **모바일 메뉴**: 햄버거 메뉴 토글
4. **스크롤 애니메이션**: Intersection Observer를 사용한 fade-in/slide-in 효과
5. **프로젝트 필터링** (선택): 기술 스택별 프로젝트 필터링

## 스타일링 가이드

### TailwindCSS 사용

- CDN을 통해 TailwindCSS 로드
- 반응형 브레이크포인트: `sm:`, `md:`, `lg:`, `xl:`
- 다크모드: `dark:` 클래스 사용

### 색상 테마

- Primary: Blue (blue-500, blue-600)
- Secondary: Purple (purple-500, purple-600)
- 배경 (라이트): gray-50, white
- 배경 (다크): gray-800, gray-900
- 텍스트 (라이트): gray-700, gray-800
- 텍스트 (다크): gray-200, gray-300

### 반응형 디자인

- 모바일 퍼스트 접근
- 네비게이션: 모바일에서 햄버거 메뉴, 데스크톱에서 수평 메뉴
- 프로젝트 카드: 모바일 1열, 태블릿/데스크톱 2열
- 스킬 카드: 모바일 1열, 태블릿/데스크톱 2열

## 개발 우선순위 (ROADMAP.md 참조)

### Phase 1-2: 구조 및 레이아웃
- HTML 시맨틱 마크업
- 모든 섹션 레이아웃 구성

### Phase 3: 스타일링
- TailwindCSS를 활용한 반응형 디자인
- 다크/라이트 모드 스타일

### Phase 4: 인터랙션
- JavaScript 기능 구현
- 애니메이션 효과

### Phase 5-6: 콘텐츠 및 최적화
- 실제 콘텐츠 입력
- 성능 최적화 및 배포

## 배포

정적 사이트 호스팅 서비스 사용:

- **GitHub Pages**:
  ```bash
  # Settings → Pages → Source를 main 브랜치로 설정
  ```

- **Vercel**:
  ```bash
  npx vercel
  ```

- **Netlify**:
  ```bash
  npx netlify deploy
  ```

## 성능 최적화 체크리스트

- 이미지 최적화 (WebP, 압축)
- CSS/JS 최소화 (배포 시)
- SEO 메타 태그 설정
- Open Graph 태그 추가
- 접근성 (a11y) 검사

## 코드 작성 시 주의사항

1. **시맨틱 HTML 사용**: `<header>`, `<nav>`, `<section>`, `<footer>` 등
2. **접근성 고려**: ARIA 레이블, alt 텍스트, 키보드 네비게이션
3. **성능**: 불필요한 라이브러리 사용 지양, CDN 사용
4. **크로스 브라우저**: 주요 브라우저(Chrome, Firefox, Safari, Edge)에서 테스트
5. **모바일 최적화**: 터치 이벤트, 뷰포트 설정, 반응형 이미지
