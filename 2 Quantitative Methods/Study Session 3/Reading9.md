# Reading 9: Correlation and Regression

## The Correlation Coefficient

- The *correlation coefficient* is a measure of the strength of the (linear) relationship between two variables
  - It can take values from -1 (perfectly negative correlation) and +1 (perfectly positive correlation)
  - A value of 0 indicates no correlation at all

- When testing the significance of a correlation coefficient, the test statistic is $t = \frac{r \sqrt{n - 2}}{\sqrt{1 - r^2}}$
  - Note that this test is two-tailed, with the confidence interval for a single correlation coefficient given by the positive and negative values of the value taken from the t-table

- To calculate the correlation coefficient from the covariance of two variables, use the following:
  $$
  r_{x,y=\frac{\text{cov}_{x,y}}{\sigma_x \sigma_y}}
  $$


## Regression Assumptions

- When performing a regression of two variables, the following assumptions are implicit:
  - A linear relationship exists between the variables
  - The independent variable is uncorrelated with the residual term (the error, or 'noise' term)
  - The expected value of the residual term is zero (positive and negative errors are equally likely, and cancel out with a sufficiently large sample)
  - The residual term is independently distributed (the error in one observation is not correlated with the error in another)
  - The residual term follows a normal distribution

## Confidence Internal for a Predicted Y-Value

- The confidence interval for a predicted Y-value is as follows:

$$
\text{confidence interval} =\text{predicted Y-value} \pm (\text{critical t-value}) \cdot (\text{standard error of forecast})
$$
