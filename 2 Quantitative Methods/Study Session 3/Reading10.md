# Reading 10: Multiple Regression and Issues in Regression Analysis

## Assessing a Multiple Regression Model

- Evaluating a multiple regression model involves the following procedure:

  1. Check that the model is correctly specified
  2. Check that the individual coefficients are statistically significant, using a t-test
  3. Check that the model is statistically significant, using an F-test
  4. Check for heteroskedasticity
     1. If present, check whether it is conditional, using the Breusch-Pagan Chi-Square test
     2. If conditional, use White-corrected standard-erros
  5. Check for serial correlation, using the Durbin-Watson test
     1. If present, use the Hansen method to adjust the standard errors
  6. Check for significant multicollinearity
     1. If present, remove one of the correlated variables from the model

- Assessing the statistical significance of an individual regression parameter is done using a t-test

- An F-test is used to assess the explanatory power of the model as a whole

- A typical regression model typical has the following form:
  $$
  Y_i = b_0 + (b_1 \times X_{1i}) + (b_2 \times X_{2i}) + (b_3 \times X_{3i}) + \epsilon_i
  $$

- When applying a multiple regression model, an estimated value for each independent variable should be used, regardless of whether the correlation is statistically significant for that variable

## Testing Multiple Regressions

- Testing a multiple regression model involves:
  - Testing the explanatory power of each individual independent variable using a t-statistic
    - The t-statistic to be used is given by $\frac{\text{coefficient estimate} - \text{hypothesised value}}{\text{standard error}}$
    - The confidence interval for such a test is given by $\text{coefficient estimate} \pm t_c \times S_e$
    - The critical value to be used in assessing a hypothesis is simply $\pm t_c$
  - Testing the effectiveness of the entire model in explaining variation in the dependent variable using an F-statistic
- In a multiple regression model, the critical t-statistic is distributed with $n-k-1$ degrees of freedom, where $n$ is the number of observations and $k$ is the number of independent variables
- ANOVA assigns the change in the dependent variable to either:
  - The regression model
  - The residuals
- An ANOVA table features the following measures:
  - RSS, the regression sum of squares
  - SSE, the sum of squared errors
  - SST, the total sum of squares, given by $\text{SSE} + \text{RSS}$
  - MSR, the regression sum of squares divided by $k$
  - MSE, the sum of squared errors divided by $n - k - 1$
  - Variance in the dependent variable is given by SST divided by $n - 1$
  - SEE, the standard error of estimate is given by $\sqrt{MSE}$, and is a measure of the uncertainty of the values of the dependent variable (this value is also the standard deviation of the residuals)
  - $R^2$ is the coefficient of determination (the percentage of the variation in the dependent variable explained by the independent variables)

$$
R^2 = \frac{\text{regression sum of squares}}{\text{total sum of squares}}
$$

- For a simple linear regression, the correlation $r_{x,y}$ between the dependent and independent variables is $\sqrt{R^2}$
- For a multiple regression, $\sqrt{R^2}$ gives the correlation between the actual and predicted values of the dependent variable
- Adjusted $R^2$ indicates the effectiveness of the model in a way that accounts for the number of independent variables
- The F-statistic used when testing the model in its entirety is given by $F=\frac{\text{MSR}}{\text{MSE}}$
  - Rejection of the null hypothesis indicates that at least one of the coefficients is significantly different from zero

## Confidence Intervals

- The confidence interval for a regression coefficient in a multiple regression is the same as in a simple regression
- The the confidence interval straddles the value zero, then the slope of the regression is insignificant

## Potential Problems in Regression Analysis

- Conditional heteroskedasticity is when the variance of the residuals is related to the number of independent variables in the regression
  - This leads to unreliable standard errors
- Serial correlation occurs when residual errors of different observations are corellated with each other
  - This leads to Type I errors
- Multicollinearity occurs when independent variables are correlated with each other
  - This causes too many Type II errors, and unreliability of slope coefficients

## Model Misspecification

- Model misspecification can involve any of the following:
  - Omitting a variable
  - Transforming a variable
    - Note that transforming a variable may also be a valid operation to improve the model, using a log-linear trend for example
  - Incorrectly pooling data
  - Using a lagged dependent variable as an independent variable
  - Forecasting the past
  - Measuring independent variables with error
- Misspecification causes regression coefficients to be biased, and inconsistent

## Heteroskedasticity

- Heteroskedasticity occurs when the variance of the residuals is not constant across all observations
  - Unconditional heteroskedasticity occurs when the level of heteroskedasticity is unrelated to the values of the independent variables
    - This usually causes no major problems with the regression
  - Conditional heteroskedasticity is when the level of heteroskedasticity *is* related to the values of the independent variables
- Conditional heteroskedasticity has the following effects:
  - Standard errors as usually unreliable
    - This has knock-on effects for t-statistics
  - The F-test is also unreliable
- Conditional heteroskedasticity can be detected through the use of a Breusch-Pagan chi-square test
  - The test statistic is $n \times \text{R}^2$
    - The $\text{R}^2$ used here is from a second regression of the squared residuals, from the first regression on the independent variables
  - The test has $k$ degrees of freedom
- Conditional heteroskedasticity can be corrected for using either:
  - The method of generalised least squares
  - White-corrected standard errors

## Serial Correlation

- Serial correlation is the correlation of residual terms with each other
  - Positive serial correlation occurs when a positive error in one time period increases the likelihood of a positive error in the next
  - Negative serial correlation occurs when a positive error in one time period increases the likelihood of a negative error in the next
- Serial correlation causes standard errors to be too smal
  - This leads to large t-statistics, implications of greater statistical significance, and thus more Type I errors (rejections of true null hypotheses)
  - F-tests also lose reliability since MSE will be too small
- Serial correlation can be detected using a Durbin-Watson statistic, roughly equal to $2(1-r)$, where $r$ is the correlation coefficient for residuals
- Serial correlation can be dealt with through the use of the Hansen method
  - If serial correlation and conditional heteroskedasticity are both present, then the Hansen method can correct for both