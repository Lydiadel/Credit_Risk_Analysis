# Credit Risk Analysis

## Author
Lydia Delgado Uriarte

## Overview
Evaluate machine learning models or algorithms to predict credit risk.

## Results

### Balanced Random Forest Classifier
- Balanced accuracy score: 0.7877 -> **79%** 

- Sensitivity/recall: **0.67** A low recall is indicative of a large number of false negatives.

#### Confusion Matrix 
<img width="742" alt="Captura de Pantalla 2022-07-10 a la(s) 21 47 43" src="https://user-images.githubusercontent.com/71950779/178179499-15021c3c-9b45-464e-89fb-75719113cb4b.png">

- Out of 87 actual high risk , 58 were predicted to be high risked, which we call true positives.

- Out of 87 actual high risk, 29 were predicted to be low risk, which are considered false negatives.

#### Imbalanced classification report
<img width="665" alt="Captura de Pantalla 2022-07-07 a la(s) 23 10 41" src="https://user-images.githubusercontent.com/71950779/177921303-41987cd3-b7e1-4b81-950c-6a6cbb70b6c5.png">


### Easy Ensemble AdaBoost Classifier
- Balanced accuracy score: 0.9254 -> **93**

- Sensitivity/recall : **0.91** Highest recall of all, meaning high prediction can be likely true negatives.

#### Confusion Matrix 
<img width="742" alt="Captura de Pantalla 2022-07-10 a la(s) 21 48 58" src="https://user-images.githubusercontent.com/71950779/178179623-f13cdebd-de4f-408b-ab9b-37303bd8a327.png">

- Out of 87 Actual High risk  79 were predicted to be high risked, which we call true positives.

- Out of 87 Actual High risk, 8 were predicted to be low risk, which are considered false negatives.

#### Imbalanced classification report
<img width="662" alt="Captura de Pantalla 2022-07-07 a la(s) 23 10 20" src="https://user-images.githubusercontent.com/71950779/177921268-66216fe5-15ed-459b-aeae-3a1fd797288a.png">


### Naive Random Oversampling
- Balanced accuracy score: 0.6533 -> **65%**

- Sensitivity/recall : **0.61** 
A low recall is indicative of a large number of false negatives.

#### Confusion Matrix 
<img width="743" alt="Captura de Pantalla 2022-07-10 a la(s) 21 45 47" src="https://user-images.githubusercontent.com/71950779/178179346-bb9795c6-82da-4892-acd6-82ad2e98836e.png">

- Out of 87 actual high risk , 53 were predicted to be high risked, which we call true positives.

- Out of 87 actual high risk, 34 were predicted to be low risk, which are considered false negatives.

#### Imbalanced classification report
<img width="669" alt="Captura de Pantalla 2022-07-07 a la(s) 23 08 27" src="https://user-images.githubusercontent.com/71950779/177921106-c8426b67-147b-4ce4-9c1c-3b0dde723bd9.png">

### SMOTE Oversampling
- Balanced accuracy score: 0.6512 -> **65%**

- Sensitivity/recall : **0.62** A low recall is indicative of a large number of false negatives.

#### Confusion Matrix 
<img width="743" alt="Captura de Pantalla 2022-07-10 a la(s) 21 28 52" src="https://user-images.githubusercontent.com/71950779/178177552-f0a04658-9105-4d77-aad7-eccee5a24094.png">

- Out of 87 actual high risk , 54 were predicted to be high risked, which we call true positives.

- Out of 87 actual high risk, 33 were predicted to be low risk, which are considered false negatives.

#### Imbalanced classification report
<img width="672" alt="Captura de Pantalla 2022-07-07 a la(s) 23 06 29" src="https://user-images.githubusercontent.com/71950779/177920907-c4d6e8ce-68c3-4c63-91a4-9843807d1f64.png">

### Undersampling ClusterCentroids
- Balanced accuracy score: 0.5103 -> **51 %**

- Sensitivity/recall : **0.64** A low recall is indicative of a large number of false negatives.

#### Confusion Matrix 
<img width="742" alt="Captura de Pantalla 2022-07-10 a la(s) 21 29 38" src="https://user-images.githubusercontent.com/71950779/178177637-101f7a25-4d1e-4fc2-8eee-ad375b072add.png">

- Out of 87 actual high risk , 56 were predicted to be high risked, which we call true positives.

- Out of 87 actual high risk, 31 were predicted to be low risk, which are considered false negatives.

#### Imbalanced classification report
<img width="669" alt="Captura de Pantalla 2022-07-07 a la(s) 23 06 56" src="https://user-images.githubusercontent.com/71950779/177920964-46136335-d443-4783-a84d-dac85d67d0e9.png">


### Combination (Over and Under) Sampling SMOTEENN
- Balanced accuracy score: 0.6375 -> **64 %** 

- Sensitivity/recall : **0.70** 

#### Confusion Matrix 
<img width="740" alt="Captura de Pantalla 2022-07-10 a la(s) 21 30 38" src="https://user-images.githubusercontent.com/71950779/178177757-ea033730-ef1d-48b5-888a-ea8c06b5202e.png">

- Out of 87 actual high risk , 61 were predicted to be high risked, which we call true positives.

- Out of 87 actual high risk, 26 were predicted to be low risk, which are considered false negatives.

#### Imbalanced classification report
<img width="666" alt="Captura de Pantalla 2022-07-07 a la(s) 23 07 58" src="https://user-images.githubusercontent.com/71950779/177921060-1ced4f15-4601-4cb2-ba61-9f40dd968469.png">



## Summary
The majority of the models has between the range of 50% - 80% accuracy and the sensivity too. In this case is to take in consideration the sensitivity of each models.

### Recommended Model 
 The best model is the **Easy Ensemble AdaBoost Classifier** due the sensivity and acccuracy is also important to predictions. It’s more important to detect potentially fraudulent transactions, high sensitivity means that among people who actually have credit risk, most of them will be correct and the problem would be treated right away.
