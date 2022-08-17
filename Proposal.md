# Project Proposal: Credit Card Fraud Detection

### By Ramy Gendy

This project challenge one of the most popular and widely used datasets in anomaly dectection. Anomaly detection problems can be solved using different models and techniques. Following are details of this project including all information needed to get started.

![Screenshot](https://storage.googleapis.com/kaggle-datasets-images/310/684/3503c6c827ca269cc00ffa66f2a9c207/dataset-cover.jpg)

## Introduction

It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. I will use various predictive models to see how accurate they are in detecting whether a transaction is a normal payment or a fraud.

Please note in the dataset, the features are scaled and the names of the features are not shown due to privacy reasons.

## Dataset

* Download directly from [here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/download?datasetVersionNumber=3).
* Source: [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?datasetId=310).

## Content

* The dataset contains transactions made by credit cards in September 2013 by European cardholders.

* This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

* It contains only numerical input variables which are the result of a PCA transformation.

* Given the class imbalance ratio, it is recommended measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC).

```
Non Frauds 99.83 % of the dataset
Frauds 0.17 % of the dataset
```
  
* Confusion matrix accuracy is not meaningful for unbalanced classification.

* A simulator for transaction data has been released as part of the [practical handbook on Machine Learning for Credit Card Fraud Detection](https://fraud-detection-handbook.github.io/fraud-detection-handbook/Chapter_3_GettingStarted/SimulatedDataset.html).

* More details on current and past projects on related topics are available [here](https://www.researchgate.net/project/Fraud-detection-5) and the page of the DefeatFraud project.

### Columns

1. As mentioned, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'.

2. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset.

3. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning.
  
4. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

## Approach

* Understand the distribution of of our dataset by applying EDA and feture engineering.
* Create a balanced dataframe of "Fraud" and "Non-Fraud" transactions.
* Decide which Classifiers we are going to use and decide which one has a higher accuracy.
* Create a pipleine to test and compare the accuracy to our best classifier.
* Understand common mistaked made with imbalanced datasets.

### Exploratory Data Analysis

1. Start by business and data understanding.
2. Using `df.info()` check the datatype of columns.
3. Check for duplicates in your data and remove it.
4. Check for missing values
5. Apply univariate analysis and repeat it to check for errors if needed.
6. Clean the data by fixing the errors using apply function and try except.
7. Check for expected data imbalance.
8. Apply possible feature engineering.
9. Detect outliers and split df to outliers and clean then analyze outliers df.
10. Finally start answering the proposed questions and understand it very well then using the table answer those questions or apply full analysis.

### Machine Learning Process

1. Encode the categorical data with the appropriate technique.
2. Split the data into train and test.
3. Feature scaling.
4. Dealing with imbalanced classess.
