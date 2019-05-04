# Reading 48: An Introduction to Multifactor Models

## Arbitrage Pricing Theory

- The APT is based on the notion of an equilibrium relationship between expected returns for a portfolio that is diversified, and its multiple sources of systematic risk
- The APT makes three underlying assumptions:
  - Unsystematic risk can be diversified away
  - Returns are generated according to a factor model
  - Arbitrage opportunities do not exist

## Arbitrage Opportunities

- An arbitrage opportunity represents the ability to make an investment that generates profit at zero risk to the investor
- Arbitrage opportunities are exploited by using the proceeds of a short portfolio to finance the purchase of a long portfolio
  - Additionally the factor sensitivities of the portfolios are identical, resulting in a net exposure to the market of zero, with the difference in returns being pure profit

$$
\text{expected return} = \text{risk free rate} + \Sigma\beta \times \text{factor risk premium}
$$

## Macroeconomic Factor Models, Fundamental Factor Models, and Statistical Factor Models

- A multifactor model generates forecasted returns as a function of multiple factors
  - Macroeconomic models assume that asset returns are best explained by shocks in macroeconomic variables
    - A factor surprise is the difference between the true value and consensus expectations of the value
  - Fundamental factor models explain asset returns as a function of multiple firm-specific ratios
  - Statistical models use multivariate statistics to identify variables that explain covariation amongst asset returns
    - However, they may not lend themselves well to economic interpretation

## Sources of Active Risk

- Active return is the difference between the returns of a portfolio, and those of a benchmark
- Active risk is the standard deviation of active return
- $\text{(Active risk)}^2 = \text{active factor risk} + \text{active specific risk}$
- $\text{Active specific risk} = \sum^n_{i=1}(W_\text{pi} - W_\text{bi})^2\sigma^2_{\epsilon i}$

## Tracking Risk and the Information Ratio

- The information ratio gives the amount of active return per unit of active risk

## Multifactor Model Uses and Outputs

- Multifactor models can be used to aid in attributing risk and return to various sources, and to aid in portfolio composition
  - An active manager can go long or short a factor portfolio, which has a factor sensitivity of one to a particular factor, and zero to all others, hence representing a pure bet on a single factor
- The difference between portfolio and benchmark return is allocated between factor return and selection return
- Multifactor models allow the curation of portfolios to increase exposure to specific risks that an investor can bear, and to limit exposure to other risks