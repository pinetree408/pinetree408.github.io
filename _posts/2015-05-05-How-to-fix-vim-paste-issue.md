---
layout: post
maintitle: How to fix vim paste issue
subtitle: vim auto indent mode에 의한 paste 개행 문제
---

## What issuse

vim을 띄우고, code를 paste 할 때, vim auto indent mode 때문에 paste한 코드의 개행이 엉망이 되어 버린다.

## How to fix

vim 의 command mode로 들어가서 다음 명령어를 쳐서 paste mode 로 전환하면 자동 개행이 꺼지므로 코드가 보기 좋게 붙게 된다.

```
set paste
```

수정 완료 후 paste mode를 끌려면 다음 명령어를 치면된다.

```
set nopaste
```
