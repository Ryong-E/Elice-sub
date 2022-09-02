<img src="http://kdt-ai5-team08.elicecoding.com/assets/image/Logo.svg"/>

#  사용 기술
<div>
  <img src="https://img.shields.io/badge/Typescript-3178C6?style=flat-square&logo=Typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=white"/>
  <img src="https://img.shields.io/badge/Recoil-black?style=flat-square&logo=Recoil&logoColor=white"/>
  <img src="https://img.shields.io/badge/ReactQuery-FF4154?style=flat-square&logo=ReactQuery&logoColor=white"/>
  <img src="https://img.shields.io/badge/ReactHookForm-EC5990?style=flat-square&logo=ReactHookForm&logoColor=white"/>
  <img src="https://img.shields.io/badge/Axios-5A29E4?style=flat-square&logo=Axios&logoColor=white"/>
  <img src="https://img.shields.io/badge/styledcomponents-DB7093?style=flat-square&logo=styled-components&logoColor=white"/>
  <img src="https://img.shields.io/badge/HTML-E34F26?style=flat-square&logo=HTML5&logoColor=white"/>
  <img src="https://img.shields.io/badge/CSS-1572B6?style=flat-square&logo=CSS3&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=Git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitLab-FC6D26?style=flat-square&logo=GitLab&logoColor=white"/>
</div>

# 기술 사용 이유
## TypeScript
타입을 직접 지정해주고 컴파일 시점에 에러를 잡아 낼 수 있습니다.<br>
자바스크립트는 타입을 런타임 이전이 아닌, 런타임에 동적으로 검사합니다.
그래서 프로그램을 실행해보지 않는 이상 어떤 타입 에러도 잡아낼 수 없습니다.
이런 이유들로 런타임 이전에 정적 타입을 검사할 수 있게 만들고자 사용하게 되었습니다.
## Recoil
`context`를 사용하게 되면 단일 값만 저장할 수 있고 여러 값들의 집합을 담을 수가 없습니다.
그래서 부분적인 상태 변경이 어려워집니다. 별도의 `Provider`를 이용해 랜더링을 제어하려고 해도 자식 요소들 전체를 재랜더링 해야 하고 의도치 않은 문제가 생깁니다.

반면 `Redux`와 `Mobx`의 기능적인 문제는 없습니다. 
하지만 이 상태 관리 라이브러리들은 리액트의 내부 라이브러리가 아니기 때문에
리액트의 가상돔의 내부 로직과는 별개로 동작합니다.
그러니까 `Redux`의 `store`은 리액트의 상태와는 별개의 것이기 때문에
사용할 시 수많은 코드를 통해서 리액트의 상태와 리덕스의 상태를 일치 시키는 작업을 해야 합니다. 
하지만 `recoil`은 `hook`처럼 리액트의 상태를 간단하게 변경하고 이용 가능하다는 이유로 선택하게 되었습니다.
## React-Hook-Form
기존의 폼에서 입력해야 하는 여러가지 번거로운 작업을 줄여줍니다
( value 설정, 데이터 전송 관리 등등 )
입력값에 조건을 달아서 에러를 띄울 수 있습니다.
타입스크립트로 작성된 라이브러리이므로, 타입스크립트와 아주 잘 맞습니다.
불필요한 렌더링을 최소화 합니다.
## React-Query
서버에서 데이터를 받아올때 로딩 중을 없애기 위해서 데이터를 가져올 떄 캐시 값으로 저장해두어서 로딩을 최소화하였습니다.
서버의 값을 클라이언트에 가져오거나, 캐싱, 값 업데이트, 에러핸들링 등
비동기 과정을 더욱 편하게 하는데 사용됩니다

# 폴더구조

```bash
📦 front
├─ node_modules
docs
├─ public
└─ src
   ├─ api
   ├─ components
   │  ├─ category
   │  │  ├─ award
   │  │  ├─ certificate
   │  │  ├─ education
   │  │  └─ project
   │  ├─ Modal
   │  ├─ styledComponents
   │  └─ user
   ├─ font
   └─ theme
```

# 실행방법
```bash
npm i -g yarn
yarn
yarn start
```
