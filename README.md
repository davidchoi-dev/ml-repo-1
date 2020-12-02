![SOCAR_LOGO_RGB_로고타입](https://user-images.githubusercontent.com/68367214/100833111-a019d980-34ac-11eb-9810-8bcbfed45e2b.png)



# Socar Fraud Detection Project



Members : 이진서, 임상우, 김재욱 (FastCampus Datascience School 14th)

  <A href="SOCAR_FINAL.html"> PPT파일 링크 </A>
<P>


## Goals
![Socar_project-Page-4 (3)](https://user-images.githubusercontent.com/68367214/98901948-08058180-24f8-11eb-97b2-fa69c826d7b4.png)

* Build Fraud Detection ML Model for SOCAR (dataset provider).


## Procedure

1. EDA 
2. Pre-processing
3. Modeling
4. Validation
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

Step 1. Baseline Set (with Raw Data)

Original Models
- Logistic Regression
- SupportVectorMachine
- RandomForestClassifier

Extended Models
- EasyEnsembleClassifier
- BalancedRandomForestClassifier
- RUSBoostClassifier



Step 2. Preprocessing

- One-Hot-Encoding
- Outlier Removal
- Scaling : RobustScaler, MinMaxScaler
- Train/Test Split



Step 3. Hyperparameter Tuning 

 + Gridsearch (Recall Priority)


Step 4. Imbalanced Data Tuning

 + Resampling (Oversampling, Undersampling)


Step 5. Validation

 + Easy Ensemble Classifier with StratifiedKFold

 
Step 6. Conclusion
- Limitation
- Interpretation


## Presentation Resourses

1. Sweetviz
2. Draw.io


## learning materials

1. Terms of Socar : https://www.socar.kr/terms
2. Hands-On Machine Learning with Scikit-Learn and TensorFlow / Aurélien Géron
