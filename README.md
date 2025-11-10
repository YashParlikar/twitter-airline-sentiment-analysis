# Project Step 3 – Code Review Submission
IS392 (451) — Group F: Anika and Yash 
Date: November 9th 2025

# Project Title
Twitter US Airline Sentiment Analysis

Our group project for IS392, AI Text-Driven Analytics, involves developing a language processing model to predict the sentiment of a given Twitter user.


To use the model, ensure that the Tweets.csv file is in the same directory as the Python script, or else the script won't be able to locate the csv file.



## Project Overview
This project analyzes U.S. airline sentiments using tweets. We perform text preprocessing, exploratory data analysis, and build an initial classification 
model to predict tweet sentiment (positive, neutral, or negative).
Dataset: [Twitter US Airline Sentiment – Kaggle](https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment)

## How to Run the Code
1. Ensure Python 3.10+ is installed.
2. Download the dataset Tweets.csv
3. Open and run .ipynb file from start to finish.

## What the code accomplishes 
- loads and cleans tweet text (by fixing punctuation, URLs, and removing stopwords)
- Performs exploratory analysis (with visualizations using bar charts)
- Converts text to TF-IDF features
- Trains a Logistic Regression classifier.
- Evaluates using F1-score and confusion matrix

## Known issues/ next steps
- Neutral sentiment classification is not as strong and negative tweets are a majority --> can take steps to try Linear SVM to balance weight better
- Removal of emojis and punctuation --> we can try to use emoji sentiment scores to better reflect the sentiment scores
- Removal of domain stopwords may exclude important words --> we can compare model accuracy with and without domain stops.
- Tweets contain sarcasm/humor that may go undetected --> we can try using more advanced models (maybe transformer-based models)
