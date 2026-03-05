# Loss Functions and Model Error

In machine learning, models make predictions based on patterns learned from data. However, predictions are rarely perfect. Therefore, it is necessary to measure how far the predicted values are from the actual values.

Loss functions are used to quantify this difference between the predicted output and the true output.

## What is Model Error?

Model error represents the difference between the predicted value and the actual value.

Example:

Actual house price = 80 lakh  
Predicted house price = 75 lakh  

Error = Actual − Predicted = 5 lakh

A machine learning model attempts to minimize this error during training.

## What is a Loss Function?

A loss function is a mathematical function used to measure how well a machine learning model is performing.

It calculates the error between:

Predicted value (ŷ)  
Actual value (y)

The goal of training is to minimize this loss.

Lower loss means the model is making better predictions.

## Common Loss Functions for Regression

### 1. Mean Squared Error (MSE)

Mean Squared Error is one of the most widely used loss functions for regression problems.

Formula:

MSE = (1/n) Σ (y − ŷ)²

Where:

y = actual value  
ŷ = predicted value  
n = number of data points

The error is squared so that larger mistakes are penalized more heavily.

### 2. Mean Absolute Error (MAE)

Mean Absolute Error measures the average absolute difference between predicted and actual values.

Formula:

MAE = (1/n) Σ |y − ŷ|

This method is less sensitive to very large errors compared to MSE.

### 3. Root Mean Squared Error (RMSE)

RMSE is simply the square root of MSE.

Formula:

RMSE = √MSE

It expresses the error in the same units as the target variable.

## Why Squaring Errors is Useful

Squaring errors has two advantages:

1. Negative and positive errors do not cancel each other out.
2. Larger errors are penalized more strongly than smaller errors.

This helps the model focus on reducing large prediction mistakes.

## Example

Actual Values: 100, 120, 130  
Predicted Values: 95, 125, 128

Errors:  
5, -5, 2

Squared Errors:  
25, 25, 4

MSE = (25 + 25 + 4) / 3

The model training process attempts to adjust parameters so that this loss value becomes as small as possible.

## Role of Loss Functions in Training

During training, the machine learning algorithm:

1. Makes predictions
2. Calculates loss using a loss function
3. Adjusts model parameters to reduce the loss

This process repeats many times until the model converges to a good solution.

## Trainer Notes

Ask learners:

- Why is error squared in Mean Squared Error?
- What happens if very large prediction errors occur?
- Why might MAE sometimes be preferred over MSE?
