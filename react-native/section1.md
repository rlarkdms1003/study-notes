REACT NATIVE UI COMPONENT
![image](https://github.com/user-attachments/assets/2440bbeb-2525-49f7-b53c-36dd378024b8)

리액트 네이티브의 장점

1. WebView를 사용하는 다른 크로스 플랫폼과는 다르게 실제 호스트 플랫폼의 표준 렌더링 API를 사용해서 렌더링하게 된다.
=> WebView를 사용하면 성능상의 문제와 Native에서사용하는 기본 UI요소나 애니메이션을 Javascript, HTML 및 CSS 조합으로 모방하려고 하기에 한계가 있다.
=> React Natie는 마크업 요소를 실제 네이티브 요소로 변환해서 사용한다.

* WebView란? 웹 브라우저 컴포넌트로 앱에 임베딩하는 것. 즉, 앱에 넣는 것을 말한다.

2. 리액트 네이티브는 리액트와 마찬가지로 state와 props가 변경되면 React Native의 뷰를 다시 렌더링 하는 것과 같이 React 사용하느것과 대부분이 비슷하기에 React를 사용하는 웹 개발자라면 손쉽게 앱 개발을 할 수 있게 만든다.
React와의 주요 차이점은 HTML 및 CSS 마크업을 사용하는 대신 호스트 플랫폼의 UI 라이브러리를 활용하여 이를 수행한다.

리액트 네이티브 개봘 환경
리액트 네이티브를 이용할 때 환경을 세팅하는 방법은 대표적으로 두 가지가 있다.
![image](https://github.com/user-attachments/assets/f719e88f-15e7-4413-8ef2-42fddd31c28b)

먼저 Expo를 이용해서 개발한 이후에 프로젝트에서는 React Native CLI를 이용해서 개발할 예정

React 설치 시 Node.js가 필요한 이유
리액트 앱은 웹 브라우저에서 실행되는 코드여서 Node.js와 직접적인 연관은 없으나 프로젝트를 개발하는 데 주요 도구들이 Node.js를 사용하기 때문에 필요하다. 이 때 사용하는 개발 도구는 바벨, 모듈화된 코드를 한 파일로 합치고 코드를 수정할 때 마다 웁 브라우저를 리로딩하는 등 여러기능을 지니 웹팩등이 있다.

expo-cli 설치 과정
![image](https://github.com/user-attachments/assets/3eed54ae-5546-4f40-bf0f-b3317fe7bb2e)
![image](https://github.com/user-attachments/assets/e42dddd5-2572-42b4-8bd6-bbf6ce7418fa)
설치 완료 후 VS Code에서 프로젝트 파일을 실행하면 아래와 같이 폴더들이 생성된것을 확인할 수 있다.
![image](https://github.com/user-attachments/assets/4689849c-cc90-4a2b-8550-1c3909e14425)

Expo로 생성한 리액트 네이티브 앱 구조 살펴보기

![image](https://github.com/user-attachments/assets/8bb35121-79d6-4742-84fe-6684c7ed07b7)

* 바벨이란? 최신 자바스크립트 문법을 지원하지 않는 브라우저들을 위해서 최신 자바스크립트 문법을 구형 브라우저에서도 돌 수 있게 변환 시켜주는 라이브러리

Package.json 파일
해당 프로젝트에 대한 정보들이 들어있다. 프로젝트 이름, 버전, 필요한 라이브러리와 라이브러리의 버전들이 명시되어있다. 앱을 시작할 때 사용할 스크립트, 앱을 빌드할 때, 테스트할 때 사용할 스크립트등이 명시되어 있다.
![image](https://github.com/user-attachments/assets/11dcebef-800a-4013-879a-7ce4d4f0419c)
-> 앱 실행, 빌드, 테스트 등의 스크립트가 명시되어 있다. 프로젝트에서 자주 실행해야 하는 명령얼르 Scripts로 작성해두면 명령어로 실행이 가능한다.

![image](https://github.com/user-attachments/assets/7606d5af-c104-454e-b419-19f5e2a6a13d)
-> 필요한 라이브러리와 라이브러리의 버전들이 명시되어 있다.

