# Reading 11: Time-Series Analysis

## Linear Trend Models

- A *linear trend model* takes the following form:
  $$
  y_t = b_0 + b_1(t) + \epsilon_t
  $$

  - $b_1$ gives the predicted change in $y_t$ for every unit change in time
  - These models make the assumtion that changes in the dependent variable can be explained purely by the progression of time
  - If data points are equally distributed above and below the trend line with a constant mean, then the model may be effective
  - Examples of good candidates for linear trend models include GDP growth and inflation

## Log-Linear Trend Models

- A *log-linear trend model* takes the following form:
  $$
  ln(y_t) = b_0 + b_1(t)
  $$

  - This model is most effective in cases where the dependent variable displays a trend for which residuals are correlated, or where the mean is not constant, for example most data related to investments
  - Additionally, data that displays seasonality, or exponential growth, is also a good candidate for this model type
  - The model is also appropriate for a variable that grows at a constant rate over time
  - Transforming the data results in a linear trend line, with increased predictive power
  - Serial-correlation is minimised by accurately capturing the behaviour of the data

## Serial Correlation

- Serial Correlation is the presence of correlation between residuals
  - Detecting the presence of serial correlation for an auto-regressive model should not use the Durbin-Watson statistic
  - The appropriate t-statistic to use is the estimated autocorrelation divided by the standard error, where the standard error is $\frac{1}{\sqrt{T}}$, where $T$ is the number of observations
  - The number of degrees of freedom is $T-2$

## Auto-regressive Models

- An *auto-regressive model* regresses a dependent variable against previous values of itself, and takes the following form:
  $$
  x_t = b_0 + \sum^p_{i=1} b_i \cdot x_{t-i} + \epsilon_t
  $$

  - For this type of model, specification requires no statistically significant autocorrelation
  - Testing for serial correlation should use a t-test, not the Durbin-Watson test

## The Chain Rule of Forecasting

- The *chain rule of forecasting* refers to multi-period forecasting using an auto-regressive model
  - Each successive period is forecast separately, with risk increasing with each forecast, as the data driving the estimate is further and further in the past

## Covariance Stationarity

- A time series is *covariance stationary* if both mean and variance are constant and finite, desirable properties

  - Additionally, covariance with leading or lagged values must be both constant and finite
  - The Dickey-Fuller test can be used to test for covariance stationarity
  - Most economic and financial relationships are not stationary, to a degree depending on the length of the series, as well as market conditions
  - For a first order auto-regressive model to be covariance stationary, the mean reverting level must be defined

- *Mean reversion* is the tendency of a variable to revert to its mean value over time

  - The mean reverting level for a first order auto-regressive model is $\frac{b_0}{1 - b_1}$

- If a series has a *unit root* it is not covariance stationary

  - If the lag coefficient is one, then the time series is said to have a unit root

  - In this case, the series will simply equate to a random walk

    - A *random walk* time series is one where the dependent variable is equal to itself in a previous time period, plus a random error
    - These series take the following form:

    $$
    x_t = b_0 + x_{t - 1} + \epsilon_t
    $$

    - If $b_0$ is non-zero, then the random walk is said to display a drift

- *First differencing* is a procedure that can eliminate a unit root from a time series

  - It is done by defining a new dependent variable that is equal to the original dependent variable, subtracted from itself in the next period, like so:
    - $y_t = x_t-x_{t-1} = (x_{t-1} + \epsilon_t) - x_{t-1} = \epsilon_t$

  - It should be noted that when using a model that has been first-differenced, the values it yields are estimates for the *change* in the original dependent variable, not estimates for the variable itself
  - The mean-reverting level of this series is 0, therefore it is covariance stationary

## Seasonality

- *Seasonality* is tested for by calculating the residual autocorrelations
  - To adjust for seasonality, and additional lag of the variable can be added to the model
  - If the adjustment is correct, the autocorrelations should no longer be statistically significant

## Assessing Forecast Accuracy

- *Root mean squared error* can be used to determine the predictive accuracy of an autoregressive model
  - The RMSE is the sqare root of the average squared error
- RMSE can also be used to evaluate out-of-sample forecasts
  - These are forecasts of values beyond the time series used to build the model

## Structural Change and Coefficient Instability

- Regression coefficients may not be consistent across time periods
  - Models using a long time series may provide additional statistical reliability
  - However, this increases the risk that the economic environment has changed during the period of time relevant to the model
- A structural change can be detected by investigating the plotted data, to see it can be divided into to two distinct behaviours
  - In this case, two distinct models must be used for each period, in order to determine if the time series has shifted
  - If so, using data only from the later period to design the model may produce more reliable results

## Cointegration

- Cointegration is the relation of two time series to the same macro variables, or their following of the same trend in a way that is not expected to change
  - In this case, the error term from regressing one on the other is covariance stationary, and the t-tests are reliable
  - The regression of series $y$ on series $x$ can be achieved thusly:

$$
y_T = b_0 + b_1 \cdot x_t + \epsilon
$$

- The Dickey-Fuller test can be used to test the residuals for a unit root
  - Critical t-values for the test can be calculated using the Engle and Granger method
  - If the null hypothesis is rejected then the series are cointegrated
- If one series is regressed onto another, both series should be checked for covariance stationarity
  - If both series are covariance stationary then the model can be relied upon
  - If neither series is covariance stationary then cointegration should be checked for
  - Otherwise, the model is not reliable

## Autoregressive Conditional Heteroskedasticity

- If the variance of residuals in one time period is dependent on the variance of residuals in another, then the time series in question is displaying autoregressive conditional heteroskedasticity
  - In this instance, the standard errors and hypothesis tests of the regression coefficients are not valid

$$
\hat{\epsilon}_t^2 = a_0 + a_1 \cdot \hat{\epsilon}^2_{t-1} + \mu_t
$$

- If $a_1$ varies significantly from zero, then the time series displays ARCH(1)
  - If ARCH errors are present, heteroskedasticity should be corrected for, otherwise the standard errors of the coefficients will be invalid
    - The appropriate way to perform this correction is either the method of generalised least squares, or the use of White-corrected standard errors
  - However, the presence of ARCH errors also enables the use of an ARCH model to predict residual variance in future periods

## Multicollinearity

- *Multicollinearity* occurs when independent variables are highly correlated with each other
  - This can lead to distorted standard errors, and unreliable coefficients
  - Note that *some* correlation is inevitable, but that high levels of correlation indicate a problem
- Multicollinearity is likely when the coefficients themselves appear to be insignificant, whereas the model taken as a whole does
- Multicollinearity can be dealt with by removing independent variables

