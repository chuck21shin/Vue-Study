# Vue Study

### 1일차 (2019년 10월 10일)

```
1. Vue에 대해 ( Pattern, 역사, 미래성 )
2. Vue 프로젝트 생성
3. Component 제작
4. SCSS/SASS 설명 & 이용법
5. Component 조합
6. 주의점 ( Arrow Function 사용 금지 등 )
7. javascript 배열 다루는 6가지 방법 & 자주 사용하는 ES6 표현
	1. Arrow Function
	2. Template Literals
	3. Object Destructuring
	4. Spread Operator
8. Component 데이터 활용
9. Component 부모 / 자식간의 데이터 주고 받기
10. Component 라이프 사이클을 이용한 프로젝트 고도화
11. Routing
12. ...
```

### 2019년 10월 10일

> 주요내용
>
> 1. SPA에 대한 설명과 SSR을 이용하지 않는 해결방법 설명
> 2. Vue 초기 설정
> 3. sass/scss 사용을 위한 dependencies 설치 ( sass-loader, node-sass )

2. Vue 초기 설정

```bash
# vue cli 설치
npm install -g @vue/cli

or

yarn add -g @vue/cli
```

다음과 같이 vue cli를 설치하면

```bash
vue --version

```

3. SASS/SCSS 이용하기

```bash
# loader 설치
npm install --save-dev sass-loader node-sass

or

yarn add -D sass-loader node-sass
```

@vue/cli를 이용한 초기설정을 하면 webpack에 sass-loader, node-sass에 대한 설정이 되어 있습니다. 하지만 기본 css를 이용하게 되어 있기 때문에 sass/scss를 사용하기 위해서는 다음 2개를 설치해주셔야 합니다.

```javascript
<style lang="scss" scoped>
header {
	backgournd-color: red;

	h1 {
		font-size: 20px;
	}
}
</style>
```

설치 하게 되면 다음과 같이 `lang="scss"`로 설정해도 오류가 발생하지 않고 `nesting`를 시작으로 sass/scss의 기능을 이용하여 스타일 할 수 있습니다.

### 2019년 10월 17일

> 주요내용
>
> 1. Vue파일을 이용한 Component 다루기

```bash
yarn add -D eslint-config-airbnb-base eslint-plugin-import eslint-plugin-vue
```