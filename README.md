# Credit_Risk_Analysis

## Overview
For this project, I used machine learning to analyze credit card risk in a dataset. In order to complete this project, I had to take the following steps: 

1. Import the "imbalance-learn" and "scikit-learn" libraries
2. Oversample the data using the "RandomOverSampler" and "SMOTE" alogrithms
3. Undersample the data using the "ClusterCentroids" algorithm
4. Use a combinatorial approach of over and undersampling using the "SMOTEENN" algorithm
5. Compare two new models that reduce bias: "BalancedRandomForestClassifier" and "EasyEnsembleClassifier", to predict credit    risk
6. Evaluate the performance of the models and determine whether they should be used to predict credit risk

## Results

### 1. Naive Random Oversampling

<img width="806" alt="naive_random_oversampling" src="https://user-images.githubusercontent.com/111243284/209411963-35d80713-a3f6-4f70-b8eb-da9c96378cfc.png">

#### Balanced Accuracy: 0.6456130066757718
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: .61/.68

### 2. SMOTE Oversampling

<img width="779" alt="SMOTE_oversampling" src="https://user-images.githubusercontent.com/111243284/209412048-dd3f7632-3f42-4ed4-afcd-77033b1dd720.png">

#### Balanced Accuracy: 0.6234433606890912
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: .61/.64

### 3. Undersampling

<img width="810" alt="undersampling" src="https://user-images.githubusercontent.com/111243284/209412062-7196f1f1-dd45-4cce-b2e0-0a79c83e165e.png">

#### Balanced Accuracy: 0.6234433606890912
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: .61/.45

### 4. Combination Over and Under Sampling

<img width="806" alt="combination over-under sampling" src="https://user-images.githubusercontent.com/111243284/209412077-b6d9d051-bd1e-4afb-b3bd-5b8b01cfdac5.png">

#### Balanced Accuracy: 0.5292734810302525
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: .70/.58

### 5. Balanced Random Forest Classifier

<img width="801" alt="balanced_random_forest_classifier" src="https://user-images.githubusercontent.com/111243284/209412089-086316ad-d5be-40c0-aab0-ab553e993370.png">

#### Balanced Accuracy: 0.7877672625306695
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: .67/.91

### 6. Easy Ensemble AdaBoost Classifier

<img width="787" alt="easy_enseble_adaboost_classifier" src="https://user-images.githubusercontent.com/111243284/209412095-5106ea31-106e-46bb-a626-a1fb8d377a3f.png">

#### Balanced Accuracy: 0.925427358175101
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: .91/.94

## Summary



