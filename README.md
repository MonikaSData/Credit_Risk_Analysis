# Credit_Risk_Analysis

## Overview of Project

Use credit dataset from LendingClub to evaluate three machine learning models by using resampling to determine which is better at predicting credit risk

**Purpose:**
The purpose of this project is to determine if using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

**Task:** 
Employ different techniques to train and evaluate models with unbalanced classes. Evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

**Approach:**

- *Use Resampling Models to Predict Credit Risk*
- *Use the SMOTEENN Algorithm to Predict Credit Risk*
- *Use Ensemble Classifiers to Predict Credit Risk*
- *A Written Report on the Credit Risk Analysis*

**Method:** Using scikit-learn and imbalanced-learn libraries, Google Collab.


## Resources
- Data Source: [LoanStats_2019Q1.csv](LoanStats_2019Q1.csv); 
- Source Code: 
    [credit_risk_resampling.ipynb](credit_risk_resampling.ipynb); [credit_risk_ensemble.ipynb](credit_risk_ensemble.ipynb);
  
- Programming Languages: Python
- Software/Tools: Google Collab, VS Code

## Results
Describe the balanced accuracy score and the precision and recall scores of all six machine learning models. 

**Random Oversampling**

![Resources/RandomOversampling.png](Resources/RandomOversampling.png)

- The accuracy score of this model is ~67%
- For high risk predictions the precision is 1% and recall/sensitivity is 64%
- For the low risk predictions the precision is 100% and recall/sensitivity is 67%



**SMOTE Oversampling**

![Resources/SMOTE.png](Resources/SMOTE.png)

- The accuracy score of this model is ~65% 
- For high risk predictions the precision is 1% and recall/sensitivity is 62%
- For the low risk predictions the precision is 100% and recall/sensitivity is 65%

**ClusterCentroids Resampler**

![Resources/ClusterCentroids.png](Resources/ClusterCentroids.png)

- The accuracy score of this model is ~41% (the lowest of all models)
- For high risk predictions the precision is 1% and recall/sensitivity is 63%
- For the low risk predictions the precision is 100% and recall/sensitivity is 41%

**SMOTEENN**

![Resources/SMOTEENN.png](Resources/SMOTEENN.png)

- The accuracy score of this model is ~55%
- For high risk predictions the precision is 1% and recall/sensitivity is 71%
- For the low risk predictions the precision is 100% and recall/sensitivity is 55%

**Balanced Random Forest Classifier**

![Resources/BalancedRandomForestClassifier.png](Resources/BalancedRandomForestClassifier.png)

- The accuracy score of this model is ~77%
- For high risk predictions the precision is 3% and recall/sensitivity is 67%
- For the low risk predictions the precision is 100% and recall/sensitivity is 87%

**Easy Ensemble AdaBoost Classifier**

![Resources/EasyEnsembleClassifier.png](Resources/EasyEnsembleClassifier.png)

- The accuracy score of this model is ~93% (the highest accuracy score out of all 6 models)
- For high risk predictions the precision is 9% and recall/sensitivity is 92%
- For the low risk predictions the precision is 100% and recall/sensitivity is 94%


## Summary
 