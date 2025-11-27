# Data Scientist Portfolio Website

데이터 사이언티스트를 위한 전문 포트폴리오 웹사이트입니다. 현대적이고 반응형 디자인으로 당신의 프로젝트와 기술을 효과적으로 전시할 수 있습니다.

## 🎯 특징

- **반응형 디자인**: 모든 기기(데스크톱, 태블릿, 모바일)에 최적화
- **모던 UI/UX**: 그래디언트, 애니메이션, 부드러운 전환 효과
- **완전 커스터마이징 가능**: 색상, 내용, 레이아웃을 쉽게 수정 가능
- **SEO 최적화**: 검색 엔진에 친화적인 구조
- **성능 최적화**: 빠른 로딩 속도와 부드러운 인터랙션
- **구간별 섹션**: 소개, 기술, 프로젝트, 연락처

## 📂 프로젝트 구조

```
homepage/
├── index.html                 # 메인 HTML 파일
├── assets/
│   ├── css/
│   │   └── styles.css         # 스타일시트
│   ├── js/
│   │   └── script.js          # 자바스크립트
│   └── images/                # 이미지 폴더 (나중에 추가)
├── README.md                  # 프로젝트 문서
└── .gitignore                # Git 무시 파일

```

## 🚀 시작하기

### 빠른 시작

1. **파일 다운로드 또는 클론**
```bash
git clone https://github.com/castleless0104-spec/homepage.git
cd homepage
```

2. **로컬 서버 실행**

Python이 설치되어 있다면:
```bash
# Python 3
python -m http.server 8000

# 또는 Python 2
python -m SimpleHTTPServer 8000
```

Node.js가 설치되어 있다면:
```bash
npx http-server -p 8000
```

3. **브라우저에서 열기**
```
http://localhost:8000
```

## ✏️ 커스터마이징 가이드

### 1. 개인 정보 수정 (index.html)

`index.html` 파일을 텍스트 에디터로 열고 다음 항목들을 수정하세요:

#### 로고 및 네비게이션
```html
<div class="logo">DS Portfolio</div>  <!-- 로고 텍스트 변경 -->
```

#### 영웅 섹션 (Hero Section)
```html
<h1 class="hero-title">데이터로 인사이트를 찾다</h1>
<p class="hero-subtitle">데이터 분석과 머신러닝으로 비즈니스 가치를 창출합니다</p>
```

#### 소개 섹션
```html
<h3>안녕하세요!</h3>
<p>저는 데이터 사이언티스트로서...</p>
```

#### 통계 정보
```html
<div class="stat-item">
    <h4>15+</h4>
    <p>프로젝트 완료</p>
</div>
```

#### 기술 카드
```html
<div class="skill-card">
    <h4>데이터 분석</h4>
    <ul>
        <li>Python (Pandas, NumPy)</li>
        <!-- 기술 추가/수정 -->
    </ul>
</div>
```

#### 프로젝트 추가/수정
```html
<div class="project-card">
    <div class="project-image" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);"></div>
    <div class="project-content">
        <h3>프로젝트 제목</h3>
        <p>프로젝트 설명</p>
        <div class="project-tags">
            <span class="tag">기술1</span>
            <span class="tag">기술2</span>
        </div>
        <a href="#" class="project-link">프로젝트 보기 →</a>
    </div>
</div>
```

#### 연락처 정보
```html
<div class="info-item">
    <h4>Email</h4>
    <p><a href="mailto:your.email@example.com">your.email@example.com</a></p>
</div>
```

### 2. 색상 테마 변경 (assets/css/styles.css)

`styles.css` 파일의 CSS 변수를 수정하여 색상 테마를 변경할 수 있습니다:

```css
:root {
    --primary-color: #667eea;      /* 주요 색상 */
    --secondary-color: #764ba2;    /* 보조 색상 */
    --accent-color: #f5576c;       /* 강조 색상 */
    --text-color: #333;            /* 텍스트 색상 */
    --bg-color: #f8f9fa;           /* 배경 색상 */
}
```

### 3. 프로젝트 이미지 추가

