# 모던 자바스크립트 라이브러리/프레임워크

1. DAY 01

+ [ECMAScript 6 슬라이드](http://slides.com/yamoo9/es6/)
+ [Babel 키노트](http://slides.com/yamoo9/babel#/)

2. DAY 02

+ [Rollup 키노트](http://slides.com/yamoo9/rollup#/)
+ [ESLint키노트](http://slides.com/yamoo9/eslint#/)

## Node Version Manager 

[NVM for windows](https://github.com/coreybutler/nvm-windows)

```sh
nvm version

# 설치된 버전들을 보여줌
nvm list

# 설치 가능한 버전 찾기
nvm list available

# 버전 선택적으로 설치 시 
nvm install 8.1.2

# nvm 옵션 목록보기
nvm ls -remote
```
## Yarn

> FAST, RELIABLE, AND SECURE DEPENDENCY MANAGEMENT.

패키지 버전관리를 잘해주고 엄청 빠르다.  
[Yarn](https://yarnpkg.com/lang/en/)
```sh
echo {} > package.json

npm i -g yarn

# yarn이 설치되었는지 확인
npm ll -g yarn

yarn -v

# yarn으로 제이쿼리 로컬 설치
yarn add jquery

yarn add bulma
yarn add --dev babel-cli babel-preset-env
```
※ yarn 사용시 생성되는 `yarn.lock`은 설치한 패키지를 관리하기 위한 파일로 지우면 안된다.

[BULMA](https://bulma.io/) : CSS 프레임워크

## jQuery

### constructor vs prototype

```javascript
var jQuery = function( selector, context ) {
  return new jQuery.fn.init( selector, context );
}

jQuery.fn = jQuery.prototype = {
  constructor: jQuery,
  /* ... */
}
```

## 모듈

[키노트](http://slides.com/yamoo9/es6/#/10)