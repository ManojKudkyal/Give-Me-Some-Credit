# Give Me Some Credit 

## Description
Banks play a crucial role in market economies. They decide who can get finance and on what terms and can make or break investment decisions. For markets and society to function, individuals and companies need access to credit. 

Credit scoring algorithms, which make a guess at the probability of default, are the method banks use to determine whether or not a loan should be granted. This project aims to improve on the state of the art in credit scoring, by predicting the probability that somebody will experience financial distress in the next two years.


## Steps taken
1. Loading and exploring the data.
2. Dealing with null values.
3. Exploratory Data Analysis(EDA).
4. Removing the data imbalance.
5. Feature selection.
6. Build logistic regression model both on the imbalnced and balanced datasets.

## Outputs

### 1. For imbalanced dataset
              precision    recall  f1-score   support

           0       0.93      1.00      0.97     41970
           1       0.51      0.01      0.02      3030

    accuracy                           0.93     45000
    macro avg       0.72      0.51      0.49     45000
    weighted avg       0.90      0.93      0.90     45000



### 2. For balanced dataset
              precision    recall  f1-score   support

           0       0.67      0.89      0.76      2891
           1       0.85      0.59      0.70      3056

    accuracy                           0.73      5947
    macro avg       0.76      0.74      0.73      5947
    weighted avg       0.76      0.73      0.73      5947



