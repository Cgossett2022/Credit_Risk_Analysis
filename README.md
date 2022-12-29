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
#### Recall: high-risk = .61 low-risk = .68

### 2. SMOTE Oversampling

<img width="779" alt="SMOTE_oversampling" src="https://user-images.githubusercontent.com/111243284/209412048-dd3f7632-3f42-4ed4-afcd-77033b1dd720.png">

#### Balanced Accuracy: 0.6234433606890912
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: high-risk = .61 low-risk = .64

### 3. Undersampling

<img width="810" alt="undersampling" src="https://user-images.githubusercontent.com/111243284/209412062-7196f1f1-dd45-4cce-b2e0-0a79c83e165e.png">

#### Balanced Accuracy: 0.6234433606890912
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: high-risk = .61 low-risk = .45

### 4. Combination Over and Under Sampling

<img width="806" alt="combination over-under sampling" src="https://user-images.githubusercontent.com/111243284/209412077-b6d9d051-bd1e-4afb-b3bd-5b8b01cfdac5.png">

#### Balanced Accuracy: 0.5292734810302525
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: high-risk = .70 low-risk = .58

### 5. Balanced Random Forest Classifier

<img width="801" alt="balanced_random_forest_classifier" src="https://user-images.githubusercontent.com/111243284/209412089-086316ad-d5be-40c0-aab0-ab553e993370.png">

#### Balanced Accuracy: 0.7877672625306695
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: high-risk = .67 low-risk = .91

### 6. Easy Ensemble AdaBoost Classifier

<img width="787" alt="easy_enseble_adaboost_classifier" src="https://user-images.githubusercontent.com/111243284/209412095-5106ea31-106e-46bb-a626-a1fb8d377a3f.png">

#### Balanced Accuracy: 0.925427358175101
#### Precision: The precision is low for high-risk loans and is high for low-risk loans.
#### Recall: high-risk = .91 low-risk = .94

## Summary
The results are summarized below:

**1. Naive Random Oversampling**
-High Risk: 64.6% accuracy, 1% precision, 61% recall, and 2% F1 Score
-Low Risk: 64.6% accuracy, 100% precision, 68% recall, and 81% F1 Score

**2. SMOTE Oversampling**
-High Risk: 62.3% accuracy, 1% precision, 61% recall, and 2% F1 Score
-Low Risk: 62.3% accuracy, 100% precision, 64% recall, and 78% F1 Score

**3. Undersampling**
-High Risk: 62.3% accuracy, 1% precision, 61% recall, and 1% F1 Score
-Low Risk: 62.3% accuracy, 100% precision, 45% recall, and 62% F1 Score

**4. Combination Over and Under Sampling**
-High Risk: 52.9% accuracy, 1% precision, 70% recall, and 2% F1 Score
-Low Risk: 52.9% accuracy, 100% precision, 58% recall, and 73% F1 Score

**5. Balanced Random Forecast Classifier**
-High Risk: 78.8% accuracy, 4% precision, 67% recall, and 7% F1 Score
-Low Risk: 78.8% accuracy, 100% precision, 91% recall, and 95% F1 Score

**6. Easy Ensemble AdaBoost Classifier**
-High Risk: 92.5% accuracy, 7% precision, 91% recall, and 14% F1 Score
-Low Risk: 92.5% accuracy, 100% precision, 94% recall, and 97% F1 Score


Based on the results, I would recommend using the EasyEnsembleClassifier model because it had the highest accuracy, precision, and recall for high risk loans. Since we are most concerned with high risk candidates potentially defaulting on their loans, it's best to identify these candidates before extending credit. When compared to the other models, the EasyEnsembleClassifier does the best job minimizing risk. 



