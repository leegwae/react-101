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

## 의존성 설명

### 런타임 의존성 (dependencies)
- **`react`** (^18.2.0): React 라이브러리 코어. 컴포넌트, 상태 관리, 가상 DOM 등 React의 핵심 기능을 제공
- **`react-dom`** (^18.2.0): React를 웹 브라우저의 DOM에 렌더링하기 위한 라이브러리. `createRoot` 등의 DOM 조작 API 제공

### 개발 의존성 (devDependencies)
- **`@babel/cli`** (^7.23.0): Babel 명령줄 도구. 터미널에서 `babel` 명령어를 사용할 수 있게 해줌
- **`@babel/core`** (^7.23.0): Babel의 핵심 엔진. 코드 변환(트랜스파일)의 실제 작업을 수행
- **`@babel/preset-react`** (^7.22.0): JSX 문법을 일반 JavaScript로 변환하는 Babel 프리셋. React 컴포넌트의 JSX를 `React.createElement()` 호출로 변환

## 특징

- 빌드 도구 없이 Babel만 사용
- minify, uglify, bundle 없음
- 트랜스파일만 수행
- 간단한 카운터 기능

## 작동 원리

1. `src/app.jsx`의 JSX 코드가 Babel에 의해 `dist/app.js`로 트랜스파일됨
2. `index.html`이 트랜스파일된 `dist/app.js`를 ES 모듈로 로드
3. React가 `#root` 엘리먼트에 카운터 컴포넌트를 렌더링