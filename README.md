# Udacity-DSND-Nanodegree-Capstone

In this project, we'll analyze the data collected from an imaginary music streaming service, Sparkify, where people can listen to music as a free-tier user, in which music can be interrupted with ads, or can subscribe to a plan for uninterrupted service. The dataset provided here has some features related to the user activities on daily basis for 225 users, on the basis of which we'll try to predict which users are more likely to churn.
The types of events reported are: <br/>
- Cancel <br/>
- Submit Downgrade <br/>
- Thumbs Down <br/>
- Home <br/>
- Downgrade <br/>
- Roll Advert <br/>
- Logout <br/>
- Save Settings <br/>
- Cancellation Confirmation <br/>
- About <br/>
- Settings <br/>
- Add to Playlist <br/>
- Add Friend <br/>
- NextSong <br/>
- Thumbs Up <br/>
- Help <br/>
- Upgrade <br/>
- Error <br/>
- Submit Upgrade <br/>

# Objective:

The objective here is to build a machine learning model to predict the users who are more likely to churn, however, the prediction largely depends on how the churn has been defined. Here, we consider tyhe people who have cancelled subscription to be the churned users.

# Approach:

First, we've explored the dataset across various variables and engineered some features at user level based on our exploratory analysis. The engineered features are as follows: <br/>

- Number of songs played by an user  <br/>
- Number of songs listened to on average per session by an user  <br/>
- Number of thumbs up for an user  <br/>
- Number of thumbs down for an user  <br/>
- Whether an user has downgraded or has visited the downgraded page  <br/>
- Number of friends added by each user  <br/>
- Average number of songs played daily by a user  <br/>
- Average session duration for an user  <br/>
- Gender of the user  <br/>
- Level of the user  <br/>

After the feature engineering was done, we scaled the dataset and divided it into train, test and validation sets. We ran logistic regression, random forest, decision tree and gradient boosting classifier on the training set, and based on the performance on the validation set, we chose the decisiopn tree model foe the final prediction on test set. <br/>

The f1-score on test set was 0.83.

# Overview of the files:

This repository contains one Jupyter notebook containing all the data exploration, feature engineering and the model building excercises, and the html version of the same.

# Requirements:

Thie following libraries have been used in this project:

- Pyspark <br/>
- Pandas <br/>
- Numpy <br/>
- Seaborn <br/>


