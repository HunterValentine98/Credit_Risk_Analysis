# Credit_Risk_Analysis

## Overview of the Analysis
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once I finished, I evaluated the performance of these models and made a written recommendation on whether they should be used to predict credit risk.

## Results
### Naive Random Oversampling
- Precision Score: 0.01
- Recall Score: 0.71
- F1 Score: 0.02

### SMOTE Oversampling
- Precision Score: 0.01 
- Recall Score: 0.61 
- F1 Score: 0.02

### Undersampling
- Precision Score: 0.01
- Recall Score: 0.69
- F1 Score: 0.01

### Combination Sampling
- Precision Score: 0.01
- Recall Score: 0.70 
- F1 Score: 0.02

### Balanced Random Forest Classifier
- Precision Score:
- Recall Score:
- F1 Score:

### Easy Ensemble AdaBoost Classifier
- Precision Score:
- Recall Score:
- F1 Score:

## Summary
