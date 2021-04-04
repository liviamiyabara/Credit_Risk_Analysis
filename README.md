# Credit_Risk_Analysis
 Module 17: Supervised Machine Learning and Credit Risk

 ## Overview
 In this week's challenge, the student helps Jill and LendingClub, a peer-to-peer lending services company to perform an analysis and create a prediction model to determine if it can be used to predict credit risk.

 The data set contains information about the loan amount, interest rate, installment, home ownership situation, annual income, verification status of the information, issue date of the loan and others. Since this credit risk infomration is an unbalanced classification problem, one class is much larger than the other class, the student needs to use different techniques of oversampling and/or undersampling before creating the model to predict credit risk. 

 [Link to Resampling code](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)

 [Link to Ensemble code](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)


 ## Results
Different algorithms were used to oversample and undersample the data to create the prediction model, below you can find the results of each method.

* **Naive Random Oversampling**

    Accuracy score of 65%. 

    The high_risk precision is 1%, 69% recall which makes, F1 of 2% only.
    The low_risk precision is 100%, 61% recall.

    ![ScreenShot](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/Resources/Naive_Random_Oversampling.JPG)

* **SMOTE Oversampling**

    Accuracy score of 66%. 

    The high_risk precision is 1%, 63% recall, F1 of 2% only.
    The low_risk precision is 100%, 69% recall, 82% F1.

    ![ScreenShot](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/Resources/SMOTE_Oversampling.JPG)

* **Cluster Centroids Undersampling**

    Accuracy score of 66%. 

    The high_risk precision is 1%, 69% recall, F1 of 1% only.
    The low_risk precision is 100%, 40% recall, 57% F1.

    ![ScreenShot](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/Resources/Cluster_Centroids_Undersampling.JPG)

* **Combination (Over and Under) Sampling**

    Accuracy score of 54%. 

    The high_risk precision is 1%, 72% recall, F1 of 2% only.
    The low_risk precision is 100%, 57% recall, 72% F1.

    ![ScreenShot](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/Resources/Combination_Under_Over_Sampling.JPG)

* **Balanced Random Forest Classifier**

    Accuracy score of 78%. 

    The high_risk precision is 1%, 72% recall, F1 of 2% only.
    The low_risk precision is 100%, 57% recall, 72% F1.

    ![ScreenShot](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/Resources/Balance_random.JPG)

* **Easy Ensemble AdaBoost Classifier**

    Accuracy score of 93%. 

    The high_risk precision is 9%, 92% recall, F1 of 16% only.
    The low_risk precision is 100%, 94% recall, 97% F1.

    ![ScreenShot](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/Resources/Easy_Ensemble_AdaBoost_Classifier.JPG)

 ## Summary

We used different techniques for oversampling, undersampling and a combination of both to create models to predict the credit risk. Since the analysis should focus on predicting the high credit risk properly, the percentage of positive predictions that are correct are more important than the percentage of actual positive results that are predicted correctly, so precision is more important over recall.  

For all the six methods presented in the results, precision is low for the minority class ('high_risk'), it varies from 1% to 9%. A low precision is indicative of a large number of false positives, in this case people with high credit risk that would be categorized as low risk. F1 score for high_risk is also low for all the six algorithms. 

Based on the results, none of the models would be a good representation of the credit analysis and the recommendation is for LendingClub to not use any of them.
