- [1. TL;DR](#1-tldr)
- [2. 모노레포](#2-모노레포)
  - [2.1. 호이스팅](#21-호이스팅)

# 1. TL;DR

이 문서는 개발 과정에서 참조된/참조할 문서를 기재한 문서입니다.

# 2. 모노레포

- [Yarn berry workspace를 활용한 프론트엔드 모노레포 구축기 - 우아한형제들 기술블로그](https://techblog.woowahan.com/7976/) <br>
  **TL;DR**<br>
  *yarn berry workspace*를 통해 우아한 형제들 개발팀이 어떻게 프로젝트를 어떻게 모노레포로 바꾸었는가에 대한 이야기입니다. <br>
  _yarn berry workspace_ 명령 등의 필요한 정보가 없기 때문에, `모노레포 도입 사례`로써의 의미가 큰 글입니다.
- [yarn workspace 모노레포 설정하기 - designdevelop@Medium](https://medium.com/@designdevelop/yarn-workspaces-%EB%AA%A8%EB%85%B8%EB%A0%88%ED%8F%AC-%EB%8F%84%EC%9E%85%EA%B8%B0-c0310ca41c0e) <br>
  **TL;DR** <br>
  이 글은 *yarn berry*를 설치하는 법부터 *yarn berry workspace*를 통해 모노레포를 구성하는 법,
  _yarn berry workspace_ 명령을 올바르게 사용하기 위해 알아야 하는 _hoist_ 등의 개념을 모두 포함해 설명하고 있습니다. <br>
  `모노레포 도입을 위한 모든 내용`으로써의 의미가 큰 글입니다.

## 2.1. 호이스팅

- [node_modules로부터 우리를 구원해 줄 Yarn Berry - Toss Tech](https://toss.tech/article/node-modules-and-yarn-berry) <br>
  _호이스팅_ 개념을 이해하기 위해 문서를 찾고있던 중 찾은 문서입니다. <br>
  _유령 의존성 (Phantom Dependency)_ 내용을 이해함으로써 *호이스팅*의 개념을 이해할 수 있습니다. <br><br>
  이러한 내용을 제외하더라도 `Yarn Berry`에 대한 다양한 내용을 포함하고 있습니다. <br>
  `Yarn Berry`에 대해 깊게 파보고 싶다면, [이 문서](https://toss.tech/article/node-modules-and-yarn-berry)를 확인해보세요.
