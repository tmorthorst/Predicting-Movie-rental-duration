# Predicting Movie Rental Durations: Regression & Feature Engineering

## Project Overview
This project focuses on building a machine learning regression model to predict the number of days a customer will rent a DVD. The main goal is to optimize inventory planning by achieving a Mean Squared Error (MSE) of less than 3 on the unseen test dataset.

## The Assignment
The management at the DVD rental company needs a predictive model to improve their inventory logistics. Specifically, they have set the following requirements:

* **Target Variable:** Calculate the rental duration in days by subtracting the rental date from the return date.
* **Feature Engineering:** Extract binary dummy variables (1 or 0) from the `special_features` column for titles containing "Deleted Scenes" and "Behind the Scenes".
* **Data Splitting:** Execute a train-test split, reserving 20% of the data for final evaluation.
* **Feature Selection:** Standardize the numerical features and use Lasso Regression (L1 penalty) to identify and select the most important predictors.
* **Modeling & Tuning:** Train an ensemble regression model (such as Random Forest) and perform hyperparameter tuning using randomized search and cross-validation.
* **Evaluation:** Predict the values on the test set and compute the Mean Squared Error (MSE) to ensure it is below the threshold of 3.

## Results
By engineering text-based features, applying Lasso for strict feature selection, and tuning a Random Forest Regressor, the final model successfully predicted rental durations with an MSE well below the required threshold. This makes the model a highly viable tool for automated inventory optimization.