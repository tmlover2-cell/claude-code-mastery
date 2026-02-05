# 개발자 웹 이력서 프로젝트 로드맵

## 프로젝트 개요
개인 개발자 포트폴리오 및 이력서를 소개하는 반응형 웹사이트

## 기술 스택
- **HTML5**: 시맨틱 마크업
- **CSS3**: 스타일링 및 애니메이션
- **JavaScript**: 인터랙션 및 동적 기능
- **TailwindCSS**: 유틸리티 기반 CSS 프레임워크

## 프로젝트 구조
```
/
├── index.html          # 메인 페이지
├── css/
│   └── styles.css     # 커스텀 스타일
├── js/
│   └── main.js        # 메인 JavaScript
├── images/            # 이미지 파일
└── README.md          # 프로젝트 문서
```

## 개발 단계

### Phase 1: 프로젝트 설정 (1단계)
- [x] 프로젝트 폴더 구조 생성
- [ ] index.html 기본 구조 작성
- [ ] TailwindCSS CDN 설정
- [ ] 기본 CSS 파일 생성
- [ ] JavaScript 파일 생성

### Phase 2: 레이아웃 구성 (2단계)
- [ ] 헤더 섹션 (이름, 직책, 연락처)
- [ ] 네비게이션 메뉴
- [ ] 소개(About) 섹션
- [ ] 기술 스택(Skills) 섹션
- [ ] 경력(Experience) 섹션
- [ ] 프로젝트(Projects) 섹션
- [ ] 학력(Education) 섹션
- [ ] 연락처(Contact) 섹션
- [ ] 푸터

### Phase 3: 스타일링 (3단계)
- [ ] TailwindCSS를 활용한 반응형 디자인
- [ ] 색상 테마 설정 (라이트/다크 모드)
- [ ] 타이포그래피 스타일링
- [ ] 카드 컴포넌트 디자인
- [ ] 버튼 및 링크 스타일
- [ ] 모바일 반응형 최적화

### Phase 4: 인터랙션 기능 (4단계)
- [ ] 부드러운 스크롤 네비게이션
- [ ] 다크모드 토글 기능
- [ ] 스크롤 애니메이션 (Fade-in, Slide-in)
- [ ] 프로젝트 필터링 기능
- [ ] 햄버거 메뉴 (모바일)
- [ ] 연락처 폼 유효성 검사

### Phase 5: 콘텐츠 작성 (5단계)
- [ ] 개인 정보 및 소개 작성
- [ ] 기술 스택 목록 정리
- [ ] 경력 사항 작성
- [ ] 프로젝트 포트폴리오 작성
- [ ] 학력 정보 입력
- [ ] 프로필 이미지 및 프로젝트 스크린샷 추가

### Phase 6: 최적화 및 배포 (6단계)
- [ ] 크로스 브라우저 테스트
- [ ] 성능 최적화 (이미지 압축, 코드 최소화)
- [ ] SEO 메타 태그 설정
- [ ] Open Graph 태그 추가
- [ ] GitHub Pages / Vercel / Netlify 배포
- [ ] 도메인 연결 (선택사항)

## 주요 기능

### 필수 기능
1. **반응형 디자인**: 모바일, 태블릿, 데스크톱 대응
2. **부드러운 네비게이션**: 각 섹션으로 스크롤 이동
3. **다크/라이트 모드**: 테마 전환 기능
4. **프로필 섹션**: 이름, 사진, 직책, 간단한 소개
5. **기술 스택**: 아이콘과 함께 기술 목록 표시
6. **경력 타임라인**: 시간순으로 경력 표시
7. **프로젝트 포트폴리오**: 주요 프로젝트 카드 형식
8. **연락처 정보**: 이메일, GitHub, LinkedIn 등

### 선택 기능
1. **애니메이션**: 스크롤 기반 fade-in/slide-in 효과
2. **필터링**: 프로젝트를 기술별로 필터링
3. **다운로드 버튼**: PDF 이력서 다운로드
4. **방문자 통계**: 간단한 조회수 카운터
5. **블로그 링크**: 기술 블로그 연동

## 이력서 기본 구성 내용

### 1. Header (헤더)
- 이름: 홍길동
- 직책: 풀스택 개발자
- 연락처: email@example.com | GitHub | LinkedIn

### 2. About (소개)
- 3년차 웹 개발자
- 주요 관심사: 프론트엔드 개발, UI/UX
- 간단한 자기소개 (2-3문장)

### 3. Skills (기술 스택)
- **Frontend**: HTML, CSS, JavaScript, React, TailwindCSS
- **Backend**: Node.js, Express
- **Database**: MongoDB, MySQL
- **Tools**: Git, VS Code, Figma

### 4. Experience (경력)
- **회사명** (2022.01 - 현재)
  - 프론트엔드 개발자
  - 주요 업무: 웹 애플리케이션 개발, UI 컴포넌트 구현

- **회사명** (2021.01 - 2021.12)
  - 주니어 개발자
  - 주요 업무: 웹사이트 유지보수, 기능 개선

### 5. Projects (프로젝트)
- **프로젝트 1**: 쇼핑몰 웹사이트
  - 기술: React, TailwindCSS, Node.js
  - 설명: 반응형 이커머스 플랫폼

- **프로젝트 2**: 할일 관리 앱
  - 기술: HTML, CSS, JavaScript
  - 설명: 심플한 Todo 애플리케이션

### 6. Education (학력)
- **대학교명** (2017 - 2021)
  - 컴퓨터공학과 학사

### 7. Contact (연락처)
- Email: example@email.com
- GitHub: github.com/username
- LinkedIn: linkedin.com/in/username

## 개발 순서 (권장)

1. **기본 HTML 구조 작성** (index.html)
2. **TailwindCSS 설정 및 기본 스타일 적용**
3. **각 섹션별 마크업 완성**
4. **반응형 레이아웃 구현**
5. **JavaScript 인터랙션 추가**
6. **콘텐츠 입력 및 이미지 추가**
7. **다크모드 구현**
8. **애니메이션 효과 추가**
9. **테스트 및 디버깅**
10. **배포**

## 참고 자료
- TailwindCSS 문서: https://tailwindcss.com/docs
- MDN Web Docs: https://developer.mozilla.org
- CSS 애니메이션: https://animate.style
- 무료 아이콘: https://heroicons.com

## 다음 단계
1. `index.html` 파일 생성 및 기본 구조 작성
2. TailwindCSS CDN 링크 추가
3. 각 섹션별 HTML 마크업 작성
4. 스타일링 및 반응형 디자인 적용
