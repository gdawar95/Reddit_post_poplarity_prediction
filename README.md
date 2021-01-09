# Reddit_post_poplarity_prediction

## Table of contents

    Introduction and data insights*	3
    Project Outline*	3
    1	Data Preprocessing*	4
    2	Feature Engineering	5
      2.1	Author Feature*	5
      2.2	Created_utc Feature	5
      2.3	Domain Feature*	6
      2.4	Title Feature*	7
      2.5	URL Feature	8
      2.6	Brand_safe, is_crosspostable, no_follow, subreddit, subreddit_type, whitelist_status Feature*	8
    3	Data Exploration	9
      3.1	Exploring Scores	9
      3.2	Exploring Authors*	10
      3.3	Exploring created_utc*	10
      3.4	Exploring Domain*	12
      3.5	Exploring Subreddit*	14
      3.6	Feature Correlation*	14
    4	Model Development	16
      4.1	Feature Selection*	16
      4.2	Model Selection	16
        4.2.1	Linear Regression	17
        4.2.2	Decision Trees (Regression)	17
        4.2.3	Random Forest Regression*	17
      4.3	Model Evaluation*	17
      4.4	Best Model	19
    5	Model Tuning and Tesing (Results)	20
      5.1	Tuning	20
      5.2	Testing (Result)*	21
    References	22

## Introduction and data insights*

Reddit is a social website to share content related to a plethora of topics called “posts”. The readers also have and option to “upvote” or “downvote” a post which is an indicator of the post’s popularity. While the popularity of the post depends on its content, however there are a variety of other features which can influence the popularity of the post. The purpose of the project is to predict the total votes received by a post or its “popularity” based on a number of features about the post such as its title, time of post, author etc. The dataset has the posts data and related features from year 2006 and has target column “score” with whole number scores ranging from 0 to 583 and 58 feature columns having both numerical and categorical features. The data points exceed 12,500 in the dataset.

## Project Outline

    1.	Data Preprocessing – Cleaning the data from null or missing values and removing sparse features 
    2.	Feature Engineering – Generating new features from the existing features to help our model learn
    3.	Data Exploration – Exploring the dataset for statistical insights and dependencies of features to target
    4.	Model Development – Deploying multiple machine learning models and comparing their performance using R2 and RMSE evaluation metrics
    5.	Tuning and Testing – The best model is then chosen and tested in the OOT (out of time) dataset so verify if the model has generalized enough to predict scores of completely unseen reddit posts data.

