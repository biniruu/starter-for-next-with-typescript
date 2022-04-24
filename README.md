# Next.js with Typescript boilerplate

넥스트 + 타입스크립트 프로젝트를 바로 시작할 수 있는 보일러플레이트예요.  
create next app으로 next.js 설치 후 next 프로젝트에 필요한 기본적인 패키지를 추가했어요.

개인 프로젝트용으로 만들었기 때문에 각 설정 파일은 개인 취향에 맞췄어요.  
저와 취향이 다른 사람에게는 맞지 않을 수도 있어요😇

패키지는 필요한 것만 골라서 설치하세요.

> 제가 패키지를 다 알지 못해요🥺 불필요한 것이 섞였거나 더 좋은 패키지가 있을 수도 있어요.

> 오랫동안 업데이트가 되지 않았으면 여기 있는 대로 설정했을 때 문제가 발생할 수 있어요.  
> 물론 최근 업데이트 일자와 상관없이 문제가 발생할 수도 있어요🫠

<br>

## Next.js 설치 👨🏻‍💻

```bash
## Create next app

$ yarn create next-app --typescript
```

<br>

## 패키지 설치 📦

```bash
## Eslint & Perttier

$ yarn add -D eslint-config-prettier eslint-plugin-prettier eslint-webpack-plugin prettier

## Jest

$ yarn add -D eslint-plugin-jest ts-jest

## Sass loader

$ yarn add -D sass sass-loader

## Stylelint

$ yarn add -D @stylelint/postcss-css-in-js postcss-syntax stylelint stylelint-config-prettier stylelint-config-standard stylelint-order stylelint-scss

## Typescript

$ yarn add -D @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-import-resolver-typescript
```

<br>

## 패키지 설명 📄

위에서 설치한 패키지가 무엇인지 알아보세요.

- `@stylelint/postcss-css-in-js` : _CssSyntaxError_ 해결을 위해 필요
- `@typescript-eslint/eslint-plugin` : typescript 관련 린팅 규칙 제공
- `@typescript-eslint/parser` : typescript를 위한 eslint 파서
- `eslint-config-prettier` : prettier와 충돌을 일으키는 eslint 규칙 비활성화
- `eslint-import-resolver-typescript` : tsconfig에서 path alias 사용을 위해 필요
- `eslint-plugin-jest` : jest 관련 린팅 규칙 제공
- `eslint-plugin-prettier` : prettier에서 인식하는 코드상의 포맷 오류를 eslint 오류로 출력
- `eslint-webpack-plugin`
- `postcss-syntax` : _CssSyntaxError_ 해결을 위해 필요
- `prettier` : 코드의 스타일을 잡아주는 포맷팅 기능
- `sass`
- `sass-loader`
- `stylelint`
- `stylelint-config-prettier`
- `stylelint-config-standard`
- `stylelint-order`
- `stylelint-scss`
- `ts-jest` : typescript 환경에서 jest를 사용할 때 필요

```
💁🏻‍♀️ CRA로 리액트를 설치했다면 아래 패키지는 필요하지 않아요.

- eslint : 코드의 문법을 검사하는 린팅과 코드의 스타일을 잡아주는 포맷팅 기능
- eslint-plugin-react : react 관련 린팅 규칙 제공
- eslint-plugin-react-hooks : react hooks 규칙 관련 피드백 제공
- eslint-plugin-import : es2015+ import/export 구문 지원
- eslint-plugin-jsx-a11y : jsx 내에서 웹 접근성 규칙 관련 피드백 제공
- eslint-webpack-plugin
- jest
- typescript
```

```
💁🏻 typescript를 사용한다면 아래 패키지는 필요하지 않아요.

- @babel/core : @babel/eslint-parser 설치를 위해 필요
- @babel/eslint-parser : babel-eslint
- @babel/preset-react : "This experimental syntax requires enabling one of the following parser plugin(s): 'jsx, flow, typescript'" 에러 해결을 위해 필요[관련 글](https://ffan0811.medium.com/error-debugging-this-experimental-syntax-requires-enabling-one-of-the-following-parser-plugin-s-22946599a0a4)
```

```
❌ deprecate 되었어요.

- babel-eslint : @babel/eslint-parser를 사용할 것
- eslint-loader : eslint-webpack-plugin으로 대체
```

```
🙌 여기서는 사용하지 않지만, 유용한 패키지예요.

- @craco/craco : CRA로 리액트를 설치했을 때 webpack 설정 지원
```

<br>

## 설정 파일 💾

제 취향이 듬뿍 담긴 파일이니 각자 취향에 맞춰 수정 후 사용하세요👻

### Eslint & Perttier

- `.eslintignore`
- `.eslintrc.js`
- `.prettierignore`
- `.prettierrc`

### Git

- `.gitignore`

### Jest

- `jest.config.ts`

### Stylelint

- `.stylelintignore`
- `.stylelintrc.js`

### Typescript

- `tsconfig.json`

<br>

## 필수 vs code 설정 🔧

settings에서 아래 설정을 변경해주세요.

- Editor: Default Formatter => `esbenp.prettier-vscode`
- Eslint > Format: Enable => `true`

<br>

## 필수 vs code 익스텐션 🧩

위 패키지를 제대로 사용하기 위해 꼭 필요한 익스텐션이에요.  
_괄호 안에 있는 익스텐션 ID로 검색하면 편리하게 찾을 수 있어요._

- `ESLint` (dbaeumer.vscode-eslint)
- `Prettier - Code formatter` (esbenp.prettier-vscode)
- `Stylelint` (stylelint.vscode-stylelint)

<br>

## 추천 vs code 익스텐션 🚀

필수는 아니지만, 편의성을 높여주는 익스텐션이에요.

- `JavaScript and TypeScript Nightly` (ms-vscode.vscode-typescript-next)
- `Jest` (Orta.vscode-jest)
- `Stylelint Disable Snippets` (hedinne.stylelint-disable-snippets)
