# React Counter App

빌드 도구 없이 Babel만 사용한 간단한 React 카운터 애플리케이션입니다. (bun 사용)

## 설치 및 실행

1. 의존성 설치:

```bash
bun install
```

2. JSX 파일을 JavaScript로 트랜스파일:

```bash
bun run build
```

3. 브라우저에서 `index.html` 파일을 열어서 확인:

```bash
bun start
```

또는 직접 `index.html` 파일을 브라우저에서 열어도 됩니다.

## 파일 구조

- `src/app.jsx` - React 컴포넌트 소스 파일
- `dist/app.js` - 트랜스파일된 JavaScript 파일
- `index.html` - 메인 HTML 파일
- `.babelrc` - Babel 설정 파일
- `package.json` - 프로젝트 설정 및 의존성

## 특징

- 빌드 도구 없이 Babel만 사용
- minify, uglify, bundle 없음
- 트랜스파일만 수행
- 간단한 카운터 기능