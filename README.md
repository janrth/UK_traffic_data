# UK_traffic_data
10 years of UK traffic data. Classification task to identify fatality of an accident

This kaggle data set can be found here(https://www.kaggle.com/tsiaras/uk-road-safety-accidents-and-vehicles). 
It covers 10 years of UK traffic data. 

As a binary classification task I wanted to predict if an accident was fatal using given information about roads, weather, time of the day,
district etc. I used the following algorithms as base models:
            - Logistic Regression
            - Random Forest Classifier
            - XG Boost Classifier
            
Using hyperopt (http://hyperopt.github.io/hyperopt/), a bayesian hyper-parameter optimizer, I tunned all models and picked the winner
based on the ROC AUC score. 

Spoiler: The XG Boost model is the (current) winner with a ROC AUC score of .78.

Additionally I tried to identify the main drivers behind the observed fatality. Using the winning model, it seems that speed (restriction) 
is the main factor for traffic fatality. 
