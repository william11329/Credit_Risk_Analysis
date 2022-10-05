# Credit_Risk_Analysis
## Analysis Overview
This project uses a Python environment to take a look at different machine learning models that can be used to predict credit risk.
These were the different methods used.
- RandomOverSampler
- SMOTE
- ClusterCentroids
- SMOTEENN
- BalancedRandomForestClassifier
- EasyEnsembleClassifier

## Results
### RandomOverSampler 
![image](https://user-images.githubusercontent.com/66809577/193964592-77637e54-bda8-499b-9aa6-407401c16e87.png)

- The balanced accuracy score is 65%.
- The high_risk precision is about 1% only with 62% sensitivity.
- Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

### SMOTE
![image](https://user-images.githubusercontent.com/66809577/193964973-077e117f-daac-409a-808a-f30fb92cd159.png)

- The balanced accuracy score is 64%.
- The high_risk precision is about 1% only with 63% sensitivity.
- Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.

### ClusterCentroids 
![image](https://user-images.githubusercontent.com/66809577/193965044-331039d6-d5ba-4798-9324-02435a7c59d2.png)

- The balanced accuracy score is about 52%.
- The high_risk precision is 1% only with 63% sensitivity.
- Due to the high number of false positives, the low_risk sensitivity is only 40%.

### SMOTEENN
![image](https://user-images.githubusercontent.com/66809577/193965139-67b69b20-b50c-4d19-9d4f-329e4a47508a.png)

- The balanced accuracy score is about 62%.
- The high_risk precision is about 1% only with 68% sensitivity.
- Due to the high number of false positives, the low_risk sensitivity is 57%.

### BalancedRandomForestClassifier
![image](https://user-images.githubusercontent.com/66809577/193965236-4f7ad453-39c5-4bfc-a2f2-1356a3d28583.png)

- The balanced accuracy score is about 79%.
- The high_risk precision is low at 4% with 67% sensitivity.
- Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

### EasyEnsembleClassifier
![image](https://user-images.githubusercontent.com/66809577/193965313-c2d8be3b-6d61-4b8d-86d5-0d03ffca175f.png)

- The balanced accuracy score is high at about 93%.
- The high_risk precision is at 7%  with 91% sensitivity.
- Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.

## Summary 
All the models used to perform the credit risk analysis seem to perform poorly. The only model I would reccomend would be the EasyEnsembleClassifier, its recall detects most high risk credit even if it falsly detects some low risk credits. Even with the false detecting I would say this model is the most accurate although there may be better options out there.
