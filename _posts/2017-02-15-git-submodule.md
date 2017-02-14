---
layout: post
maintitle: Git submodule
subtitle: how to use git submodule
---

### version: 0.0.1

## Submodule이 있는 git project clone 하기
서브모듈이 포함된 리파지터리를 클론하면, 이전에 포함시켰던 submodule의 디렉토리는 존재한다.
하지만 내용은 비어 있다.
먼저, 서브모듈을 가져오려면 먼저 초기화 해야한다.

```sh
$ git submodule init
```

다음으로 서브모듈을 업데이트한다.

```sh
$ git submodule update
```

이때, submodule을 update한다는 의미는, 현재 부모 리파지터리의 커밋에서 참조하고 있는 서브모듈의 커밋을,
자식 리파지터리의 리모트에서 체크아웃해온다는 뜻이다.
자식 프로젝트의 디렉토리로 이동해 로그를 확인해보면 대상 커밋으로 채워진 걸 확인할 수 있다.

하지만, 자식 프로젝트의 브랜치도 확인해보면,
브랜치를 보면 detached 상태로 되어 있다.
부모 프로젝트에서 서브모듈을 업데이트하면, 브랜치나 태그 같은 간접 레퍼런스를 가져오는 게 아니라,
저장된 특정 커밋을 체크아웃하기 때문이다.
