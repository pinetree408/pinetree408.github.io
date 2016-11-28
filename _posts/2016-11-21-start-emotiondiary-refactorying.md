---
layout: post
maintitle: Start emotiondiary refactorying
subtitle: initialize flask develope env
---

## How to setup
Install flask with python virtualenv

```sh
$ virtualenv venv
$ . venv/bin/activate
$ pip install flask
$ pip freeze > requirements.txt
```

## Git push 시에 주의할 점
.gitignore 파일을 꼭 추가하고 진행한다. python app framework를 virtualenv와 개발을 할시에 basic으로 적용이 가능한 gitignore 파일의 포맷은
[dotfile/gitignore](https://github.com/pinetree408/dotfile/blob/master/gitignore)에 있다.
새 repo를 만들고 진행할때, 잊지말고 추가하자.
혹시 추가를 못하는 경우에는 [gitignore-issue](http://pinetree408.github.io/2015/05/04/How-to-fix-gitignore-issue posting)을 따라서 진행한다.
