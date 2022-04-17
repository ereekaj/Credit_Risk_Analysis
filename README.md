# Credit_Risk_Analysis

## Overview of the analysis: 

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

In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. In the next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the precision and recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble Classifier had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
