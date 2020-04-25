# airline_delay
This repository consists a personal project that classifies if a flight will get delayed based on some features. The project uses a data from Kaggle to build a machine learning process


### Table of Content8

1. [Background](#background)
2. [Installation](#installation)
3. [Library Used](#library)
4. [Project Definition](#definition)
    [Problem Motivation](#motivation)
    [Problem Questions](#questions)
    [Metric](#metric)
5. [Data Understanding](#understanding)
6. [Analysis](#analysis)
7. [Conclusion](#conclusion)
5. [References](#reference)


## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*. User just need to clone this repository and run the notebook from top to bottom.

## Library Used <a name="library"></a>

The library used includes pandas for data structure and reading data into notebook, numpy for mathematical analysis, seaborn and matplotlib for data visualization and scikitlearn for model estimation. 

# Project Definition <a name="definition"></a>

## Project Motivation <a name="motivation"></a>

Flight delay has been a bottleneck for many travellers and flight carriers. Most times, the reason for delaying a flight is beyond these carriers. However, these delays affect travellers on getting to their destination at the appropriate time.

In 2013, it was estimated that about 36% of flights were delayed by more than five minutes in Europe, 32% of flights were delayed by more than 15 minutes in the US, and 16% of flights were cancelled or delayed greater than 30-40 minutes in Brazil. Therefore, this indicates how important this indicator is and how it acts no matter how wide the scale of airline is. 

Hence, the insight and prediction model retrieved from this project can contribute in the form of a prototype in helping travellers to identify operational variables that contribute to delays in any airline company. To provide solution to the stated problem, the following questions will be asked and answered.

This implies that if an intending customers have information on the flight they plan to book, they can predict if that flight will be delayed for more than 15minutes

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

## Metric <a name="metric"></a>
The metrics used to measure this project is the Average Precision Score . AP summarizes a precision-recall curve as the weighted mean of precisions achieved at each threshold, with the increase in recall from the previous threshold used as the weight


# Data Understanding <a name="understanding"></a>
The data used for this project is an extract of the data provided by The U.S. Department of Transportation's (DOT) Bureau of Transportation Statistics. They tracks the on-time performance of domestic flights operated by large air carriers. Summary information on the number of on-time, delayed, canceled, and diverted flights is published in DOT's monthly Air Travel Consumer Report and in this dataset of 2015 flight delays and cancellations.

## Data description

1. Month, DayofMonth, DayOfWeek
2. DepTime – departure time
3. UniqueCarrier – code of a company-career
4. Origin – flight origin
5. Dest – flight destination
6. Distance, distance between Origin and Dest airports
7. dep_delayed_15min – target

## Data Preprocessing

The data used contained no missing values, hence the was no need for hanling missing values. However, some columns were reported in a way that may not provide enough information, more features were extracted from the existing features.

## Data Exploration

The data shows that there are 100000 observations of flights recorded which also implies that there are no missing observations. using bar chart, the data shows the count of the delayed and non-delayed flights. It shows that that about 19% of the total flights were delayed for more than 15mins, while 81% were not cancelled. 

# Analysis <a name="analysis"></a>

## Implementation <a name="implement"></a>
We split the user set into training (80%) and test (20%), and create a pipeline that assembles the features selected above, then runs a machine learning model; our problem is a classification one, so we implemented the following algorithms:

1. Logistic regression
2. Decision tree
3. Random forest
4. Gradient boosted tree
5. Naive Bayes
6. KNeighborsClassifier



## Conclusion <a name="conclusion"></a>

The project explored how some flight features relate with the delay of such flights. The revealed that Southwest Airlines has the highest proportion of delay. The project also selects RandomForestClassifier as the best algorithm using the average precision score as an evaluation metric.

The complete discovery of this project can be found at [here](https://medium.com/@adeotiadegboyega/will-my-flight-be-delayed-or-not-dfb440c12b44?sk=e3311e52f2371f1f87fc97a3e7a84141)


## References <a name="reference"></a>

[Predicting the Survival of Titanic Passengers](https://towardsdatascience.com/predicting-the-survival-of-titanic-passengers-30870ccc7e8)

[Tips for Effective Data Visualization](https://towardsdatascience.com/tips-for-effective-data-visualization-d4b2af91db37)
