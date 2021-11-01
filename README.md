# Credit_Risk_Analysis



## Overview
The purpose of this analysis was to employ multiple machine learning algorithms to assess credit risk in a dataset of loan applicants from LendingClub, a peer-to-peer lending services. The applicants' data would then render them 'high-risk' or 'low risk' credit. Algorithmic performance was analyzed by the accuracy score, precision, and recall seen in the imbalanced classification reports and confusion. 




## Machine Learning Models ##


### * Naive Random Oversampling
### * SMOTE Oversampling
### * ClusterCentroids Undersampling
### * SMOTEENN Combination Sampling
### * Balanced Random Forest Classifier
### * Easy Ensemble AdaBoost Classifier




# Results


## * Naive Random Oversampling (NRS)
   ![image](https://user-images.githubusercontent.com/86337475/139560546-a0a225ab-3657-4de5-8225-e2b7359f8344.png)
 
   ![image](https://user-images.githubusercontent.com/86337475/139560574-544b2031-03f6-4807-89fa-2f16c337d4e7.png)

The accuracy score of NRS was found to be 65%. Precision was very poor at 0.01, however recall was relatively strong at 73%, suggesting that this model is sensitive to high-risk credit and retreives a large fraction of relevant instances (High-risk credit score in this analysis). With precision so low, there will  be a significant amount of false positives, or users labeled as 'high-risk'. In the case of LendingClub, a peer-to-peer lending company, this could potentially be an acceptable model to use for individuals who are less concerned with precision and accuracy, and more concerned with recall of high-risk credit scores to avoid. 




### * SMOTE Oversampling
![image](https://user-images.githubusercontent.com/86337475/139560998-321417f5-316d-42e1-8d19-bf946196c6d2.png)


![image](https://user-images.githubusercontent.com/86337475/139561004-db4edb41-345f-4f00-b012-2780ec992035.png)
 
 
 Although they have practically the same accuracy score (65-66%), SMOTE performed worse than NRS on predicting this dataset with a lower recall of 63%, compared to NRS with 73%. Therefore we cannot recommend SMOTE above NRS.


### * ClusterCentroids Undersampling


![image](https://user-images.githubusercontent.com/86337475/139561424-90a77204-3103-442e-a8b9-3e86544f3d64.png)

Undersampling with ClusterCentroids retreived nearly random 54% accuracy, and very low (1%) precision, but recall was second highest so far at 69%, so it will retrieve a relatively strong number of true target values and could provide users 


### * SMOTEENN Combination Sampling

![image](https://user-images.githubusercontent.com/86337475/139561776-229eea79-d9f8-4a37-9e7b-615fe94d066c.png)
A combination of oversampling and undersampling gives SMOTEENN algorithm the best marks yet. 
66% accurate, and the highest recall rate of 78%. This is the strongest machine learning model for this dataset for the individual who is highly risk averse in a peer-to-peer lending environment. 


### * Balanced Random Forest Classifier


![image](https://user-images.githubusercontent.com/86337475/139561877-b6fac723-d240-44e3-8490-93311e5ed545.png)

The Random Forest Classifier has high precision (73%), but low recall (34%), and a good accuracy score of 67%, making this an overall good model for predicting credit risk. There is a higher risk of not retrieving all of the desired target values.


### * Easy Ensemble AdaBoost Classifier


![image](https://user-images.githubusercontent.com/86337475/139562202-11d21ac0-5431-4184-a2de-2598f30aa52c.png)

AdaBoost ensemble classifier delivered the best acurracy score (91%) as well as the highest recall (90%).  Precision was low at 6%, but in line with other models. Based on these data. we give LendingClub our recommda a lkk\
