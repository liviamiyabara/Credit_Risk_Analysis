# Credit_Risk_Analysis
 Module 17: Supervised Machine Learning and Credit Risk

 ## Overview
 In this week's challenge, the student helps Jill and LendingClub, a peer-to-peer lending services company to perform an analysis and create a prediction model to determine if it can be used to predict credit risk.

 The data set contains information about the loan amount, interest rate, installment, home ownership situation, annual income, verification status of the information, issue date of the loan and others. Since this credit risk infomration is an unbalanced classification problem, one class is much larger than the other class, the student needs to use different techniques of oversampling and/or undersampling before creating the model to predict credit risk. 

 [Link to Resampling code](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)
 [Link to Ensemble code](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)


 ## Results
Different algorithms were used to oversample and undersample the data to create the prediction model, below you can find the results of each method.

* Naive Random Oversampling
    Accuracy score of 65%. 
    The high_risk precision is 1%, 69% recall which makes, F1 of 2% only.
    The low_risk precision is 100%, 61% recall.

    ![ScreenShot](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/Resources/Naive_Random_Oversampling.JPG)

* SMOTE Oversampling
    Accuracy score of 66%. 
    The high_risk precision is 1%, 63% recall, F1 of 2% only.
    The low_risk precision is 100%, 69% recall, 82% F1.

    ![ScreenShot](https://github.com/liviamiyabara/Credit_Risk_Analysis/blob/main/Resources/SMOTE_Oversampling.JPG)


 ## Summary

While precision ("pre" column) and recall ("rec" column) are high for the majority class, precision is low for the minority class.
