# Identifying Dominant Predictors of Violent Crimes
The research project was primarily done in R to investigate the influence of shall-issue laws and key covariates on violent crime rates.

## Dataset
The “Guns” dataset under the R package “AER.” The dataset is compiled by the U.S. Department of Justice to analyze the effect of gun-control laws on violent crimes. 
It features a balanced panel of data from 1977–1999 on 50 U.S. states, plus the District of Columbia, for a total of 51 states. Each observation is a given state in a given year. 

## Research Question
Our research question is to determine the 3 covariates with the largest level of influence on violent crime rates. 
To address the research question, our objective is to build an inference model that best explains the relationship between the violent 
crime rate and other covariates based on our existing observations.

## Methods
Models: linear regression, ridge regression, additive spline models
Model diagnostics: residual plots, transformations, variance inflation factors
Model selection and evaluation: evaluated performance using a squared loss function against the test set and measured influence by the difference of a standardized 1 unit increase
