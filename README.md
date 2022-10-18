# job-application
Predict the success or failure of  a job application
@author: Talardia Gbangou, October 2022

Objective:
This notebok contains the results of the data exploration and building of a machine learning model to predict the success and failure of application of the position of chercheur d’or chez OrFée.

Project: 
This project writes a functional and structured code in python using a jupyter notebook. It contains the following steps:

1.1. Data description

* importing relevent libraries
* load dataset
* checking influence of some features on the target or depedent variable
* checking wether we have balanced or imbalance dataset
* find and treatting missing dataset
* converting categorical data

1.2. Significance test: we used sveral stattistical tests techniiques dependending the variables considered:
* a) for significance test between two categorical nominal variables we used CHI-SQUARE test
* b) for significance test between a categorical and numerical variable, we used anova test
* c) for significance test between two numerical variables we used ttest

Conclusion: 
According to the analyses, there is indeed a statistically significant dependence (at 95% confidence interval) between:
(a) Specialty and gender,
(b) hair color and salary, and
(c) Years of experience and the grade

1.3 Treating categorical variables as part of feature engineering :¶
We have nominal variables so we performed one hot encoding (which is appropriate here)

2. Machine learning
Randform forest is a popular supervised machine learning algorithm based on ensemble learning that we will use for our classification problem
We did some tuning of the hyperparameter of the random forest model to treat the overfiting and to take into account the imbalanced dataset
Confusion metric and F-score (combine precision-recall) are used in order to take into account the imbalanced dataset
Feature importance with the random forest is also assessed

2.2. Building a machine learning model for prediction¶
Randform forest is a popular supervised machine learning algorithm based on ensemble learning that we will use for our classification problem
2.3 Feature importances
2.4 Random Forest Model evaluation after feature selection¶
based on the feature importance, we can re-evaluate the the model performance by droping some of least important features (e.g. let's drop the 3 last features U, brun and roux)

Conclusion final:¶
by removing the tree least important features, the random forest model still predicts the success and failure of application with an accuracy of around 88%. Performing further hyperparameter tuning and playing with feature importance can potentially help improve the model performance beyond 88%.

Tech Stack
* python using a jupyter notebook 
* (Python 3.9.7)

