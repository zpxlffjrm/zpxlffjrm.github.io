---
title: "데이터 모델링"
toc: true
toc_sticky: true

categories:
  - Mongo
tags:
  - mongos
  - certificate
  - data modeling

last_modified_at: 2020-04-08T12:11:00+00:00
---

## 데이터 모델링

데이터 모델링은 현실을 모방하여 데이터베이스에 저장될 데이터의 모델을 만드는 것이다.

데이터 모델은 어떤 오브젝트가 어떤 타입을 가져야하는지 명시해야 하며 다른 오브젝트와의 관계와 규약을 규정하는 실제가 아닌 추상적인 모델이다.
하지만 해당 모델은 수도코드와 비슷한 추상적인 모델이므로 내용을 반영하여 실제 모델로 제작하는 과정이 필요하다.

어떻게 보면 건축가의 기획서으로 볼수 있다.
[참고 자료](https://www.guru99.com/data-modelling-conceptual-logical.html)

그럼 몽고디비에서는 어떨까?

## 몽고디비에서 데이터 모델링

### 핵심 룰

가장 핵심적인 룰은 몽고디비는 형식에 관계없이 저정한다는 것이다.

NoSQL 데이터베이스의 특성상 별도의 스키마를 필요로 하지 않기 때문!
그렇기 때문에 하나의 도큐먼트에서 상호작용이 필요한 데이터들, 필요한 데이터들은 하나의 도큐먼트에서 확인 가능한것이 좋다.