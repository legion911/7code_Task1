
# Titanic Classification

A brief description of what this project does and who it's for

![image](https://github.com/legion911/7code_Task1/assets/118493225/2b17b4e2-06bf-45d4-af67-6ca13a49c3f0)


## About

RMS Titanic

Possibly the most well-known shipwreck in today's popular culture is the R.M.S. Titanic. It was the largest and most opulent passenger ship available at the time, and it was said to be unsinkable. Launched on May 31, 1911, Titanic carried 2,240 passengers and crew on its maiden trip, which departed from Southampton on April 10, 1912. More than 1,500 passengers and crew perished when the Titanic fell to the bottom of the ocean on April 15, 1912, after colliding with an iceberg.
## Introduction

This repository contains an end to end analysis of the Titanic-dataset and a brief solution to the problem of titanic survival prediction. Additionally, we make use of a variety of ML methods in an effort to produce the most accurate model possible.
## Problem Statement

Can we predict if a passenger on the Titanic has survived given what we know about them? To put it another way, we are developing a machine learning model to discover the correlation between passenger characteristics and their likelihood of surviving and then use that knowledge to estimate survival outcomes for passengers whose data we have not yet trained our model on.
## EDA (Exploratory Data Analysis)

Passenger ID - To identify unique passengers

Survived - If they survived or not (0 = Dead 1 = Alive)

P Class - The class passengers travelled in

Name - Passenger Name

Sex - Gender of Passenger

Age - Age of passenger

SibSp - Number of siblings or spouse

Parch - Parent or child

Ticket - Ticket number

Fare - Amount paid for the ticket

Cabin - Cabin of residence

Embarked - Point of embarkment (C = Cherbourg; Q = Queenstown; S = Southampton)

## Data Preprocessing

This stage involves finding the empty cells or any duplicate entries in the dataset. If found, the missing values can be replaced based on the column. We can replace missing values for the 'Age' column by filling those cells with the mean value of the age. Label encoding is done for easier interpretation of categorical data. Normalization of data is done in the later stages using MinMaxScaler.
## Data Visualization

![image](https://github.com/legion911/7code_Task1/assets/118493225/cee8686a-c1b5-4419-9391-f3b51e176b2a)

![image](https://github.com/legion911/7code_Task1/assets/118493225/401ff445-f2b8-4e65-a5d7-4f2c86c14ecb)


Distribution plots of Age vs Survived and Age vs PClass are produced which is followed by a Correlation heatmap and pairplot of the data.
## Sample Testing

![image](https://github.com/legion911/7code_Task1/assets/118493225/3a35da9d-59cd-42a8-b47c-b1c70d36a24a)


Sample data is taken for the purpose of training and testing. The columns which are deemed to be of no use are dropped from the dataset. Logistic regression algorithms is applied on the model and the classification report is obtained along with a confusion matrix.
## Model Selection

Here we define a function classify( ) which will run the model against various ML algorithms and compute accuracy and cv scores. The classification algorithms used are as follows -

DecisionTree

RandomForest

ExtraTrees

XG Boost

KNN

Ada Boost
## Conclusion

Through our analysis we conclude that RandomForestClassifier provides the most accurate predictions when it comes to determining the survival of a passenger on the RMS Titanic.
