# Credit_Risk_Analysis

## Overview

The purpose of this analysis was to use different methods of supervised machine learning to predict credit risk. Here, I used logistic regression and and random forest classifiers to predict credit risk. Because the dataset is unbalanced, leaning more towards low risk, I employed different techniques to balance the dataset in an effort to determine which model is best for predicting credit risk.

## Results

The results of the 6 models generated in this analysis are: 

1. Naive Random Oversampling and Logistic Regression - The accuracy score was 64.99%. The precision for high risk credit was a low 1% while the recall was 62%.
2. SMOTE Oversampling and Logistic Regression - The accuracy score was 63.80%. The precision was 1% while recall was 67%. 
3. Undersampling and Logistic Regression - The accuracy was 39.49%. The precision was 1% and the call was 67%. 
4. Oversampling and Undersampling using SMOTEENN and Logistic Regression - The accuracy was 55.09%. The precision was 1% while the recall was 69%. 
5. Balanced Random Forest Classifier - The accuracy was 90.08%. The precision was 3% while the recall was 60%. 
6. Easy Ensemble AdaBoost Classifier - The accuracy was 92.72%. The precision was 6% while the recall was 89%. 

## Summary

After running all 6 models, it seems as though using Logistic Regression with oversampling, undersampling, or both is not great at predicting credit risk. Here, the accuracy was low, around 60% each time. In addition, there wasn't a good balance between the precision and recall. With the Random Forest classifiers, the accuracy was much higher, at around 90%. In addition, the precision was higher and there was a better balance between precision and recall.

After running all of the models, I'd recommend using the Easy Ensemble AdaBoost Classifier. The accuracy was highest here at 92.72%. In addition, the precision was highest at 6% and there was high sensitivity/ recall. This is exemplified further by the f1 score at 0.11 for high risk and 0.96 for low risk, which are the highest scores among all 6 models. 