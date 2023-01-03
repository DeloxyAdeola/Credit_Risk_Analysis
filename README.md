# Credit_Risk_Analysis
The purpose of this project is to use machine learning using different algorithm like , SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, EasyEnsembleClassifier, RandomOverSampler to predict credit risk. Since Credit risk is a deep_rooted inbalanced classification problems reason we needed to employ different techniques to train and evaluate models with unbalanced classes. The data used is from LendingClub, a peer-to-peer lending services company. 

**Balanced Random Forest Classifier**
The calculated accuracy score is 78%
low_risk     68470
high_risk      347

By features of impotrance the 
total_rec_prncp and total_payment are the lead factors to consider for our analysis.
FIGS

 [alt text](image_url)
 
**Easy Ensemble AdaBoost Classifier**
The balanced accuracy score is 93%
The precision for high risk is 9%
The precision for low risk is 100%
The recall for high risk is 92%
The recall for low risk is 94%

**SMOTE Oversampling**
The balanced accuracy score is 62.1%
The precision for high risk is 1%
The recall for high risk is 54%
The precision for low risk is 100%
The recall for low risk is 70%

**Undersampling: Cluster Centroids**
he balanced accuracy score is 50.6%
The precision for high risk is 0%
The recall for high risk is 48%
The precision for low risk is 100%
The recall for low risk is 53%

**Combination Sampling SMOTEENN**
The balanced accuracy score is 62.7%
The precision for high risk is 1%
The recall for high risk is 63%
The precision for low risk is 100%
The recall for low risk is 62%
Balanced Random Forest Classifier


Summary
In summary, most of the machine learning models do not preform particularly well. All 6 of the models had a precision rate of 100% for low risk, as precision is a measure of how reliable a positive classification is, this means that the models were able to correctly predict low risk 100% of the time. However, for this data this statistic is irrelevant. As the data is extremely imbalanced, with about 0.5% of the data being high risk, even if a model predicted all high risk as low risk, the precision rate would still be 100%.The easy ensemble AdaBoost classifier had a high risk recall rate of 92%, a low risk recall rate of 94% and a high risk precision rate of 9%. With a balanced accuracy score of 93.2%, this model is the best of the 6 models. With a balanced accuracy score of 93.2%, this is the best model of the 6 models. While other models not explored here may have a higher precision rate for high risk, of the 6 models here, this can be recommended as the best model to use.
Both of the oversampling models had recall rates from between 54%-70% and only 1% precision rate for high risk. Both of their balanced accuracy scores were around 62%. While this accuracy score is not particularly good, their precision rate for high risk also disqualifies them as usable models.
The undersampling model using cluster centroids had a high risk recall rate of 48%, a low risk recall rate of 53% and a high risk precision rate of 0%. With  accuracy score of 50.6%, which to me is not useful. The final resampling model, SMOTEENN, which is a combination of over and under sampling, had a high risk recall rate of 63%, a low risk recall rate of 62% and a high risk precision rate of 1%. With a balanced accuracy score of 62.7%, this model is also not usable.Finally, both ensemble models had a significant improvement over the resampling models. While both precision rates for low risk were still 100%, the balanced random forest classifier had a high risk recall rate of 70%, a low risk recall rate of 87% and a high risk precision rate of 3%. With a balanced accuracy score of 78.8%, this model is much better than others.


