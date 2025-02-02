# Home Price Prediction in California

Project Overview

This project aims to predict housing prices in California using machine learning models. Various regression techniques were applied to determine the most accurate model for estimating median house values based on features such as median income, housing median age, and proximity to ocean locations.

Dataset Description

The dataset contains housing-related attributes, including:

Longitude & Latitude: Geographic coordinates

Housing Median Age: Age of the house

Total Rooms & Bedrooms: Number of rooms and bedrooms

Population & Households: Number of residents and households

Median Income: Income levels in the region

Median House Value: Target variable to predict

Ocean Proximity: Categorical variable indicating closeness to the ocean

Problem Statement

The goal is to build a predictive model that estimates house prices accurately using regression models while identifying the most influential features affecting housing prices.

Data Preprocessing

Handled missing values using KNN Imputation.

Encoded categorical data using One-Hot Encoding.

Created new features such as:

Rooms per Household

Bedrooms per Room

Population per Household

Coordinate Ratios

Removed less relevant features to avoid multicollinearity.

Model Training & Evaluation

Several regression models were trained and evaluated:

Linear Regression

R^2 Score: 0.61

RMSE: High error variance

Random Forest Regressor

R^2 Score: 0.78

RMSE: 52,640

XGBoost Regressor (Default Parameters)

R^2 Score: 0.79

RMSE: 51,555

XGBoost Regressor (Hyperparameter Tuned)

R^2 Score: 1.0 (Overfitted)

RMSE: 221.63 (Likely due to overfitting)


Results & Conclusions

XGBoost (default settings) performed the best, achieving 79% accuracy with a low RMSE.

The hyperparameter-tuned XGBoost model showed overfitting, achieving an R^2 of 1.0 (which is unrealistic in real-world scenarios).

Feature importance analysis indicated that median income, population per household, and bedrooms per room were key drivers of house prices.

The goal of predicting median house values was successfully achieved with high accuracy using ensemble models.


Key Learnings

Feature engineering significantly improved model performance.

Handling missing values and encoding categorical data effectively increased accuracy.

Ensemble methods like Random Forest and XGBoost outperformed basic regression models.

Overfitting is a risk when hyperparameter tuning is too aggressive.

