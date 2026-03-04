# Greenhouse Gas Emissions Prediction

## Overview
This project aims to predict the average annual greenhouse gas emissions of companies using machine learning models.

The goal is to evaluate whether company characteristics and geographic location can explain emission levels.

## Dataset

The dataset includes:

- company category
- longitude
- latitude
- average annual emissions (target variable)

The data was split into:
- training dataset
- testing dataset

## Problem Type
This is a **regression problem**, as the target variable is a continuous numerical value.

## Data Preparation
- Removed non-informative variables (company name, industry code)
- Checked for missing values
- Converted categorical variables to factors

## Models Trained

### K-Nearest Neighbors
- hyperparameter tuning for k
- cross validation

### Neural Network
- tuning for hidden units
- weight decay regularization

### Random Forest
- tuning number of predictors per split

## Model Evaluation
Models were evaluated using:

- RMSE
- MAE
- R²

## Results
The **KNN model achieved the best predictive performance** with the lowest RMSE.

## Tools
- R
- tidyverse
- caret
- machine learning models
