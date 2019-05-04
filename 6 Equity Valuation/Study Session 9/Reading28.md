# Reading 28: Return Concepts

## Definitions of Return

- *Holding period* return is the increase in price of an asset plus any cash flow received, divided by the original price of the asset
$$
R_\text{holding period}=\frac{P_\text{final} + \text{CF}_\text{final}}{P_\text{initial}} - 1
$$
- *Required return* is the minimum return an investor requires given the nature of the asset
- *Internal rate of return* is the rate of return that equated discounted cash flows to current asset price
  - In an efficient market, the IRR and required return are the same
- If expected return exceeds required return, the asset is undervalued
  - This mispricing can lead to a *convergence* of price, as market participants try to exploit it, thus eliminating it and yielding a return
  - This convergence can be prevented by market inefficiencies, so calculating a mispricing does not guarantee a convergence yield
- Models used to estimate the required return on equity include:
  - CAPM:
$$
r_j = r_\text{rf} + r_\text{equity} \cdot \beta_j
$$
  - Multi-factor model:
$$
r_j = r_\text{RF} + \sum^n_{i=1} \text{risk premium}_i
$$
  - Fama-French model:
$$
\begin{aligned}
r_j& = r_\text{RF}\\
& + (r_\text{mkt prem} \times \beta_\text{mkt,j})\\
& + (r_\text{small-cap prem} \times \beta_\text{SMB,j})\\
& + (r_\text{value prem} \times \beta_\text{HML,j})
\end{aligned}
$$
  - The Pastor-Stambaugh model adds a liquidity factor to the Fama-French model
  - Macroeconomic multifactor models use macroeconomic variables as inputs
    - They are appropriate for use in any market in which public entities represent a sufficiently large share of the economy
  - Build-up models are similar to the multi-factor model, in that they do not use betas to adjust for exposure to a given factor
    - Build-up models are useful for thinly traded-companies, since they allow for adjustments on a firm-specific level
    - However, they use historical estimates, which means they depend on good availability of data
- A country-risk model allows the calculation of a risk premium associated with doing business in an emerging market
  - An analyst should being with a model from a developed country, then modify that model with inputs from an emerging market to derive an emerging market risk premium
- Each method has various strengths and weaknesses:
  - The CAPM is simple but has low explanatory power
    - The CAPM is a victim of *model uncertainty*, because it is unknown if its use is theoretically correct and appropriate
    - Furthermore, it is subject to input uncertainty because is it difficult to estimate the appropriate risk premiums accurately
    - Additionally, there is still debate over whether the arithmetic, or geometric means of market returns should be used
  - Multifactor models have more explanatory power but are more costly
  - Build-up models are simple and tailored to specific firms, but they are not forward-looking

## The Equity Risk Premium

- An *equity risk premium* is the additional return in excess of the risk-free rate that investors require in return for taking on the risk of equity securities
- There are four ways of estimating the equity risk premium:
  - A backward-looking estimate of the equity risk premium can be calculated by subtracting the mean return of a diverse equity index from the mean return on U.S. Treasury bills over a given time period
  - A forward-looking estimate uses more current information, but must be updated periodically
  - Macroeconomic models use current information, but they are inappropriate for jurisdictions where public equities do not represent a significant share of the economy
  - Survey estimates are simple to compile, but there can be a wide variation of opinions
- Models used to estimate the equity risk premium include:
  - Gordon growth model: 
    - The equity risk premium can be estimated as the one-year forecasted dividend yield on market index, plus the consensus long-term earnings growth rate, minus the long-term government bond yield
$$
r_\text{equity}=\frac{D_1}{P_0} + \text{earnings growth} - r_\text{rf}
$$
  - Ibbotson-Chen model:
$$
r_\text{equity} = (1 + \hat{i}) \times (1 + g_\text{EPS}) \times (1 + g_\frac{P}{E}) - 1 + r_\text{index} - r_\text{rf}
$$

## Beta Estimation

- A regression of returns on a stock with returns on an index provides an estimate of beta
  - There is a tendency for beta to drift towards one (or the industry average)
  - Beta can be adjusted for beta drift before use in the CAPM using the Blume method:
$$
\beta_\text{adj} = \frac{2}{3} \times \beta_\text{regression} + \frac{1}{3}
$$
- Beta can be estimated for thinly-traded stocks by following four steps:
  - Identify a publicly traded benchmark firm
  - Estimate $\beta_\text{benchmark}$ using a method such as a regression
  - Unlever the benchmark beta
  - Relever using the capital structure of the target firm