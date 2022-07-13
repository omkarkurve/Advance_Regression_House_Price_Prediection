# Project Name

### Housing Price Prediction using Ridge and Lasso Regression

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below. The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not. The company wants to know the following things about the prospective properties:

Which variables are significant in predicting the price of a house, and how well those variables describe the price of a house.
Also, determine the optimal value of lambda for ridge and lasso regression.
Reading and Understanding the Data

### Basic Data Cleanup
Missing value check and imputation using Business Logic.
Cahnging data types of the variables.

### Exploratory Data Analysis:

Performed Univariate and Bi-variate analysis on identified variables. = Correlation heatmap

### Data Preparation for model building:

Performed Robust Scaling of numerical features using median and quantile values.
Performed Variance Thresholding (threshold= .003) to exclude the features having almost zero variance.

### Model Building:
Ridge Regression model with GridSearchCV to find optimal value of alpha.
Identified top 25 features based on beta coefficient values.


## Conclusions

- Ridge and Lasso both the models have almost same test and train accuracy. So it can be said that there is no overfitting.
- Lasso and Ridge both have similar r2 score and MAE on test dataset. But Lasso has eliminated 110 features and final no. of features in Lasso Regression model is 116. Where - Ridge has all 226 features. So, our Lasso model is simpler than Ridge with having similar r2 score and MAE. Ridge Regression model on test dataset: r2 score= 0.8912, MAE= 0.0934, RMSE= 0.1357 Lasso Regression model on test dataset: r2 score= 0.8947, MAE= 0.0914, RMSE= 0.1335
- Considering above points we can choose our Lasso Regression model as our final model.

## Technologies Used

pandas - v1.3.4
numpy - 1.20.3
matplotlib - v3.4.3
seaborn - v0.11.2
sklearn - v0.24.2


## Contact
Created by [@gitomkarkurve] - feel free to contact me!
