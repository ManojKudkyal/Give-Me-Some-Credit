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

# Balancing technique used
To address the issue of class imbalance in our dataset, we utilized the 
### Synthetic Minority Over-sampling Technique (SMOTE). 

What is SMOTE? <br>
SMOTE (Synthetic Minority Over-sampling Technique) is an oversampling technique that creates synthetic examples of the minority class. Unlike simple oversampling where duplicate examples are added, SMOTE generates new instances by interpolating between existing minority class examples.

How SMOTE Works: <br>
* Select a Minority Class Sample: Choose a sample from the minority class.
* Find k Nearest Neighbors: Identify k nearest neighbors for this sample (typically k=5).
* Synthesize New Samples: For each selected sample, create new synthetic samples by interpolating between the selected sample and its neighbors.
* By using SMOTE, we aim to provide a more balanced dataset to our logistic regression model, which should help improve the model's ability to correctly classify minority class instances.

## Outputs

### 1. For imbalanced dataset
              precision    recall  f1-score   support

           0       0.94      1.00      0.97     42060
           1       0.46      0.01      0.02      2940

    accuracy                           0.93     45000
    macro avg       0.70      0.51      0.49     45000
    weighted avg       0.90      0.93      0.90     45000



### 2. For balanced dataset
              p precision    recall  f1-score   support

           0       0.63      0.89      0.74     41839
           1       0.81      0.48      0.60     42146

    accuracy                           0.68     83985
    macro avg       0.72      0.68      0.67     83985
    weighted avg       0.72      0.68      0.67     83985



