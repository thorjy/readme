# SC1015 Mini-Project
For our mini project in the Introduction to Data Science and Artificial Intelligence module (SC1015), we performed analysis on the Student Alcohol Consumption [dataset](https://www.kaggle.com/datasets/uciml/student-alcohol-consumption) from Kaggle.

## Overview
We will use Machine Learning techniques to optimise the environment for Students in an attempt to improve their grades.

## Members (Team 4)
1. Thor Jia Ying
2. Haw Jin Yu
3. Wong Ho Yi Ethan

## Problem Definition
Main Problem
* How can we optimise the environment to improve Students’ Grades? 

Sub-Problems
* What are the factors that are important in determining our grades?
* How can we sieve out students who are in need of help? 

### Notebook Details
#### Data Cleaning and Preparation
   1. Checking for Null values that exist inside the data sets.

   2. Merging the two datasets on Math and Portugese by finding the intersecting key values in certain columns and creating new columns to represent the grades of the students better 

   3. Remove insignificant datas that are not within our age scope : Scrutinizing the data such that we only include age groups 15 to 19 years old.
   
   4. Remove insignificant columns by dropping them : "school", "guardian", "sex", "reason".

#### Visualisation of data
   1. Correlation check, to find out which variables are suitable to be explored.

   2. Used box plots, heatmaps, and histograms to visualise our variables.


#### Exploratory Data Analysis
  1. Checked the relationship of interesting and the higher correlated independent variables against students overall grades

  2. Combined certain columns to provide better visualisation 


#### Machine Learning
   1. Linear Regression Models

          a. Using Uni-Variate to determine factors that have the best linear correlation with "Total Grades" (Final Grade, sum of "G1", "G2", and "G3")
          
          b. Using Multi-Variate to see how the combination of various social factors will affect "Total Grades". 
          
   2. Ordinary Least Square Regression

          a. Using OLS Regression, we are able to find out which variables are statistically significant. These variables are time taken, romantic relationship status, parents education and family relationship.

   3. Random Forest Classification 

          a. Looking at the feature importance we are able to find out what variables are important when predicting student grades using a Random forest.

          b. We decided not to use the random forest because total grade is a continuous variable and it is non binary. However it can be useful if we were to have information about the minimum passing score. Classifying student grades according to pass and fail.

          c. Similar to the regression model, previous grades is the most importance variable to predict total grade.
          
         
#### Conclusion

 1. There are many variables that can affect student grades. However, amongst all of them, there are only a selected few than can be manipulated in order to optimise student grades.

 2. The important variables that determines grades are "G1", "G2", results of the first and second trimester respectively, and "Failures". Using this information, we are then able to tackle our first subproblem. Since we know these factors play an important role, to perform badly in the first and second trimester will be an indication of how the student will subsequently perform for their final grade. Hence, educators and parents could use the grades at the trimesters as an early detection of weaker students, pulling them out and provide them the necessary help. Alternatively, one could also sieve out the students who have high frequency of failed test, and provide more guidance on the respective failed topics.

 3. Correlation does not equal causation, we cannot be 100% sure if these solution can improve grades. But there is definitely a good chance that it can impact grades based on our statistic analysis. Some social factors that we can provide solutions for are "travel time", "romantic", "Fedu" (Father's education), "Medu"(Mother's education) and "famrel"(Family relationship).

 4. Overall, we solved subproblems 1 and 2, and came to an answer for our main problem.


### What we have learnt from this project?

1. Machine learning may be able to help predict outcomes based on given training data set, but ultimately it should not be heavily relied on./

2. The use of new machine learning techniques such as Ordinary Least Square Regression and Random Forest Classification

3. Categorical data have no reference scale, so each persons' scale of categorical perception is different, therefore the results drawn may not be accurate. 


### Contributions
Haw Jin Yu - Machine learning, New and Beyond, Conclusion, sides, ReadMe, Video

Wong Ho Yi Ethan - Data cleaning, Data Exploration, Data analysis, slides, ReadMe

Thor Jia Ying - Introduction and Problem Formulation, Machine learning, slides, ReadMe


### References
https://www.kaggle.com/datasets/uciml/student-alcohol-consumption

https://vitalflux.com/ordinary-least-squares-method-concepts-examples/

https://towardsdatascience.com/a-practical-guide-to-implementing-a-random-forest-classifier-in-python-979988d8a263?gi=93e3d85833b7

https://www.edutopia.org/article/5-ways-help-students-focus-learning-rather-grades/