1. `assets/images/` 폴더에 이미지 파일을 추가하세요
2. `index.html`에서 프로젝트 카드의 `project-image` div 스타일을 수정:

```html
<!-- 그래디언트 대신 이미지 사용 -->
<div class="project-image" style="background-image: url('assets/images/project1.jpg');"></div>
```

### 4. 글꼴 변경

`styles.css`의 font-family 설정을 수정하세요:

```css
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    /* 다른 글꼴로 변경 가능 */
}
```

## 🎨 색상 팔레트 샘플

제안하는 색상 조합들:

### 파란색/보라색 (기본)
- Primary: `#667eea`
- Secondary: `#764ba2`
- Accent: `#f5576c`

### 그린/터쿼이즈
- Primary: `#00d4ff`
- Secondary: `#0099ff`
- Accent: `#39ff14`

### 주황색/분홍색
- Primary: `#ff6b6b`
- Secondary: `#ee5a6f`
- Accent: `#feca57`

## 📱 반응형 디자인

웹사이트는 다음 기기에 최적화되어 있습니다:

- **데스크톱**: 1200px 이상
- **태블릿**: 768px - 1199px
- **모바일**: 480px - 767px
- **소형 모바일**: 480px 이하

## 🔧 배포 방법

### GitHub Pages 배포

1. GitHub에 리포지토리 푸시
2. 리포지토리 Settings → Pages
3. Source를 "main branch"로 선택
4. 저장 후 배포 링크 확인

### Netlify 배포

1. [Netlify](https://www.netlify.com)에서 회원가입
2. "New site from Git" 클릭
3. GitHub 리포지토리 연결
4. 배포 설정 후 자동 배포

### Vercel 배포

1. [Vercel](https://vercel.com)에서 회원가입
2. "New Project" 클릭
3. GitHub 리포지토리 임포트
4. 자동 배포 시작

### 커스텀 서버 배포

```bash
# 파일 업로드 (FTP/SFTP)
sftp user@your-server.com
put -r /path/to/homepage/* /var/www/html/

# 또는 직접 배포
scp -r /path/to/homepage/* user@your-server.com:/var/www/html/
```

## 💡 팁과 트릭

### SEO 최적화
- `<title>` 태그를 설명적으로 작성
- `<meta name="description">` 업데이트
- Open Graph 메타 태그 추가

```html
<meta property="og:title" content="Your Portfolio Title">
<meta property="og:description" content="Your portfolio description">
<meta property="og:image" content="url-to-image">
```

### 구글 애널리틱스 추가

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_ID');
</script>
```

### 이메일 폼 기능 추가

[Formspree](https://formspree.io) 또는 [Netlify Forms](https://www.netlify.com/products/forms/)를 사용하여 이메일 기능 추가:

```html
<form action="https://formspree.io/f/YOUR_ID" method="POST">
    <!-- 폼 필드 -->
</form>
```

## 🐛 문제 해결

### 페이지가 로드되지 않음
- 파일 경로가 올바른지 확인
- 브라우저 콘솔에서 오류 메시지 확인 (F12)

### 스타일이 적용되지 않음
- CSS 파일 경로 확인: `assets/css/styles.css`
- 브라우저 캐시 삭제 (Ctrl+Shift+Delete)
- 파일이 저장되었는지 확인

### 자바스크립트가 작동하지 않음
- 자바스크립트 파일 경로 확인: `assets/js/script.js`
- 브라우저 콘솔에서 에러 확인
- 광고 차단 확장 프로그램 비활성화 시도

## 📚 추가 리소스

- [MDN Web Docs](https://developer.mozilla.org/)
- [CSS-Tricks](https://css-tricks.com/)
- [W3Schools](https://www.w3schools.com/)
- [Can I Use](https://caniuse.com/)

## 📝 라이센스

이 프로젝트는 MIT 라이센스 하에 배포됩니다.

## 🤝 기여

개선 사항이나 버그 리포트는 [Issues](https://github.com/castleless0104-spec/homepage/issues)에서 제출해주세요.

## 👨‍💻 작가

Data Scientist Portfolio Template - Created by castleless0104-spec

---

**마지막 업데이트**: 2025년 11월 27일

행운을 빕니다! 🚀
