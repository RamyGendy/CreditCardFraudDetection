# Credit Card Fraud Detection
#### Ramy Gendy

This project challenge one of the most popular and widely used datasets in anomaly dectection. Anomaly detection problems can be solved using different models and techniques. Following are details of this project including all information needed to get started.

![Screenshot](https://storage.googleapis.com/kaggle-datasets-images/310/684/3503c6c827ca269cc00ffa66f2a9c207/dataset-cover.jpg)

## Introduction

It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. I will use various predictive models to see how accurate they are in detecting whether a transaction is a normal payment or a fraud.

Please note in the dataset, the features are scaled and the names of the features are not shown due to privacy reasons.

## Dataset

* [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/download?datasetVersionNumber=3)


## Content

* The dataset contains transactions made by credit cards in September 2013 by European cardholders.

* This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

* It contains only numerical input variables which are the result of a PCA transformation.

* As mentioned, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'.

* Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset.

* The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning.
  
* Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

* Given the class imbalance ratio, it is recommended measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). 
  
* Confusion matrix accuracy is not meaningful for unbalanced classification.

* A simulator for transaction data has been released as part of the [practical handbook on Machine Learning for Credit Card Fraud Detection](https://fraud-detection-handbook.github.io/fraud-detection-handbook/Chapter_3_GettingStarted/SimulatedDataset.html).

* More details on current and past projects on related topics are available [here](https://www.researchgate.net/project/Fraud-detection-5) and the page of the DefeatFraud project.

## Approach

* Understand the distribution of of our dataset.
* Create a balanced dataframe of "Fraud" and "Non-Fraud" transactions.
* Decide which Classifiers we are going to use and decide which one has a higher accuracy.
* Create a pipleine to test and compare the accuracy to our best classifier.
* Understand common mistaked made with imbalanced datasets.

## Used Language

![python](https://img.shields.io/badge/Language-python-green.svg) ![SQL](https://img.shields.io/badge/Language-SQL-blue)

## Used Libraries

* NumPy.
* Pandas.
* Sci-kit Learn.
* TensorFlow.
* Matplotlib.
* Seaborn.
* Time.
* Collections.

## Build Status

* N/A.

## Getting Started

* Clone this repository `git clone https://github.com/RamyGendy/CreditCardFraudDetection.git` into AWS Sagemaker Studio or Google Colab (or download manually on local machine).

## Author

* [Ramy Gendy](https://github.com/RamyGendy).

## Copyright & Licensing Information

* [Open Database](https://opendatacommons.org/licenses/dbcl/1-0/)