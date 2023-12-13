# Project Name
> Bike Sharing Assignment

## Table of Contents
* [General Info](#general-information)
* [Approach](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)

## General Information
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

Dataset containing previous years Demand data was provided, Objective is 
1. To model the demand for shared bikes with the available independent variables
2. To understand Which variables are significant in predicting the demand for shared bikes
3. To understand how exactly the demands vary with different features

So, accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations

## Approach
1. [Importing Necessary Modules](#Importing-Necessary-Modules)
2. [Data Understanding](#Data-Understanding)
   - [Loading Data from the CSV](#Loading-Data-from-the-CSV)
   - [Understanding Structure of dataset](#Understanding-Structure-of-dataset)
   - [Data Quality checks](#Data-Quality-checks)
3. [Data Preparation](#Data-Preparation)
    - [Fixing Data Types](#Fixing-Data-Types)
    - [Converting Values to clean and understandable format](#Converting-Values-to-clean-and-understandable-format)
    - [Droping irrelevant columns](#Droping-irrelevant-columns)
    - [EDA](#EDA)
       - [Univariate Analysis](#Univariate-Analysis)
       - [Bivariate Analysis](#Bivariate-Analysis)
    - [Creating Dummy Variables](#Creating-Dummy-Variables)
4. [Model Building](#Model-Building)
    - [Test Train Split](#Test-Train-Split)
    - [Scaling features](#Scaling-features)
    - [Feature Selection](#Feature-Selection)
       - [RFE](#RFE)
       - [Manual Feature Selection](#Manual-Feature-Selection)
5. [Model Evaluation](#Model-Evaluation)
       - [Residual Analysis](#Residual-Analysis)
       - [Model Evaluation using Test data](#model-Evaluation-using-Test-data)
       - [Model Efficiency](#Model-Efficiency)

## Conclusions
$ cnt  = 0.1481-0.0994  \times holiday + 0.5408 \times temp -0.1615 \times windspeed + 0.0722 \times season \_ summer + 0.1153 \times season\_winter + 0.2331 \times yr\_2019
-0.0442 \times mnth\_JAN -0.0398 \times mnth\_JUL +0.0898 \times mnth\_SEP -0.2845 \times weathersit\_Light Snow -0.0798 \times weathersit\_Mist Cloudy $

Following are the predictor impacting demand in order highest to lowest
1. temp
2. weathersit_Light Snow
3. year 2019
4. windspeed
5. season_winter
6. holiday
7. mnth_SEP
8. weathersit_Mist Cloudy
9. season_summer
10. mnth_JAN
11. mnth_JUL

How well this predictors describe demand is explained by it's respective co-efficient on the above equation


## Technologies Used
- numpy - version 1.5.3
- pandas - version 1.24.3
- seaborn - version 0.12.2
- matplotlib - version 3.7.1
- statsmodels - version 0.13.5
- sklearn - version 1.2.2

## Contact
Created by [@arung12] - feel free to contact me!