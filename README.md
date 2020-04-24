# Project 3 : Web APIs & NLP
#### Author: Najiha Boosra (DSI-NYC)

## Problem Statement

This is a binary classification problem. Our goal is two-fold:
- Using API, we have to collect posts from two subreddits
- Then we have to use NLP to train a classifier on which subreddit a given post came from.


We are going to gather and prepare our data using the requests library, To create and compare two models. One of these must be a Bayes classifier, however the other can be a classifier of logistic regression, Bagging Classifier, Random forest, Extra tree etc.We will pick one based on the solution. Through it is about classification model so success will be measured by an accuracy score.

## Executive Summary

After pull requests using API, we are going to use r/baby and r/Pets from the Reddit web page. There are lots of text with punctuations, several signs, spaces, etc, We have to clean all the data as much as possible to perform EDA. Then we use the stopwords method. In the modeling part we have to create a baseline model and then relative classification models. From the models we will get train test and cross Val score.this are the key to find our desired model to evaluate. So we can find the desired matric from the confusion matrix. At last we will find coefficients from the interpretable model using logistic regression.

## Contents:

- **[Case Study: Using `requests` to scrape](#Case-Study)**.

- **[Import Libraries](#Data-Import-Libraries)**.

- **[Converting to Pandas Dataframe](#Converting-to-Pandas-Dataframe)**.

- **[Automating Multiple Pull Requests](#Automating-Multiple-Pull-Requests)**

- **[Data Cleaning & EDA](#Data-Cleaning-Exploratory-Data-Analysis)**.

- **[Model Preparation](#Model-Preparation)**.

 - **[Modeling](#Modeling)**.
   - **[Baseline Model](#Baseline-Model)**.
   - **[Pipeline Models](#Pipeline-Models)**.
   - **[Logistic Regression Models](#Logistic-Regression-Models)**.
   - **[Naive Bayes Models](#Naive-Bayes-Models)**.
   - **[Random Forest](#Random-Forest)**.
   - **[Extra Trees](#Extra-Trees)**.
   - **[Bagging Classifier](#Baggin-Classifier)**.
   - **[DecisionTreeClassifier](#DecisionTreeClassifier)**.


- **[Model Evaluation](#Model-Evaluation)**.

- **[Conclusions and Recommendations](#Conclusions-and-Recommendations)**.

- **[References](#References)**.

### Conclusions and Recommendations

Thus this model will be able to predict a posts for both subreddit with very good accuracy of ~94% by the TfidfVectorizer using Logistic Regression as estimator. In the real world we can find Young Americans may be less likely to be homeowners or parents of human children, but they are leading in their rate of pet ownership. Popularity of baby priority over pets. If we have more data we can be more predictable than this.

This project can be recommended for:
- Use for sentiment analysis of pets vs baby priority
- also how to pull data requests from web

### References

- [Pushshift API](https://github.com/pushshift/api)

- https://api.pushshift.io/reddit/search/submission?subreddit=baby

- https://api.pushshift.io/reddit/search/submission?subreddit=Pets

- https://www.epochconverter.com

- https://pushshift.io/api-parameters/
