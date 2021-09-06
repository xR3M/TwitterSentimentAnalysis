# Twitter Sentiment Analysis

~ Machine Learning Project 

## Introduction

The goal of this project is to train a Naive Bayes classifier to evaluate the sentiment from thousands of Twitter tweets being either positive or negative.

## Dataset

The "Twitter.csv" dataset will be used for this project. The dataset contains a collection 31962 tweets.

## Data Preprocessing

The csv file contains 3 columns: "id", "label", and "tweet". The column "label" contains the sentiment of the tweet, 0 for positive and 1 for negative. In addition, common stopwords should be removed as it doesn't help with analyzing the sentiment of the tweet, the same goes for punctuations. Also the id column should be removed as it serves no purpose.

## Algorithm Overview

### Functions used

message_cleaning: a function that remove the punctuations and stopwords within a tweet. The input is the tweet and the output is the string of words without punctuations and stopwords.

### Environments

Language: Python

Libraries: Scikit, Pandas, Numpy, Seaborn, Matplotlib, String, nltk

### Results

By using the Naive Bayes classifier from the Sklearn library, we get a model that was able to properly classify 6050 tweets and incorrectly classify 370 tweets. Checking the classification report I noticed that the y_predict_test has a precision of 0.60 while y_test has a prediction of 0.96 which is very substantial. With this in mind, I conclude that using the Naive Bayes classifier produce very poor results and that other types of classifier will probably be more optimal.