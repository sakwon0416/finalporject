# finalproject

1. what i did
- voting 모델을 사용하여 주어진 데이터를 학습하고 이를 기반으로 판단하였다
- voting machine에는 각 random forest, MLP모델, Bagging 모델이 들어갔다.
- Bagging model은 가장 가까운 것을 기반으로 판단하는 knn모델로 만들어졌다.

2. dataset에 대한 설명
- 4종류의 뇌종양이 있고, 사진으로 각각 분류되어있었다.

3. 내가 고른 모델:
-voting 모델을 선택하였는데 이는 각 모델의 예상을 합하여 결과를 산출하는 모델이다.
-voting 모델에는 각각 randomforest와 MLP모델 그리고 knn으로 이루어진 Bagging 모델이 들어갔다

 4.hyperparameter
 -randomforest는 깊이가 최대 1000이도록 설계하였고
 - Bagging모델은 평가모델을 knn으로 설계하였고 최대 sample을 100개로 늘렸다.
 - MLP모델은 tanh로 활동모델을 결정하였고, 최대 반복을 1200회, 그리고 학습 방식은 적응형으로 바꾸었다.
