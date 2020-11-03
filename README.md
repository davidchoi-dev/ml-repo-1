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

더 나아가 사고 발생시 머신러닝 모델을 통해 Fraud 가능성이 높은 경우, 담당자에게 고위험군임을 알리는 서비스까지 구축해보려 한다.


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

알고리즘 (모델마다 그리드서치-> 모델의 최적 파라미터를 찾기위함)

1. 다이렉트 그냥 돌려봄 (예측1 / 기준) 
2. 다운샘플링 - 1:10 정도 약 300개정도로 설정/각자 다름, 각 방법마다 샘플링 크기는 달라질 수 있음 (예측2)
3. 오버샘플링 (예측3)
4. 오버/다운샘플링 (예측4)
----------------------
모델평가 => k-folding 5겹으로 선진행
----------------------
5. 나온 4개의 결과를 다시 오버/다운샘플링 (예측5) ** 앙상블 기법의 성능이 좋아야하는데 안좋으니 30개 밖에 안되는 데이터가 보팅이 제대로 되지 않은게 아닌가?
6. 특정 클래스에 가중치를 줌 (예측6)
---------------------- ** pipeline을 잘꾸미는 것이 중요
모델평가 => Cross validation


* 사기 탐지 정확도 평가 단계 Point :

암을 진단하는 사례에서는 정상을 Positive로 설정한다면, 모든 환자를 정상으로 진단해도 Accuracy가 99%가 나온다.
이 경우 1% 암 환자 진단을 놓치게 되므로 의미가 없다.

![1_pOtBHai4jFd-ujaNXPilRg](https://user-images.githubusercontent.com/68367214/97948653-8d8c8180-1dd4-11eb-9460-9205b4467a37.png)

본 프로젝트에서 정상을 Positive, Fraud를 False로 상정해보자.

Fraud를 정상으로 분류하는 False Positive(오탐)이 높아지면 사기 손실 비용이 커진다. 

반면, 정상을 Fraud로 잘못 분류하는 False Negative(미탐)이 높아지면 조사과정에서 고객 불만이 커진다.

따라서 중요하게 생각하는 요소에 따라 모델의 평가에 대한 정답을 내리기 어려움.

그래서 Accuracy, Recall, Precision 을 모두 고려하여야하며 어떤 모델이 좋은 모델일지에 대한 기준을 정해야함
(Case: Trade-off 관계 내에서, 이익 극대화와 고객의 불만 최소화 모두를 충족하기는 어려움.)

=> 본 프로젝트에서는 Fraud를 밝혀내는 것을 더 중요한 목적으로 상정하고, Recall(재현율)에 조금 더 초점을 맞추어 분석.


## Project Improvements

1. 추가 Feature 제안 : 반납 지연시간, 요금 연체 횟수도 추가로 수집이 된다면 유의미할 수 있음.


## Presentation Resourses

1. Sweetviz
2. Draw.io
3. Tableau


## learning materials

1. Socar 약관 : https://www.socar.kr/terms
2. Hands-On Machine Learning with Scikit-Learn and TensorFlow / Aurélien Géron
