# Credit_Risk_Analysis

## Overview:

Using the credit card dataset from LendingClub ,we will predict the credit risk employing different techniques like imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

We’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, 

## Results: 

### Oversampling
![image](https://user-images.githubusercontent.com/120151872/233814396-02aaaf4f-394a-43f8-b14e-22408194a636.png)

- Balanced accuracy score : 0.60
- Precision : 0.01 for high_risk and 1.00 for low_risk
- Recall score : 0.71 for high_risk and 0.60 for low_risk
- f1 score : 0.02 for high_risk and 0.75 for low_risk

The low precision and F1 scores for high_risk category means this model is not appropiate to predict high_risk credit assessment.

### SMOTE Oversampling
![image](https://user-images.githubusercontent.com/120151872/233814420-bea66118-11c4-464a-a325-00b56fcac6b2.png)

- Balanced accuracy score : 0.66
- Precision : 0.01 for high_risk and 1.00 for low_risk
- Recall score : 0.63 for high_risk and 0.69 for low_risk
- F1 score : 0.02 for high_risk and 0.82 for low_risk

From the low precision and F1 scores for high_risk category, it can be concluded that this model is not good to predict high_risk credit assessment.

### Undersampling 
![image](https://user-images.githubusercontent.com/120151872/233814444-7d1c962e-540f-45f0-98f7-49ca7ed06a8b.png)
- Balanced accuracy score : 0.66
- Precision : 0.01 for high_risk and 1.00 for low_risk
- Recall score : 0.69 for high_risk and 0.40 for low_risk
- F1 score : 0.01 for high_risk and 0.57 for low_risk

From the low precision and F1 scores for high_risk category, it can be concluded that this model is not good to predict high_risk credit assessment.

### Combination (Over and Under) Sampling
![image](https://user-images.githubusercontent.com/120151872/233814467-4e1c588e-cb45-49f6-a362-3b4ee6a7c80e.png)

- Balanced accuracy score : 0.54
- Precision : 0.01 for high_risk and 1.00 for low_risk
- Recall score : 0.72 for high_risk and 0.57 for low_risk
- F1 score : 0.02 for high_risk and 0.72 for low_risk

From the low precision and F1 scores for high_risk category, it can be concluded that this model is not good to predict high_risk credit assessment.

### Balanced Random Forest Classifier
![image](https://user-images.githubusercontent.com/120151872/233814301-5745d9ed-4d0e-4938-84c2-11c1f4db1b38.png)

- Balanced accuracy score : 0.79
- Precision : 0.03 for high_risk and 1.00 for low_risk
- Recall score : 0.70 for high_risk and 0.88 for low_risk
- F1 score : 0.06 for high_risk and 0.93 for low_risk

From the low precision and F1 scores for high_risk category, it can be concluded that this model is not good to predict high_risk credit assessment.

### Easy Ensemble AdaBoost Classifier
![image](https://user-images.githubusercontent.com/120151872/233814332-20bea31e-9bda-4601-a972-7117b9e8e216.png)


- Balanced accuracy score : 0.93
- Precision : 0.03 for high_risk and 1.00 for low_risk
- Recall score : 0.92 for high_risk and 0.94 for low_risk
- F1 score : 0.16 for high_risk and 0.97 for low_risk
 
The accuracy score is the higher (0.93) between all the models performed and with the other parameters we can say  this model is appropiate to predict high_risk credit assessment.

## Summary
Looking at all the results in the 6 models, it can be concluded that the Easy Ensemble AdaBoost Classifier is the best to predict high risk credit assessments. Although the F1 score is low, the accuracy score is 0.93 which indicates that this model can correctly categorize the risk at 93%. The precision is low (0.03) but the recall 0.92 which is the highest result. So, this model is the winner for the high accuracy score and good balance of precision and recall scores.
