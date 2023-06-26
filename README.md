# Airline-passenger-referal-prediction

## Problem Statement
Data includes airline reviews from 2006 to 2019 for popular airlines around the world with multiple-choice and free-text questions. Data is scraped in Spring 2019. The main objective is to predict whether passengers will refer the airline to their friends.

### Dataset Variables

airline: Name of the airline

overall: Overall point is given to the trip between 1 to 10

author: Author of the trip #reviewdate: Date of the Review customer.

review: Review of the customers in free text format.

aircraft: Type of the aircraft.

Traveller type: Type of traveller (e.g. business, leisure)

cabin: Cabin at the flight.

date flown: Flight date

seat comfort: Rated between 1-5

cabin service: Rated between 1-5.

foodbev: Rated between 1-5

entertainment: Rated between 1-5

ground service: Rated between 1-5 value for money: Rated between 1-5.

recommended: Binary, target variable.

## Summary

The airline passenger referral prediction dataset consists of various categorical and numerical columns. The dataset consists of a total of 17  columns such as airline, overall, author, review_ date, customer_review, aircraft, traveller_type, recommended etc.
I followed step-by-step processes for the project like data collection, data cleaning, EDA, Visualization, Model Training and Testing, Hyperparameter Tuning, and Evaluation. 
In EDA I started by checking the head of the dataset, it contains various categorical and numerical columns. I dropped some categorical features which are irrelevant with respect to  the target variable “recommended”. Further, I check unique values and duplicate values in the dataset. Later I count the duplicate values and drop them. I also worked on  NAN values, I count and dropped them. Later I remove all NAN values from the target variable.
I used  KNN imputer for the imputation of missing values. KNNimputer is a sci-kit learn class that is used to fill out or predict missing values.
In this approach, I specify a distance from the missing values which is also known as the K parameter. The missing value will be predicted in reference to the mean of the neighbours. After imputing values, I reindex the data frame to make recommended target variable at the last of the dataset. Later I do some visualizations such as boxplots to find outliers, count plots, barplot, and correlation matrices for inferences. 
Further, I split the dataset into two parts a training dataset (80%) and a testing dataset (20%). A function is also created to save the performance matrices such as Accuracy, precision, recall, f-1 score, and roc- auc score. The model gets trained from the training data, after training we use regression models such as logistic regression, Decision tree, random forest, K- nearest neighbours and cross-validation technique one by one and evaluated the results.
The test results of all the models are evaluated and compared. We checked performance metrics such as Accuracy, precision, recall, f-1 score, and roc- auc score.
All the models performed well giving accuracy above 93% and logistic regression gave the best result with an accuracy of 95.1%.

### Here is the presentation link:

https://github.com/Zeeshan00789/Airline-Passenger-Referral-Prediction/blob/main/Presentation%20Caps3.pdf



