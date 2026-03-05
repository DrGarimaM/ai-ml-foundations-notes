# Linear Regression

Linear Regression is one of the simplest and most widely used machine learning algorithms for predicting numerical values.

It models the relationship between input variables (features) and an output variable (target) using a straight line.

## Basic Idea

The relationship is represented using the equation:

y = mx + b

Where:

y → predicted value  
x → input feature  
m → slope of the line  
b → intercept

## Example

Suppose we want to predict house price based on house size.

As house size increases, the price usually increases as well. Linear regression finds the best line that fits the data points and uses it to make predictions.

## If We Add Many Variables (Location, Floor, Facing etc.)

Yes — Linear Regression can handle multiple input variables.

This is called:

Multiple Linear Regression

Instead of: y=mx+b the problem becomes: Price = b0 + b1(Size) + b2(Location) + b3(Floor)+ b4(Layout) + b5(Facing)
Each variable contributes to the final prediction.

So the model learns how much each factor affects price.

Example interpretation:

--> size contributes most

--> location contributes second

--> facing contributes very little

This is actually one of the biggest advantages of linear regression:

It is interpretable.
## How the Model Learns

The algorithm adjusts the slope and intercept so that the distance between predicted values and actual values becomes minimal.

This is usually done using the Least Squares method, which minimizes the squared prediction errors.

## Applications

Linear regression is used in many domains:

Finance:
Sales forecasting

Healthcare:
Disease progression prediction

Telecommunications:
Network traffic prediction and demand forecasting

## Trainer Notes

Explain the concept using a scatter plot and a best-fit line.

Ask learners:
If the relationship between variables is not linear, will linear regression work well?
y = a + bx + cx²
Now the graph becomes curved, but the model is still linear in parameters.

This is called:

Polynomial Regression

So linear regression can approximate some nonlinear patterns.

But for very complex relationships we use:

Decision Trees

Random Forest

Neural Networks
## Can Linear Regression Produce Multiple Outputs?

Usually:

Linear regression predicts one output variable.

Example:

Inputs:
 Size
Location
Floor

Output:
Price

So:
Multiple inputs → One output
But There Is a Variant
Called Multivariate Regression or Multi-Output Regression.

Example:
Predict:
House price
Rental value
Property tax
from same inputs.

So:Multiple inputs → Multiple outputs--> But this is less commonly taught initially.
