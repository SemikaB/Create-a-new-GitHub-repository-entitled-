# Credit_Risk_Analysis
### Overview 

 In this project we analysed at how all the factors in our loan_stats csv helped to predict if someone is high or low risk status. One method used use for this type of issue is creating a model and then evaluate and train the models created. In this specific project we are using imbalanced-learn and scikit-learn libraries to build models and evalute them using a resampling method. In the first couple of models I oversampled the data using randomoversampler and smote algorithms and undersample the data with the clustercentroid algorithm. In the remaining models a combination approach to over and undersample the data using smoteenn. Finally, a comparison of two machine learning models that minimize bias was preformed, balancedrandomforestclassifier and easyensembleclassifier.
 
 ### Results
 
 In Naive Random Oversampling it shows hat our balanced accuracy test equals 67%, and the precision for the high_risk has a very low positivity at 1% and the recall equals 74%
 
 <img width="1382" alt="ima1" src="https://user-images.githubusercontent.com/100738128/176954962-823825a3-7fd4-46d4-9787-99e25f09c602.png">

SMOTE oversampling results: the accuracy score is 66.2%, the precision for the high_risk loans has a low positvit

<img width="1286" alt="ima2" src="https://user-images.githubusercontent.com/100738128/176955018-05255c87-7cd4-4eea-9068-1fb93061fdbc.png">

Undersampling results: balanced accuracy score is 66.2% overall, the precision is at 99% and the recall is 41%

Combination(over and undersampling) quals; balanced accuracy score is 54.7% the precision is 99% and the recall is 57% overall

<img width="1355" alt="ima4" src="https://user-images.githubusercontent.com/100738128/176955135-438dc993-f6e2-4d19-a075-0990ee21a7ae.png">


Balanced Random Forest Classifier equals; the accuracy score is 77.2% the precision is 99% and the recall is 88%

<img width="1293" alt="ima5" src="https://user-images.githubusercontent.com/100738128/176955174-911352bf-558a-4412-a003-d05488e82063.png">

Easy Ensemble AdaBoost Classifier results equals; accuracy score is 91.7% the precision is 99% and the recall is 94%

<img width="1353" alt="ima6" src="https://user-images.githubusercontent.com/100738128/176955208-abd1815e-0f37-4849-9d43-55ea4a2a88c8.png">

### Summary

In this module the first four models we undersampled, oversampled and a combination of both was done in an attempt to determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
