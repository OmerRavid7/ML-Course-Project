# ML-Course-Project
Real-estate price prediction comparison
# House Price Prediction

This repository contains a project for predicting house prices using various regression models, including Linear Regression, Ridge Regression, Lasso Regression, and a Neural Network model. Additionally, a meta-model is used to combine the predictions from the individual regression models to improve overall performance.

## Dataset

The dataset used for this project is train.csv. This dataset includes various features related to houses, and the target variable is SalePrice.

## Project Overview

1. *Data Cleaning and Preprocessing*
    - Missing values are handled by dropping columns with a high percentage of missing values and filling remaining missing values with column means.
    - Categorical variables are transformed using one-hot encoding.
    - The dataset is split into training and testing sets.

2. *Modeling*
    - *Linear Regression*: A basic linear regression model is trained and evaluated.
    - *Ridge Regression*: A ridge regression model is trained, and hyperparameters are tuned using GridSearchCV.
    - *Lasso Regression*: A lasso regression model is trained, and hyperparameters are tuned using GridSearchCV.
    - *Neural Network*: A deep neural network model with multiple hidden layers is trained.
    - *Meta-Model*: Predictions from the three regression models are stacked and used as input features for a meta-model, which is a simple neural network.

3. *Evaluation*
    - Models are evaluated using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
    - Results are visualized using scatter plots and loss curves.

## Dependencies

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- tensorflow
