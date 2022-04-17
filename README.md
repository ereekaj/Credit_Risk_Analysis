# Credit_Risk_Analysis

## Overview of the analysis: 

The purpose of this project is to employ different maching learning techniques to train and evaluate models with unbalanced classes. Using the credit card credit dataset from LendingClub, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, I used a combo approach of over- and undersampling using the SMOTEENN algorithm. Lastly, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results: 
* **Naive Random Oversampling results**: The balanced accuracy test it 64%, the precision for the high_risk has a very at 1% and the recall is 66%.

![aive Random Oversampling screenshot](https://github.com/ereekaj/Credit_Risk_Analysis/blob/main/Resources/NativeRandomOversampler.png)

* **SMOTE oversampling results**: The accuracy score is 65%, the precision for the high_risk loans has a low positvity again at 1% and recall is 61%.

![SMOTE oversampling screenshot](https://github.com/ereekaj/Credit_Risk_Analysis/blob/main/Resources/SmoteOversampling.png)

* **Undersampling results**: The accuracy score is 65%, the precision for high_risk is is at 1% and the recall is 69%.

![Undersampling results screenshot](https://github.com/ereekaj/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroidsResampler.png)

* **SMOTEENN (over and undersampling) results**: The balanced accuracy score is 54.5% the high_risk precision is 1% and the recall is 72%.

![SMOTEENN screenshot](https://github.com/ereekaj/Credit_Risk_Analysis/blob/main/Resources/SmoteennCombo.png)

* **Balanced Random Forest Classifier results**: The accuracy score is 76% the precision is 3% and the recall is 64%.

![balanced Random Forest Classifier screensho](https://github.com/ereekaj/Credit_Risk_Analysis/blob/main/Resources/BalancedRandomForestClassifier.png)

* **Easy Ensemble Classifier results**: The accuracy score is 93.7% the precision is 9% and the recall is 92%.

![Easy Ensemble Classifier screenshot](https://github.com/ereekaj/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier.png)

## Summary: 

In the first four models I undersampled, oversampled and did a combination of both to determine which model is best at predicting high risk loans. In the next two models I resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In the first four models the accuracy score is not as high as the ensemble classifiers and the precision and recall in the oversampling/undersampling/mixed models is low as well. I was looking for a good balance of recall and precision in the models; therefore, I recommend the ensemble classifiers over the first four models. As you can see from the screenshots, the Easy Ensemble Classifier had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
