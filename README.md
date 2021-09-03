
# Credit_Risk_Analysis

## Overview of the analysis:
Using machine learning to solve the question of credit card risk, I used unbalanced classification models (unbalanced because good loans easily outnumber risky loans). Using two libraries, imalanced-learn and scikit-learn I built and evaluated models using resampling. 

The data set was the credit card credit dataset from LendingClub, a peer-to-peer lending services company. I oversampled the data with RandomOver Sampler and SMOTE algorithms, underssampled using ClusterCentroids, and used a combination of over- and undersampling using the SMOTEENN algorithm, then compared two machine learning models that reduce bias; BalancedRandomForestClassifier and EasyEnsembleClassifier. 

## Results: 


<img width="1027" alt="Screen Shot 2021-09-03 at 2 32 21 PM" src="https://user-images.githubusercontent.com/14239715/132051532-b81921fd-cc0d-45d1-aa74-f7da1bce4c7f.png">

<img width="971" alt="Screen Shot 2021-09-03 at 2 32 27 PM" src="https://user-images.githubusercontent.com/14239715/132051546-c247280b-119d-4145-b6f6-34a5806b376d.png">

<img width="975" alt="Screen Shot 2021-09-03 at 2 32 34 PM" src="https://user-images.githubusercontent.com/14239715/132051564-c6e7392d-89a8-4307-84f6-e462c6f9ffe1.png">

<img width="902" alt="Screen Shot 2021-09-03 at 2 32 41 PM" src="https://user-images.githubusercontent.com/14239715/132051575-047e3dc5-2742-4503-9370-b6d1b2b79586.png">

<img width="1109" alt="Screen Shot 2021-09-03 at 4 02 10 PM" src="https://user-images.githubusercontent.com/14239715/132060301-36d92476-7fe2-4020-8244-97125049a20d.png">

<img width="1121" alt="Screen Shot 2021-09-03 at 4 02 24 PM" src="https://user-images.githubusercontent.com/14239715/132060342-83a0ddaf-0114-41db-8870-8326f76fc25e.png">


<img width="1133" alt="Screen Shot 2021-09-03 at 4 02 34 PM" src="https://user-images.githubusercontent.com/14239715/132060349-1fa66dbb-ded2-4222-a75e-9f714f6db9cf.png">



## Summary and Result discussion: 

• The precision score of all of the these models are excelent at predicting low risk credit candidates and terrible at predicting high risk candidates as made evident by the 'pre' score of ~0.01 for high risk and ~.99 score for low risk and a high F1 score for low risk candidates.  

• The sensitivity was far more balanced, the two oversampling methods averageing out at around .60 vs the undersampling at .40. 

Perhaps predicting low risk credit candidates is enough as this system is relativlely binary, making it suitable for the regression testing above. You're either a low risk candidate or you're not. 
