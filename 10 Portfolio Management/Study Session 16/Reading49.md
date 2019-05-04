# Reading 49: Measuring and Managing Market Risk

## Value At Risk

- Value at risk estimate the minimum loss that, with a given probability over a given period, will occur, expressed as either a cash amount, or a percentage of portfolio value
- Methods of VaR estimation include:
  - Parametric methods that use estimated variances and covariances of securities within a portfolio to estimate the distribution of possible portfolio values
  - Historical simulations that use historical values for risk factors over some prior lookback period to generate distributions of possible values
  - Monte Carlo simulations that draws values for each risk factor from an assumed distribution and calculates portfolio values based on a set of changes in those factors, repeated thousands of times to generate a distribution of possible portfolio values
- VaR estimates use the following convention:
  - "5% Annual VaR is -14%" indicates that there is a five percent chance of the portfolio decreasing in value by fourteen percent over the course of a year
- Advantages of VaR estimates include:
  - Wide acceptance by regulators
  - Simple to interpret
  - Useful for comparison
- Disadvantages of VaR estimates include:
  - Discretion over the probability and time period analysed introduces subjectivity
  - Very sensitive to the method of estimation used
  - Focuses only on "left-tail" outcomes
  - Vulnerable to misspecification error
- VaR is calculated by determining the value that is a given number of standard deviations below the mean return for the time period in question
  - For a five percent annual VaR, the estimate would be the value that is 1.65 standard deviations below the mean annual return
  - A VaR for one time period can be calculated for another by adjusting the mean and standard deviations
    - An annual mean can be converted into a daily mean by dividing by the number of annual trading days
    - An annual standard deviation can be converted into a daily standard deviation by dividing by the square root of the number of annual trading days

## Extensions of VaR

- *Conditional VaR* is the expected loss, given that the loss exceed VaR
- *Incremental VaR* is the estimated change in VaR caused by a given change in the size portfolio position
- *Marginal VaR* is the estimated change in VaR for a small change in a portfolio position, used also as an estimate of the position's contribution to overall VaR
- *Ex-ante tracking error* or *relative VaR* is the difference between the portfolio and benchmark returns

## Managing Market and Volatility Risk Using Options Exposure Measures

- Equity risk is measured by $\beta$
- Interest-rate risk is measured by duration (sensitivity to changes in yield) and convexity
- Options risk is measured by delta, gamma, and vega
- Market risk can be managed by adjusting holdings to alter exposure to each of these factors

## Sensitivity and Scenario Risk Measures

- A stress test uses extreme changes to examine the likely effects on a portfolio or an organisation
  - A reverse stress test is designed to identify the scenario that will lead to business failure
  - A stress test may be used to determine the  firm's economic capital, the capital needed to overcome severe losses in the business
- Sensitivity analysis can provide a better perspective of the vulnerability of a portfolio to multiple risk factors, but do not provide probabilities, or in the case of sensitivity analysis, the sizes of expected changes

## Unique Benefits of VaR, Scenario, and Sensitivity Risk Measures

- VaR estimates provide a probability of loss
- Sensitivity measures express the relative exposures to different risk factors
- Scenario measures describe exposure to simultaneous changes in multiple risk factors

## Risk Measures Used by Various Institutions

- Banks:
  - Market risk for investment portfolios
  - Leverage
  - Duration and convexity
- Asset managers:
  - Returns volatility
  - Probability distribution of absolute or relative losses
- Pension fund managers:
  - Surplus volatility
- Property and casualty insurers:
  - Sensitivity to risk factors
  - VaR
  - Stress test results
- Life insurers
  - Stress test results
  - Surplus volatility
  - VaR

## Constraints Used in Managing Market Risk

- Risk budgeting involves allocation portions of a total 'risk budget' across investment positions to generate maximum returns
- Position limits prevent positions from exceeding cash amounts, or percentages of total portfolio value being allocated to individual securities, a security class, or securities of a specific issuer
- Stop-loss limits require position reductions once losses exceed a given amount in a given time period
- A scenario limit prohibits positions that entail expected losses that exceed a specified amount in a given scenario