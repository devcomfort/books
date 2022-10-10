<h1>Yarn Berry Workspaces 정리</h1>

> 이 문서는 [yarn workspace 모노레포 설정하기 - designdevelop@medium](https://medium.com/@designdevelop/yarn-workspaces-%EB%AA%A8%EB%85%B8%EB%A0%88%ED%8F%AC-%EB%8F%84%EC%9E%85%EA%B8%B0-c0310ca41c0e)을 참조하여 작성하였습니다.

<h1>목차</h1>

- [명령어 정리](#명령어-정리)
  - [패키지 관리](#패키지-관리)
- [참조 문서](#참조-문서)

# 명령어 정리

## 패키지 관리

- `yarn init -y`: 프로젝트 초기 설정
- `yarn workspace <프로젝트명> add <패키지 이름>`: 해당 프로젝트에 원하는 패키지를 설치
- `yarn workspace <프로젝트명> remove <패키지 이름>`: 해당 프로젝트에 원하는 패키지를 설치
- `yarn add <패키지 이름> -w`: 루트 디렉토리에 패키지 추가

# 참조 문서

- [Yarn berry workspace를 활용한 프론트엔드 모노레포 구축기 - 우아한형제들 기술블로그](https://techblog.woowahan.com/7976/)
  `Yarn berry workspace`를 통해 우아한 형제들 개발팀이 프로젝트 관리 방식을 어떻게 바꾸었는지에 대한 글입니다. <br>
  모노레포를 소개하는 것에 의미가 큰 글입니다.
- [yarn workspace 모노레포 설정하기 - designdevelop@Medium](https://medium.com/@designdevelop/yarn-workspaces-%EB%AA%A8%EB%85%B8%EB%A0%88%ED%8F%AC-%EB%8F%84%EC%9E%85%EA%B8%B0-c0310ca41c0e)
  개인이 작성한 `yarn berry workspace`를 다루는 법에 대한 글입니다. <br>
  `yarn berry workspace`에서 사용할 수 있는 명령어 양식과 `yarn berry workspace`를 통해 `모노레포`를 구축하기 위해 필요한 몇몇의 개념이 포함되어 있습니다. <br>
  모노레포를 실제로 다루기 위한 실용적인 정보를 담고 있다는데 의미가 큰 글입니다. <br><br>
  아래의 4가지 모노레포 툴에 대해서도 간단하게 이야기하고 있습니다.
  - [Yarn](https://d2.naver.com/helloworld/7553804#ch1)
  - [Lerna](https://d2.naver.com/helloworld/7553804#ch2)
  - [Nx](https://d2.naver.com/helloworld/7553804#ch3)
  - [Turborepo](https://d2.naver.com/helloworld/7553804#ch4)
- [node_modules로부터 우리를 구원해 줄 Yarn Berry - Toss Tech](https://toss.tech/article/node-modules-and-yarn-berry)
  *hoisting*을 이해하기 위해 찾던 문서 중 하나입니다. <br>
  *유령 의존성*을 이해함으로써 *hoisting*의 개념을 이해할 수 있도록 돕습니다. <br>
  `yarn berry`에 대해 깊게 파보고 싶다면, 이 문서가 여러 명령셋을 포함하고 있으니, 확인하기 바랍니다.
