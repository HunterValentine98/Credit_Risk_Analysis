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
- Precision Score: 0.03
- Recall Score: 0.70
- F1 Score: 0.06

### Easy Ensemble AdaBoost Classifier
- Precision Score: 0.09
- Recall Score: 0.92
- F1 Score: 0.16

## Summary
When looking for a model to that predicts bad loans, neither of our oversampling models produced predictions that would be usable for actual use. Our Undersampling model produced similar results, so I would not recommend this model either. Our combination sampling produced a model that with almost identical scores to our Naive Random Sampling model. None of these models should be used for predictions.

When referring to our Classifier results, lets begin with the balanced random forest classifier first. We had a precision score of 0.03, meaning our precision definitely needs to improve(3/100). It was able to detect 70% of bad loans. The F1 score of 0.06 is still extremely low. This model should not be used.

Our Easy Ensemble AdaBoost Classifier produced much better results. Our recall score of 0.92 means we detected 92% of bad scores. Yet our precision score would lead me to believe we still should not use this model. At 0.09, only 9 of 100 bad loan applications the model believed were bad, 9 were actually only bad.
