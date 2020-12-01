# Machine learning | Assignment06 and Assignment07

## Overview

This repository contains two machine learning assignments from the Data Science for Public Policy course at Georgetown's McCourt School in Fall 2020. The first assignment (assignment06) covers the basics of the statistical concepts behind machine learning and an initial introduction to implementation in R. The second assignment (assignment07) focuses on applying machine learning concepts in R using both pre-defined data and real-world data. 


## Assignment06

This assignment includes exercises that cover error metrics relevant for machine learning and methods for assessing accuracy of a machine learning model. Using a basic data set with just one predictor variable, I compare an intuitive classification model implemented with a custom function in R with a decision tree/CART model implemented using the `parsnip` package from the `tidymodels` family. These are both very simple models and produce identical results in terms of predictions and accuracy. Finally, I implement a K-Nearest Neighbors model by hand and find that a model where k = n was easiest to estimate computationally because the prediction was all the same since you were looking at all observations for each of them (i.e. the prediction was the mode every time). 

## Assignment07

This assignment focused on implementing supervised machine learning models in R. Using restaurant inspection data, I estimate a decision tree classification model using the `tidymodels` framework. Similarly, I then estimate a linear regression model and a KNN model with three different values of *k* for a diamonds data set. I find that the KNN model with *k* = 11 performs the best in terms of the RMSE metric. Finally, I use a DC government data set that includes information on economic development investments from across a variety of agencies and programs for FY15-19 to predict the total DC government investment in a given project based on factors including affordable housing units, affordability levels, number of bedrooms, and others. I implement my first specification as a KNN model and find that *k* = 13 has the lowest error level. In the context of predicting investment levels, however, the model does not perform very well since the error is high relative to the majority of observations. 
