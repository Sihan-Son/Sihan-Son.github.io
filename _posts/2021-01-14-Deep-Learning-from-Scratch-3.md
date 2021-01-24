---
layout: post
title: "[Book] 밑바닥부터 시작하는 딥러닝 3 "
date: 2021-01-14
excerpt: "내가 직접 만드는 딥러닝 프레임워크 DeZero"
sitemap:
    changefreq: daily
    priority: 1.0
review: true
tag:
    - 밑바닥
    - book
    - Hanbit
    - ML
    - DL
comments: true
---

`Deep Learning`(이하 `DL`)은 배우기 쉬운데 어려운, 굉장히 아이러니한 분야가 되어가고 있습니다. 강력하고 좋은 프레임워크와 튜토리얼들이 배움과 사용의 문턱을 굉장히 낮추어 주었습니다. 이는 동전의 양면처럼 장단점이 극명하게 나뉘는 결과를 초래했습니다. 문턱이 낮아지면서 다양한 아이디어와 기술들이 분야에 기여하고, 흥미 있고 능력있는 친두들을 일찍 발굴해 내는 등의 장점이 있습니다. 동시에 레토르트 식품을 서빙하는 식당들이 많아지고 있습니다. 모델에 대한 이해 없이 하이퍼파라메타와 데이터셋만 조금 바꾸어 결과를 뽑아 사용하는 말 그대로 밑바닥이 부족한 사용자들도 속출하는 듯 합니다. 저도 후자에 속하는 사람이었습니다.

밑바닥이 부족하다 보니 모델을 튜닝하고 구성하는데 제약사항이 많이 발생했습니다. 지식의 링크도 구멍이 많아서 공부를 하거나 모델을 만질때 내가 정확히 뭘 모르는지 모르고 있었고 이 함수가 대체 왜 필요한지 고민할 뿐 모르고 사용했습니다.

자동미분을 고차미분으로 이것을 결국 `Backpropagation` 완성형으로 만들며 코드를 구조화 합니다. 이 책은 단순히 `DL`만을 다루지 않고 구조화 된 코드, 메모리 관리, 시각화 등 다양한 파트를 만지면서 프레임워크를 쌓아 올립니다. 한 단계, 한 단계 단계 별로 완성 확장, 완성 확장하며 아키텍쳐를 형성을 하고 결국 프레임워크가 탄생합니다. 통제 당하면서 순서에 따르는 프로그래밍이 답답하고 불만족스러울 수는 있지만 다음 단계의 이름을 보고 어떤 코드가 짜여질까 고민하는 것도 이 책으로 공부하는 하나의 방법이 될 수 있을 것입니다.

책을 즐겨 읽는 편이라 번역에 생각보다 까탈스러운 편이라고 생각합니다. 그래서 이런 번역된 기술 서적들을 볼 때는 논리적인 부분이 아닌 번역 그 자체 때문에 읽는 흐름이 막히는 것은 별로 좋아하지 않습니다. 베타리딩을 하면서 역자님과 소통을 하면서 단어랑 흐름에 굉장히 고민을 많이하신 흔적을 발견했고, 실제로 전 읽으면서 글 자체는 막히는 것 없이 잘 읽혔던 것 같습니다. 자동미분, 역전파 부분에서 막히는건 번역 문제가 아니에요. 어려운게 맞아요.

번역도 깔끔하게 좋았고, 내용도 충분히 알찬 책이지만 `DL`을 시작하는 용으로는 별로 추천드리지는 않습니다. `DL`을 구성하는 요소들을 만들지만 개념이 잡히지 않은 상태에서는 이 책이 말하고자하는게 잘 와닿지 않을 수 있습니다. 그래서 제 추천은 `DL`을 처음 시작 할 때는 <a href='https://sihan-son.github.io/alone-dl'>`혼자 공부하는 머신러닝+딥러닝`</a>, <a href=''>`실체가 손에 잡히는 딥러닝`</a>, <a href='https://sihan-son.github.io/do-it-deep-learning'>`Do it 딥러닝`</a>, <a href=''>`밑바닥 부터 시작하는 딥러닝 1`</a>(나열 된 책들 서평 작업 중입니다.) 등등 정말 시작하는 사람들을 위해 씌여진 책이나 강의보고 보시는걸 추천 합니다.

이 책에 대한 평을 제가 좋아하는 분이 쓰신 이 책 <a href="https://jehyunlee.tistory.com/12">서평</a>에 쓰신 문장을 빌려 하고 싶습니다. `뼈에 새기진 못해도 흔적은 남길 수 있는 책`입니다.

난이도: 중하  
추천대상: `DL` 생기초는 익힌 독자층

---

베타리더로 참가해 작성한 서평입니다.

---

![swift](https://sihan-son.github.io/public/book/hanbit/DL_Scratch_3.jfif)

정말 잘 쓰고 싶었는데 어딘가 만족 안되는 글이 되었습니다.  
20번째 서평인데 이번달에 한두권 정도 더 쓴 다음에 블로그 테마부터 전체적인 개편을 하려고 합니다. 지금까지는 책에 대한 간단한 내용소개와 다른 책과 차이점, 추천 독자, 역서의 경우 번역에 대해 이야기를 했는데추가 했으면 하는 내용이 있으면 페이스북이나 블로그 댓글로 피드백 주시면 반영해 보겠습니다.