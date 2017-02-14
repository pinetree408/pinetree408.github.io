---
layout: post
maintitle: Python dict & json
subtitle: how to use python dict json
---

###version: 0.0.1

##문제점
기존의 python web framework를 사용할때, 모델에서 data를 이쁘게 simplfy하기위해서,
부가적으로 데이터를 dict > json으로 변경해서 사용해왔다.
그런데 flask에서 render_template 함수에 json를 바로 전달해 사용하면,
javascript에서는 추가의 후처리없이 바로 property들을 call해서 사용할 수 있었다.
하지만, jinja html에서 같은 방법으로 call을 하는 경우 json type에서 호출이 되지 않았다.

##해결방안
어쩔 수 없이, json을 다시 dict을 바꾸어 사용하니 해결되었다.
### json to dict
```python
dict = json.loads(json)
```
### dict to json
```python
json = json.dump(dict)
```
