# Predicting-Asthma-Rates-in-California
![Asthma](Asthma.jpg)

Author: Pranjal Srivastava

## Date: 5/8/2022

This project aims to predict Asthma rates in California using various environmental factors such as the presence of pesticides, toxic releases, pollution burden score, PM2.5, traffic, and ozone levels. The data used for this project is extracted from the Clean_Cal_Environtmentdata.csv file, which contains comprehensive information about the environment in different regions of California.
Stages in the Project

## 1. Data Cleaning
The project begins by cleaning the dataset and removing any missing values to ensure accuracy in predictions. This process involves using the na.omit() function and writing the clean data back to the csv file.

## 2. Univariate Analysis & Standard Deviation
Univariate analysis is carried out to summarize individual variables in the dataset. Standard deviations for the variables are also computed.

## 3. Exploratory Plots
Histograms and scatter plots of the variables are drawn to observe the distribution of data and potential relationships between variables.

## 4. Fitting a Model
A multiple linear regression model is fitted on the data using all the variables to predict asthma rates.

## 5. Diagnostics
The residuals of the model are plotted against the fitted values to identify any non-linearity or heteroscedasticity. Quantile-Quantile plots are used to verify the assumption of normality for the residuals. The presence of outliers and multicollinearity is also checked.

## 6. Modified Model
A Box-Cox transformation is applied to handle non-normality in the dependent variable, and a new model is fit on the transformed variable.

## 7. Removing Outliers
Cook's Distance is calculated for each observation in the new model to identify outliers. Any observation with a Cook's Distance greater than 4/n is considered an outlier and removed from the dataset.

## 8. Final Model Selection
Models are compared based on their AIC scores and the model with the minimum AIC score is selected. This model includes Ozone, Traffic, Pollution Burden Score, and Toxic Release as predictors.

## Usage

To replicate this analysis, you need to run the code provided in this README in an R environment. You should also have the Clean_Cal_Environtmentdata.csv file in your working directory. The code has been written and commented in a way that allows for easy understanding and modification.
