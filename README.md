# Twitter Depression Detection

![alt text](https://github.com/miladrezazadeh/twitter_depression_detection/blob/main/img/depression.png?raw=true)

## Overview

Social media platforms such as Twitter, Instagram and Facebook play dominant roles in our day to day life. The popularity of these platforms has been significantly increased during the pandemic. Studies show that people are more likely to share their feelings and emotions on Twitter since the beginning of the Covid-19 pandemic. Positive emotions are not commonly associated with higher life satisfaction; however, negative emotions are more likely to express a person true feelings. 

Depression is the most common mental disorder which is more than just being sad. Some signs of depression are lack of interest in daily activities, significant weight loss or gain, insomnia or excessive sleeping, lack of energy, inability to concentrate, feelings of worthlessness or excessive guilt and in severe cases recurrent thoughts of death or suicide. Auspiciously, depression is treatable. The treatment is a combination of therapy and antidepressant medication.


## Background and Motivation

* Large volumes of data which can be retrieve from social media platforms such as Twitter can potentially provide valuable insights into human behaviour and emotions. 

* Twitter is one of the most common platform for people to share their emotions and opinions which could be used to provide a better understanding of their mental health and wellbeing, people’s everyday decision-making and perceptions about their quality of life.

* Depression is the common mental disorder and which may result in suicides. There are more than 300 million people suffer from depression every year globally.


## Goals

The goal of this project is to implement supervised machine learning techniques in order to detect tweets containing depressive characteristics. 

## Datasets

We need two types of datasets one with tweets containing depressive characteristic which is obtained from twitter API and the other one with random tweets.

1. Data mining more than 20K tweets by using [Twitter API and Tweepy library](https://github.com/miladrezazadeh/twitter_depression_detection/blob/main/notebooks/data_gathering_twitter_API.ipynb). The raw data retrieved from Twitter can be find [here](https://github.com/miladrezazadeh/twitter_depression_detection/tree/main/data/raw/scrapped).  

2. Random tweets has been extracted from the [Kaggle datasets](https://www.kaggle.com/ywang311/twitter-sentiment/data). 

* The processed dataset used for training machine learning algorithms can be find [here](https://github.com/miladrezazadeh/twitter_depression_detection/tree/main/data/processed).

## Data Science Pipeline:
* Data Collection : Balanced dataset collected from Twitter API and Kaggle dataset.
* Data Preprocess: Data Cleaning/exploring/processing/Anotation/Analysis via NLP libraries.
* EDA and Feature Selection : CountVectorizer, TFIDF, spaCy word embedding model, spaCy word embedding model.
* Model Selection : Logistics Regression, support vector machine(SVM), k-nearest neighbors(k-NN), Decision Tree Classifier, Random Forest Classifier, Neural Network, LSTM
* Model Training : Scikit-Learn
* Inference : F1-Score, Confusion matrix and ROC-AUC to make an inference
* Model Deployment : Deployment on AWS or heroku
* Data Product : Flask-based web application

## Practical Applications

## Milestones

## Libaries to install
Use the package manager [pip](https://pip.pypa.io/en/stable/) to install requred libraries.

```bash
pip install -r requirements.txt
```

## Clean the dataset

```bash
python clean.py <file_name> 
```
## Train the best model
```bash
python train.py <file_name> <model_name>
```
## Predict 
```bash
python predict.py <tweet.txt> SVM
```
## References

* https://www.apa.org/topics/depression
* https://www.kaggle.com/ywang311/twitter-sentiment/data
