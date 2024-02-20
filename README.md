# Identifying Dominant Predictors of Violent Crimes
The research project was primarily done in R to investigate the influence of shall-issue laws and key covariates on violent crime rates.

## Dataset
The “Guns” dataset under the R package “AER.” The dataset is compiled by the U.S. Department of Justice to analyze the effect of gun-control laws on violent crimes. It features a balanced panel of data from 1977–1999 on 50 U.S. states, plus the District of Columbia, 
for a total of 51 states. Each observation is a given state in a given year. 

## Research Question
My research question is to determine the 3 covariates with the largest level of influence on violent crime rates. 
To address the research question, my objective is to build an inference model that best explains the relationship between the violent 
crime rate and other covariates based on our existing observations.

Once I identify the best fitted model, I will rank the covariates based on the magnitude of a one unit change in violent crime rate when holding other variables constant, and select the top three. This analysis aims to support governments in initiating discussions on policy making and implementing targeted programs that could effectively reduce crime rates.

## Explanatory Data Analysis: 
Explore intial relationships between our response (violent crimes) and other covariates present in the data set. Noticed there with a lot of nonlinear associations which would make linear models ineffective. 

## Model Building: 
I built multiple linear regression, ridge regression and additive spline models from scratch to demonstrate how the models were getting better as we started using models that could handle nonlinear associations. How do we define "better model"? I rank the models using a squared loss function - a lower score = better model. This is done by dividing the dataset into a training set and test set. I train the models with the training set and then rank the models using the test set. 

## Determining level of influence: 
To assess the level of influence of each covariate, I standardize them and refit the best model with the standardized data. Standardizing the covariates ensures that each one contributes equally to the model and serves as a fair benchmark for comparisons. To measure the level of influence, we examine the magnitude of a one unit increase for each covariate on the response variable. 

## Tags
Linear regression, ridge regression, generalized additive models, cross validation, spline models, model diagnostics, model selection, model evaluation
