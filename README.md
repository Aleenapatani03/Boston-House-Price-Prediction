# Boston House Price Prediction

## Project Objective

This project aims to predict house prices in Boston using machine learning regression models. We implemented several regression algorithms to determine the best model based on performance metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² Score.

## Introduction

The Boston Housing dataset is a popular dataset for regression tasks. It contains data about the housing prices in Boston, along with features such as crime rate, average number of rooms, distance to employment centers, and more. The objective is to predict the median value of homes in the area based on these features.

## Data Preprocessing
Steps taken in data preprocessing:

 1.Loading the Dataset:

The dataset is available through sklearn.datasets.load_boston() or can be found in CSV format online.

 2.Handling Missing Data:

The dataset was inspected for missing values, and any missing data was handled by imputation or removal (if necessary).

 3.Feature Scaling:

Some regression models (such as Support Vector Machines) may require scaling of features. We used StandardScaler to scale the data if necessary.

 4.Feature Engineering:

The dataset contains both numerical and categorical features. We made sure all the features are in the appropriate format for the models.

 5.Splitting the Dataset:

The dataset was split into training and test sets using train_test_split.

 Modeling

We trained the following regression models:

1.Linear Regression

2.Ridge Regression

3.Lasso Regression

4.Random Forest Regressor

5.Gradient Boosting Regressor

6.Support Vector Regressor (SVR)

7.Decision Tree


## Model Evaluation
Evaluation Metrics:
We evaluated the performance of each model using the following metrics:

1.Mean Absolute Error (MAE): Average of the absolute differences between the predicted and actual values.

2.Mean Squared Error (MSE): Average of the squared differences between the predicted and actual values.

3.Root Mean Squared Error (RMSE): Square root of MSE, providing a sense of the magnitude of the error.

4.R² Score: Measures the proportion of variance in the dependent variable that is predictable from the independent variables.

## Results

1.Best Model: Gradient Boosting Regressor

R² Score: 0.9144 (explained 91% of the variance in the data)

RMSE: 2.50 (low error, indicating accurate predictions)

Achieved the highest performance among all models.

2.Second Best Model: Random Forest Regressor

R² Score: 0.8919

RMSE: 2.82

Strong performance with minimal error, close behind Gradient Boosting.

3.Third Best Model: XGBoost Regressor

R² Score: 0.9058

RMSE: 2.63

Performed well but slightly less accurate than Random Forest.

4.Worst Performing Model: Decision Tree Regressor

R² Score: 0.6851

RMSE: 4.81

Struggled to capture the complexity of the data, with much higher error.

Conclusion:
Gradient Boosting Regressor was the best model for predicting Boston house prices.

Random Forest and XGBoost followed closely, offering strong predictive power.

Decision Tree was the least effective model for this task.

## Conclusion

The Gradient Boosting Regressor achieved the highest R² score, indicating it has the best performance in predicting Boston house prices.

The Random Forest Regressor and XGBoost Regressor also performed well, but Gradient Boosting had a slight edge.

The Decision Tree Regressor performed poorly compared to the other models, with a much lower R² score and higher error metrics.

