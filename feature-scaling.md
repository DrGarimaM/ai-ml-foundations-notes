# Feature Scaling

Feature scaling is a preprocessing technique used in machine learning to ensure that input variables (features) are on a similar scale.

In many datasets, different features may have very different ranges. If these differences are not handled properly, some variables may dominate the learning process.

## Example Problem

Consider a dataset used to predict house price.

| Feature | Example Value |
|-------|-------|
Size (sq ft) | 1500 |
Floor Number | 5 |
Location Code | 2 |

Notice that the numerical ranges are very different:

- Size may range from 500 to 3000
- Floor may range from 1 to 20
- Location codes may range from 1 to 5

Because machine learning algorithms work with numerical values, features with larger magnitudes may influence the model more strongly.

## Why Feature Scaling is Important

If features are not scaled:

- Variables with large numerical values may dominate the learning process.
- Model training may become unstable.
- Optimization algorithms may converge slowly.

Feature scaling helps ensure that all features contribute more fairly during model training.

## Common Feature Scaling Techniques

### 1. Min-Max Scaling (Normalization)

This method rescales feature values to a fixed range, usually between 0 and 1.

Formula:

X_scaled = (X - Xmin) / (Xmax - Xmin)

Example:

Size = 1500  
Scaled Size = 0.65

Min-max scaling preserves the shape of the original distribution while adjusting the scale.

### 2. Standardization (Z-score Scaling)

This method transforms features so that they have:

Mean = 0  
Standard Deviation = 1

Formula:

X_scaled = (X - Mean) / Standard Deviation

Standardization is commonly used in many machine learning algorithms.

## Algorithms That Require Feature Scaling

Some machine learning algorithms are sensitive to feature scale, including:

- Linear Regression (when using gradient descent)
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machines (SVM)
- Neural Networks

These algorithms rely on distance calculations or gradient-based optimization.

## Algorithms That Usually Do Not Require Scaling

Tree-based algorithms generally do not require feature scaling:

- Decision Trees
- Random Forest
- Gradient Boosted Trees

These algorithms split data based on thresholds rather than distances.

## Example from Telecommunications

Consider a dataset for predicting network congestion with the following features:

| Feature | Range |
|------|------|
Signal Strength (dBm) | -110 to -40 |
Bandwidth Usage | 0 to 1000 Mbps |
Number of Users | 1 to 500 |

Without feature scaling, variables like bandwidth usage may dominate the learning process due to their larger numerical range.

Scaling helps ensure that all features contribute appropriately to the model.

## Trainer Notes

Ask learners:

- Why might features with large numerical values influence model training more strongly?
- Which machine learning algorithms require feature scaling?
- Why do tree-based models generally not need scaling?
