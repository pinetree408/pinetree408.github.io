---
layout: post
maintitle: How to fix gitignore issue
subtitle: gitignore 설정 후 정상 적용 문제 해결하기
---

## What issuse

Git를 사용하여 프로젝트를 진행하면서 점점 gitignore에 등록해야 할 디렉토리나 파일이 늘어났다. 따라서 해당 파일들을 .gitignore 파일에 등록하였는데,  이미 저장소에 푸시된 내용이 삭제되지는 않는 문제가 발생했다. 해당 issue를 검색을 해보면 .gitignore 에 적용한 설정이 정상적으로 동작하지 않는다는 내용이 많았다.

## How to fix

아래의 명령을 사용하면 곧바로 설정이 적용된다. 푸시를 하게되면 저장소에 이미 올라가있는 파일들도 삭제된다.

```sh
$ git rm -r --cached .
$ git add .
$ git commit -m "fixed untracked files"
```