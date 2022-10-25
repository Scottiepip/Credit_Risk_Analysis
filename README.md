# Credit_Risk_Analysis

## Overview:
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we'll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once done, we’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results:

### Navie Random Oversampling
![image](https://user-images.githubusercontent.com/108709071/197661178-1bada361-4636-440b-bf21-527b6e78dfbf.png)

![image](https://user-images.githubusercontent.com/108709071/197661273-8efdf3b9-2570-4a3c-9fbc-3c32349f88c3.png)

  - Balanced Accuracy Score: 62.5%
  - Precision Score - High Risk: 1%
  - Precision Score - Low Risk: 100%
  - Recall Score - High Risk: 60%
  - Recall Score - Low Risk: 65%

### SMOTE Oversampling
![image](https://user-images.githubusercontent.com/108709071/197661307-e83437bc-78d0-44ed-8815-dc16b3eb6924.png)

![image](https://user-images.githubusercontent.com/108709071/197661331-bdc28089-b931-4c14-be7f-a256c5ee2ad6.png)

  - Balanced Accuracy Score: 65.1%
  - Precision Score - High Risk: 1%
  - Precision Score - Low Risk: 100%
  - Recall Score - High Risk: 64%
  - Recall Score - Low Risk: 66%

### Cluster Centroids Undersampling
![image](https://user-images.githubusercontent.com/108709071/197661355-7f7f9a67-ed12-40cb-b543-efb4c22b6334.png)

![image](https://user-images.githubusercontent.com/108709071/197661383-ba7e7d5f-7e37-4a36-b1aa-b5d26df2dc5e.png)

  - Balanced Accuracy Score: 51%
  - Precision Score - High Risk: 1%
  - Precision Score - Low Risk: 100%
  - Recall Score - High Risk: 59%
  - Recall Score - Low Risk: 43%

### SMOTEENN Undersampling
![image](https://user-images.githubusercontent.com/108709071/197661481-ff2087f4-ac60-4417-abd9-295249a24fb7.png)

![image](https://user-images.githubusercontent.com/108709071/197661502-cfdbebc4-59a8-4129-8e15-32d56e343fad.png)

  - Balanced Accuracy Score: 63.8%
  - Precision Score - High Risk: 1%
  - Precision Score - Low Risk: 100%
  - Recall Score - High Risk: 70%
  - Recall Score - Low Risk: 57%


### Balanced Random Forest Classifier
![image](https://user-images.githubusercontent.com/108709071/197661530-e8e14add-45f3-42d8-a03e-b240973f5205.png)

![image](https://user-images.githubusercontent.com/108709071/197661557-3b7bcc27-b37f-44ba-99b6-abff17370e3e.png)

  - Balanced Accuracy Score: 78.8%
  - Precision Score - High Risk: 4%
  - Precision Score - Low Risk: 100%
  - Recall Score - High Risk: 67%
  - Recall Score - Low Risk: 91%

### Easy Ensemble AdaBoost Classifier
![image](https://user-images.githubusercontent.com/108709071/197661577-5bb83715-3bfc-40b5-867f-c8be7c4fbdbc.png)

![image](https://user-images.githubusercontent.com/108709071/197661597-28b78234-f855-4372-bb9d-f386dff23f83.png)

  - Balanced Accuracy Score: 92.5%
  - Precision Score - High Risk: 7%
  - Precision Score - Low Risk: 100%
  - Recall Score - High Risk: 91%
  - Recall Score - Low Risk: 94%

## Summary:
According to the results above, the Easy Ensemble AdaBoost Classifier model has the hightest balanced accuracy score of 92.5% and also the highest recall score on both High Risk and Low Risk of 91% and 94%.

Therefore, the Easy Ensemble AdaBoost Classifier model is recommanded to be used to predict Credit Risk.
