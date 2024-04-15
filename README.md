# statistical_learning_linear_regression
Linear regression application with  the least squares library OLS, and  a comparison between the prediction outputs of the LR model and a KNN regressor


Simple linear Regression
- predicting a quantitative response Y based on a single predictor variable X. SLR assumes that there is a linear relationship between X and Y.
y = mX t c
we use the model to find estimates of m and c. Then we can make predictions on y values based on the estimation

m - slope/ gradient- average increase in Y associated with a one-unit increase in X.
c - intercept

RSS - residual sum of squares
1. Estimate the coefficients
- measuring closeness, minimizing the least squares criterion 
y^ = m^X + c^
e = y - y^

2. Assessing the accuracy of the coefficient estimates. (Hypothesis testing)
after finding the slope and the intercept, we assess how good they are

e is the quantity that shows that the true relationship between the terms is not linear

there is a sample mean and a population mean.  A sample is a subset of the population. Sometimes the sample mean is an overestimate of the population mean, sometimes it is an underestimate. A metric is used to estimate how much the sample mean deviates from the population mean.

STANDARD error and these standard errors are used to compute the confidence interval.
The standard errors are used to compute the hypothesis tests.

The null hypothesis says, there is no relationship between X and Y. Thus B1 =0. B1 is the slope

The alternate hypothesis says, there is a relationship between X and Y. B1 !=0

T-statistic 
p-value


- population regression line: line of best fit
- least squares line

confidence interval - A 95% confidence interval is defined as a range of values that has a 95% probability of containing the true unknown value of the parameter
Rejecting the null hypothesis allows us to conclude that there is a relationship between the response and the predictor

3. Assessing the accuracy of the model
Mean squared error

after rejecting the null hypothesis, quantify the extent to which the model fits the data
- Residual Standard error (RSE): an estimate of the standard deviation of e. The average amount by which the response will deviate from the true regression line. RSE is a measure of a lack of fit. if the predictions obtained are close to the true outcomes, RSE will be small. The absolute measure of a lack of fir

- R^2 statistic: takes on a value between 0 and 1. 

1- RSS/TSS 

TSS- total sum of squares: measures the inherent variability in the response  before the regression is performed

RSS - measures the unexplained variability in the response after the regression

R^2 value that is close to 1 indicates that a large proportion of the variability in the response is explained by the regression
0 means that regression does not explain the variability. this could happen because the model is wrong, or the error variance is high



 Non-parametric method - Does not assume a linear relationship between X and Y

KNN Regression
Given a value K and a prediction point x0, K identifies the training observations that are closest to x0, represented by N0. It estimates f(x0) using the average of all the training responses
A small value for k,
flexible fit
- low bias and high variance
Linear Regression with K-Nearest Neighbor

A large value for k 
smoother and less variable fit



1. Non-linearity: the residual plot is used to check for linearity. the residual plot is not supposed to have a pattern. If there is a pattern, then there is a problem  with the linear model.

if the residual terms exhibit  a strong U-shape, it is a strong indication of nonlinearity.

2. correlation of error terms
for linear regression, error terms are assumed to be uncorrelated
 if there is a correlation between the errors, the confidence and prediction intervals will be narrower than they should be

check if there is a correlation among the error terms. You can plot the residuals as a function of time, if the errors are uncorrelated, then there is no discernible pattern. if the errors are positively correlated then we may see tracking in the residuals

the correlation usually occurs among time series data.


3. Non-constant Variance of error terms
for a linear regression model, the error terms should have  a constant variance



