# airline_delay
This repository consists a personal project that classifies if a flight will get delayed based on some features. The project uses a data from Kaggle to build a machine learning process

# fake-news-classifier
This is capstone project required by Udacity to pass the Data Science NanoDegree. The project is a classifier that aims to classify an article as either fake or real based on the title of the article and the article content. The project follows the data CRISP-DM method


### Table of Content8

1. [Background](#background)
3. [Installation](#installation)
4. [Library Used](#library)
5. [Problem Statement](#statement)
6. [Problem Questions](#questions)
6. [File Descriptions](#files)
7. [Conclusion](#conclusion)
5. [References](#reference)

## Project Motivation <a name="background"></a>

Flight delay has been a bottleneck for many travellers and flight carriers. Most times, the reason for delaying a flight is beyond these carriers. However, these delays affect travellers on getting to their destination at the appropriate time.

In 2013, it was estimated that about 36% of flights were delayed by more than five minutes in Europe, 32% of flights were delayed by more than 15 minutes in the US, and 16% of flights were cancelled or delayed greater than 30-40 minutes in Brazil. Therefore, this indicates how important this indicator is and how it acts no matter how wide the scale of airline is. 

Hence, the insight and prediction model retrieved from this project can contribute in the form of a prototype in helping travellers to identify operational variables that contribute to delays in any airline company. To provide solution to the stated problem, the following questions will be asked and answered.

This implies that if an intending customers have information on the flight they plan to book, they can predict if that flight will be delayed for more than 15minutes

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*. User just need to clone this repository and run the notebook from top to bottom.

## Library Used <a name="library"></a>

The library used includes pandas for data structure and reading data into notebook, numpy for mathematical analysis, seaborn and matplotlib for data visualization and scikitlearn for model estimation. 

## Data Understanding <a name="statement"></a>
The data used for this project is an extract of the data provided by The U.S. Department of Transportation's (DOT) Bureau of Transportation Statistics. They tracks the on-time performance of domestic flights operated by large air carriers. Summary information on the number of on-time, delayed, canceled, and diverted flights is published in DOT's monthly Air Travel Consumer Report and in this dataset of 2015 flight delays and cancellations.

1. Month, DayofMonth, DayOfWeek
2. DepTime – departure time
3. UniqueCarrier – code of a company-career
4. Origin – flight origin
5. Dest – flight destination
6. Distance, distance between Origin and Dest airports
7. dep_delayed_15min – target

## Problem Questions <a name="questions"></a>

To provide solution to the stated problem, the following questions will be asked and answered;
1. How is the delay of flights distributed
2. How is flight delay distributed among the days of the week
3. How is flight delay distributed over period of the day
4. How are delayed flights distributed over the months
5. How are delayed flights distributed over the UniqueCarriers
6. What is the monthly average hour of the delayed flights
7. what is the hourly average distance of destination delayed flights
8. What is the daily average hour of the delayed flights
9. How accurately will the the features predict whether a flight gets delayed for more than 15mins or not


## File Descriptions <a name="files"></a>
The metrics used to measure this project is the Precision-Recall ROC Curve. Precision-Recall is a useful measure of success of prediction when the classes are very imbalanced. In information retrieval, precision is a measure of result relevancy, while recall is a measure of how many truly relevant results are returned.

The precision-recall curve shows the tradeoff between precision and recall for different threshold. A high area under the curve represents both high recall and high precision, where high precision relates to a low false positive rate, and high recall relates to a low false negative rate. High scores for both show that the classifier is returning accurate results (high precision), as well as returning a majority of all positive results (high recall).


## Conclusion<a name="conclusion"></a>

This notebook uses machine learning process to classify fake news. To provide the best model, the researcher made of three set of features to train the model. The model was trained on the NLP pipeline of article title, NLP pipeline of the article content and a set of manual features extracted from the article title and content. 

### Reflection

This project revealed that in order to classify fake news, both the article title and text are good features as they both gave a good precision and recall score. Furthermore, the project also revealed that text features like, number of some part of speech, punctuation counts, word counts, etc. also are good features in classifying fake news. The project however showed that Support Vector Classifier seems to be the best classifier among the classifiers used in this project

### Improvement

This project was created without any hyperparameter tuning. In order to improve the model, one may perform some slight parameter tuning. Also, one may create a pipeline using FeatureUnion to combine the three(3) features and create a single model.

## References <a name="reference"></a>

[Predicting the Survival of Titanic Passengers](https://towardsdatascience.com/predicting-the-survival-of-titanic-passengers-30870ccc7e8)

[Tips for Effective Data Visualization](https://towardsdatascience.com/tips-for-effective-data-visualization-d4b2af91db37)
