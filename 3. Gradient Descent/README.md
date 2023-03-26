Machine Learning Practice -- Day 3

Function Name: gradient_descent

Input:

x: numpy array. The input features.
y: numpy array. The target output.

Output:

m_curr: float. The slope of the best fit line.
b_curr: float. The y-intercept of the best fit line.

Function Description:
This function implements the gradient descent algorithm to find the best fit line for a given set of input features (x) and target output (y). It starts with an initial guess of slope (m_curr) and y-intercept (b_curr), and then iteratively updates these values to minimize the cost function. The cost function represents the difference between the predicted values of y and the actual values of y. The gradient descent algorithm updates the values of m_curr and b_curr in the direction of steepest descent of the cost function. The learning rate is a hyperparameter that determines the step size in the direction of the gradient. The algorithm stops when the change in cost function between successive iterations is very small.

Function Name: sklean

Input: None

Output:

model.coef*: float. The slope of the best fit line obtained using the Linear Regression model of sklearn library.
model.intercept*: float. The y-intercept of the best fit line obtained using the Linear Regression model of sklearn library.

Function Description:
This function reads the data from the 'test_scores.csv' file, and fits a linear regression model to the data using the Linear Regression model of sklearn library. The slope and y-intercept of the best fit line are returned as the output.
