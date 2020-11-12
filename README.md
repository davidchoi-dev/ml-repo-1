# Socar Fraud Detection Project

Teams: 이진서, 임상우, 김재욱 (FastCampus Datascience School 14th)



## Goals
![Socar_project-Page-4 (3)](https://user-images.githubusercontent.com/68367214/98901948-08058180-24f8-11eb-97b2-fa69c826d7b4.png)

* Build Fraud Detection ML Model based on Past Data-set.


## Execution

1. EDA 
2. Data Preprocess 
3. Build & Train Model
4. Model Validation
5. Conclusion


## Machine Learning Model

![그림1](https://user-images.githubusercontent.com/68367214/98902177-86faba00-24f8-11eb-92cc-5edd15d121ab.png)


1. LogisticRegression
2. SupportVectorMachine
3. RandomForest

4. EasyEnsembleClassifier
5. BalancedRandomForestClassifier
6. RUSBoostClassifier



## Details

Step 1. Baseline Set 

Original Models
- Logistic Regression
- SupportVectorMachine
- RandomForestClassifier

Extended Models
- EasyEnsembleClassifier
- BalancedRandomForestClassifier
- RUSBoostClassifier

 + with Raw Data

Step 2. Preprocess


 + with One-Hot-Encoding
 + with Train/Test Split


Step 3. Hyperparameter Tuning 

 + with Gridsearch (Recall Priority)


Step 4. Imbalanced Data Tuning

 + with RobustScaler (For Overfitting)
 + with Resampling (Oversampling, Undersampling, Under+oversampling)


Step 5. Validation

Original Models
- Logistic Regression
- SupportVectorMachine
- RandomForestClassifier

Extended Models
- EasyEnsembleClassifier
- BalancedRandomForestClassifier
- RUSBoostClassifier

 + with Resampling
 + with StratifiedKFold

 
Step 6. Conclusion
- How to set Benchmarks
- Interpretation

## Presentation Resourses

1. Sweetviz
2. Draw.io
3. Airdrop


## learning materials

1. Terms Of Socar : https://www.socar.kr/terms
2. Hands-On Machine Learning with Scikit-Learn and TensorFlow / Aurélien Géron
