# Memory End to End Network를 이용한 한국어 QA task 해결
----------------------------------------------------

목표
----
Facebook bAbI QA task 해결을 위해 만들어진 Memn2n 알고리즘을 한국어 QA task 적용


과정
---
1. 아래의 코드를 참고해서 bAbI QA 첫 번째 task 트레이닝 및 검증

https://github.com/carpedm20/MemN2N-tensorflow

https://github.com/vinhkhuc/MemN2N-babi-python.git

https://github.com/fchollet/keras

https://github.com/1202kbs/MemN2N-Tensorflow

https://github.com/domluna/memn2n#joint-training-results

* 대체로 90% 후반대의 accuracy

2. 한국어로 번역한 첫 번째 task 트레이닝 및 검증

Accuracy 약 70%

3. 해리포터 소설로 데이터 세트 제작

단어 수 15142개, 트레이닝세트 문제 수 473, 테스트세트 문제 수 31, 스토리 최대 단어 수
5651

4. 제작한 데이터 세트로 트레이닝 및 검증

퍼포먼스가 낮음???, 코드에 따라서 결과가 다름???


문제점
-----

* bAbI QA task에 비해 제작한 데이터 세트의 스토리가 사이즈가 굉장히 크고 복잡함

* 그에 비해서 학습시킬 수 있는 문제 수는 굉장히 적었음

* 참고했던 코드를 이해하는 데 드는 어려움

* 시간 부족으로 학습 횟수가 적었음


차후 계획
--------

* bAbI QA task를 전부 번역해서 난이도를 낮춰서 도전

* Tensorflow 공부


참고 문헌
--------

Sainbayar Sukhbaatar, Arthur Szlam, Jason Weston, Rob Fergus, "End-To-End Memory Networks", arXiv:1503.08895 [cs.NE], https://arxiv.org/abs/1503.08895v5.
