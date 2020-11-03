# Socar Fraud Detection Project

Teams: 이진서, 임상우, 김재욱 (FastCampus Datascience School 14th)


![image](https://user-images.githubusercontent.com/68367214/97532893-a115a200-19fa-11eb-9049-2dcadfc44eac.png)

교보생명의 보험사기 사전예측

교보생명이 인공지능(AI)과 머신러닝 기술로 보험사기 가능성을 사전에 경고해주는 
보험사기예측시스템(K-FDS)을 자체 개발해 본격 운영에 들어갔다고 올해 5월 26일 발표.

실제적으로 교보생명에서는 1년간의 시범적 운영을 통해 200여건의 부당 보험금 지급 방지에 성공.


## Goals

![Socar_project-Page-3](https://user-images.githubusercontent.com/68367214/97603219-891c3d80-1a4f-11eb-9693-9f43ab8b0c99.png)

본 쏘카 프로젝트에서는 과거 데이터를 기반으로 머신러닝 모델을 통해, Fraud 인 고객을 탐지해내는 것을 목적으로 한다.
 
효과적으로 선별할 수 있는 모델을 적용하여, Fraud 고위험군 사용자들을 분류해낸다면 자사에 이익을 줄 수 있을것이다. 

더 나아가 최초 사고 식별시, 머신러닝의 여러기법을 통해 Fraud 일 가능성이 높은 경우, 담당자에게 고위험군임을 알리는 서비스까지 구축해보려 한다.


## Execution

1. EDA
2. 데이터 전처리
3. 분석 모델 적용 및 인사이트 도출
4. 사전알림 서비스 구축


## Machine Learning Model

* Machine Leaning - Supervised Learning - Classification

1. Decision Tree
2. Logistic Regression
3. KNN
4. SVM
        

## Architectures

![Socar_project-Page-2](https://user-images.githubusercontent.com/68367214/97545022-bf38cd80-1a0d-11eb-84a7-30a7d3d5a116.png)


## Details

* 모델링 과정

1. 
2. 
3. 


* 사기 탐지 정확도 평가 단계 Point :

![99DC064C5BE056CE10](https://user-images.githubusercontent.com/68367214/97944654-865f7680-1dc8-11eb-998f-10d044c5735d.png)

암을 진단하는 사례에서 정상을 Positive로 설정한다면, 모든 환자를 정상으로 진단해도 Accuracy가 99%가 나온다.
이 경우 1% 암 환자 진단을 놓치게 되므로 의미가 없다.

그러므로 본 사기탐지 프로젝트에서도 Fraud의 경우를 Positive(1), 정상을 Negative(0)로 설정했을때,

False Negative(미탐)이 높아지면 사기 손실 비용이 커지고, 정상을 사기로 잘못 분류하는 False Positive(오탐)이 높아지면 조사과정에서 고객 불만이 커진다.

1. 적정 FN과 FP를 설정하기 위해서는 기업의 정책과 현장사례들을 통하여 조정하는 과정이 필요.
2. 중요하게 생각하는 요소에 따라 모델의 정확도 평가에 대한 정답을 내리기 어려움.
3. Accuracy, Recall, Precision 을 모두 고려하여야함.
(일반적으로 Trade-off 관계 내에서, 이익 극대화와 고객의 불만 최소화 목적에 부합하는 최적 지점 확보 필요.)

=> 본 프로젝트에서는 Fraud를 밝혀내는 것이 더 중요한 목적으로 상정하고, Recall(재현율)을 유의미하게 확보함을 목적으로함.


## Project Improvements

1. 추가 Feature 제안 : 반납 지연시간, 요금 연체 횟수도 추가로 수집이 된다면 유의미할 수 있음.


## Presentation Resourses

1. Sweetviz
2. Draw.io
3. Tableau


## learning materials

1. Socar 약관 : https://www.socar.kr/terms
2. Hands-On Machine Learning with Scikit-Learn and TensorFlow / Aurélien Géron
