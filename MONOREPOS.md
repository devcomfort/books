<h1>모노레포 명령어 정리</h1>

[yarn workspace 모노레포 설정하기 - designdevelop@medium](https://medium.com/@designdevelop/yarn-workspaces-%EB%AA%A8%EB%85%B8%EB%A0%88%ED%8F%AC-%EB%8F%84%EC%9E%85%EA%B8%B0-c0310ca41c0e)을 참조하여 작성하였습니다.

- [명령어 정리](#명령어-정리)
  - [패키지 관리](#패키지-관리)
  - [*nohoist*에 대하여](#nohoist에-대하여)

# 명령어 정리

## 패키지 관리

- `yarn init -y`: 프로젝트 초기 설정
- `yarn workspace <프로젝트명> add <패키지 이름>`: 해당 프로젝트에 원하는 패키지를 설치
- `yarn workspace <프로젝트명> remove <패키지 이름>`: 해당 프로젝트에 원하는 패키지를 설치
- `yarn add <패키지 이름> -w`: 루트 디렉토리에 패키지 추가

## *nohoist*에 대하여

`Yarn Berry workspaces`를 통해 관리되는 모노레포에서는 *유령 종속성*에 대해 어느 정도 알아야 할 필요가 있습니다. <br>
기존의 `yarn`과 `npm`에서는 `node_modules`를 통해 패키지를 관리해왔습니다. <br>
`Yarn Berry`에 오면서 `node_modules`가 아닌 `PnP` 방식을 사용했고, 이로 인해 *유령 종속성*이 생겼으며, 이에 따른 여러 장점이 생겼습니다.

다만 `PnP` 방식을 지원하지 않는 몇몇 패키지에 대해서는 여전히 `node_modules`를 사용해야 하는데, 이를 위해서 `nohoist` 옵션이 존재합니다.

`nohoist`에 들어간 모노레포는 종속성 중복 검사에서 제외됩니다. `Yarn Berry`의 종속성 중복 제거를 통한 최적화 대신에 원활한 동작을 할 수 있도록 해주는 셈입니다.
