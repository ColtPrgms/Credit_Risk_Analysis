# Credit_Risk_Analysis
### **Challenge #17**
#### by Colt Korth

&nbsp;

## **Project Overview**
The goal is to build a Machine Learning Model to accurately predit credit risk based on the provided dataset. 

&nbsp;

## **Results**
+ **Naive Random Oversampling**
  - _Balanced Accuracy Score:_ 0.6649811101424005
  - _Precision Score:_
    - High Risk: 0.01
    - Low Risk: 1.00
  - _Recall Score:_
    - High Risk: 0.63
    - Low Risk: 0.67

&nbsp;

+ **SMOTE Oversampling**
  - _Balanced Accuracy Score:_ 0.6442986007872334
  - _Precision Score:_
    - High Risk: 0.01
    - Low Risk: 1.00
  - _Recall Score:_
    - High Risk: 0.61
    - Low Risk: 0.68

&nbsp;

+ **Cluster Centroids Resampler**
  - _Balanced Accuracy Score:_ 0.5227085020406026 
  - _Precision Score:_
    - High Risk: 0.01
    - Low Risk: 1.00
  - _Recall Score:_
    - High Risk: 0.60
    - Low Risk: 0.45

&nbsp;

+ **SMOTEENN Sampling**
  - _Balanced Accuracy Score:_ 0.647506556921329
  - _Precision Score:_
    - High Risk: 0.01
    - Low Risk: 1.00
  - _Recall Score:_
    - High Risk: 0.71
    - Low Risk: 0.58

&nbsp;

+ **Random Forest Classifier**
  - _Balanced Accuracy Score:_ 0.7926392645111097
  - _Precision Score:_
    - High Risk: 0.03
    - Low Risk: 1.00
  - _Recall Score:_
    - High Risk: 0.70
    - Low Risk: 0.88

&nbsp;

+ **Easy Ensemble Classifier**
  - _Balanced Accuracy Score:_ 0.9316600714093861
  - _Precision Score:_
    - High Risk: 0.09
    - Low Risk: 1.00
  - _Recall Score:_
    - High Risk: 0.92
    - Low Risk: 0.94

&nbsp;

## **Analysis**
The purpose of our model is to predict credit risk with accuracy. when comparing the six models together, the focus will be on Balanced Accuracy Score. That said "Native Random Oversampling", "SMOTE Oversampling", "Cluster Centroids Resampler", and "SMOTEENN Sampling" all have a Balanced Accuracy Score of less than 68%. This implies each of these can predict credit risk only slightly better than flipping a coin. Each of these does not suit our needs. Random Forest Classifier had a Balanced Accuracy Score of 79%. This is much better than the previous 4 models. It even had slightly better Precision and Recall Scores as well. The Easy Ensemble Classifier had a Balanced Accuracy Score of 93%! This is a highly accurate model which is recommended for use. The precision score is only 9%, which implies that the model mostly predicts a low risk status. This can be fixed in the future by having more high risk data entered into the training for the model. 
