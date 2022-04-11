# Credit_Risk_Analysis

#Overview

Credit risk is very tough to predict. There are a lot of variable to factor into what makes a person a credit risk. After our work in the module, we want to take a look at how all the factors in our loan_stats csv file to help predict whether someone is low or high risk for a loan. One method that is used is creating a model and then evaluate and train the models that are created. In this particular project we are using imbalanced-learn and scikit-learn libraries to build models and evalute them using a resampling method. In the first models, we oversampled the data using randomoversampler and smote algorithms and undersampled the data with the clustercentroid algorithm. In the remaining models we used a combination approach to oversample and undersample the data using smoteenn. Finally, we compared two machine learning models called balancedrandomforestclassifier and easyensembleclassifier.

#Results

	1. Naive Random Oversampling results: Our balanced accuracy test it 65%, the precision for the high_risk has a very low positivity at 1% and the recall is 71%. The precision for the low_risk 100% and the recall is 58%.


![Naive_Random_Oversampling](https://github.com/ljohnson1212/Credit_Risk_Analysis/blob/main/Naive_Random_Oversampling.png)


	2. SMOTE oversampling results: the accuracy score is 65.9%, the precision for the high_risk loans has a low positvity at 1% and recall is 63% overall. The precision for the low_risk is 100% and the recall is 68%.


![SMOTE](https://github.com/ljohnson1212/Credit_Risk_Analysis/blob/main/SMOTE_oversampling.png)


	3.Undersampling results: balanced accuracy score is 65.9% overall, the avg precision is at 99% and the recall is 40%


![Undersampling](https://github.com/ljohnson1212/Credit_Risk_Analysis/blob/main/Undersampling.png)



	4. Combination(over and undersampling) results: balanced accuracy score is 63.6% the avg precision is 99% and the recall is 59% overall


![Combination](https://github.com/ljohnson1212/Credit_Risk_Analysis/blob/main/Combination.png)


	5. Balanced Random Forest Classifier results: the accuracy score is 77.7% the avg precision is 99% and the recall is 89%


![Balanced_Random_Forest_Classifier](https://github.com/ljohnson1212/Credit_Risk_Analysis/blob/main/Balanced_Random_Forest_Classifier.png)


	6. Easy Ensemble AdaBoost Classifier results: the accuracy score is 91.8% the precision is 99% and the recall is 94%


![Easy_Assemble_Adaboost_Classifier](https://github.com/ljohnson1212/Credit_Risk_Analysis/blob/main/Easy_Ensemble_Adaboost_Classifier.png)



#Summary

In the beginning of our project we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The last two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score and recall is not as high as the ensemble classifiers. In your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers. The results show us that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.