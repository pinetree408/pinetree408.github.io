---
layout: post
maintitle: Start Blog With Github and Jekyll
subtitle: github과 jekyll 사용해서 blog 시작! 
---

## How to use Github Pages

Github Pages는 github의 프로젝트를 만들 수 있게 github에서 제공하고 있는 서비스이다. 사이트를 만들기 위해서 서버를 설치하고 웹서버 환경을 구축할 필요없이 github에 웹 리소스를 Reposity에 git push 하는 것 만으로 웹 사이트를 만들 수 있다.

GitHub page를 생성하는 방법은 gh-pages branch에 index.html 파일을 git push 하는 것 만으로도 만들 수 있고, 다른 static website generator framework를 사용해도 된다. GitHub에서는 공식적인 Database를 지원하고 있지 않기 때문에 static website를 사용해야 한다.

## How to use Github Account Pages

GitHub는 프로젝트 페이지 말고도 GitHub Account Page를 만들 수 있다. 만약 GitHub의 계정이 test 라고 한다면 http://test.github.io 라는 개인 페이지를 만들 수 있는 것이다. 프로젝트 페이지와 달리 계정 페이지는 gh-pages branch를 사용하는 것이 아니라 master branch를 사용한다. 계정 페이지를 만들기 위해서는 GitHub에 새로운 리파지토리를 생성해야한다.

즉 계정이 test라고 한다면 Reposity의 이름을 test.github.io 라고 만든다. 그러면 https://github.com/test/test.github.io 과 같이 GitHub에 Reposity가 생성이 된다.현재는 리파지토리가 비어져 있을 것이다. 이것을 자신의 컴퓨터에 clone을 한다.

## How to use Jekyll