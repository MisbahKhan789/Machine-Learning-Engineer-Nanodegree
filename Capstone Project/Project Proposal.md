# Project Proposal 

## Domain Background

The topic of this ML project will be "Daily News for Stock Market Prediction". The project idea is inspired by an existing Kaggle dataset. As for background information, the resource of daily news is crawled from 
historical news headlines of Reddit World News Channel. The news are ranked by reddit users' votes, and only the top 25 headlines are considered for a single date. Meanwhile, the stock data is taken from Dow Jones Industrial Average (DJIA).

## Problem Statement 

Can we predict Dow Jones Industrial Average (DJIA) rise or fall based on top news headlines of that day? In this project, I plan to utilize advanced NLP & ML skills to provide a solution of predicting the rise/fall of DJIA value as a binary classification task.

## Datasets and Inputs 

Although three csv files are posted on Kaggle, the creator actually posted one of the three as a combined dataset of the other two. Therefore, simply we only need to consider the csv file named as "Combined_News_DJIA.csv". This dataset has 27 columns & 1989 rows. 
27 column features contains 25 top news each, datetime and a label (0 or 1). The label is given as whether the DJIA rises(1) or falls(0) in that day. 

## Solution Statement

Basic thoughts:
- Applying countvectorizer to all the headlines.
- Applying Machine Learning Algorithms (Random forest , XGBOOST and CATBoost). 
- Comparing Accuracy & Hyperparameter Tuning 

However, I don't want to merely fit on a traditional ML pipeline for this project. In fact, I would like to try other more advanced word embedding method and models for this project as well. To explore some methods that I haven't encountered before in the domain of NLP is also 
a goal of this project. 

## Benchmark Model

- Random forest
- XGBOOST
- CATBoost

## Evaluation Metrics

- classification report
- confusion matrix
- accuracy score 

Results based on model will also go through model tuning steps for the highest accuracy. Tuning methods including: GridSearchCV, RandomizedSearchCV.

## Project Design

- Data Preprocessing (filling NaN values; combining news columns)
- NLP Preprocessing (removing punctuations; changing texts to lowercases)
- ML Pipeline (applying countvectorizer to all the headlines; applying ML models)
- Model Tuning (utilizing GridSearchCV/RandomizedSearchCV to achieve higher accuracy)
- Model Comparing (comparing final results among models)
- Converting the whole process into a ML pipeline 
- Presenting as a user-friendly ML web app (Input Textarea: entering today news; Output Label: predicting today DJIA rise/fall)
