# Reading 38: Credit Analysis Models

## Credit Risk Measures

- Probability of default is the probability that a borrower will fail to provide cash flows which they have committed to providing
- Loss given default is the loss that a lender will incur in the event that a borrower defaults
- Expected loss is the probability of default multiplied by the loss given default
- Present value of loss adjusts expected loss for time-value, and uses risk-neutral probabilities
  - The present value of expected loss is the difference between the value of a risk-free bond, and a risky bond

## Credit Ratings and Scores

- Credit ratings and scores are ordinal rankings of creditworthiness
  - They do not account for business cycle stage, in favour of being stable over time

## Structural Models of Corporate Credit Risk

- Structural models of corporate credit risk are based on the structure of a company's balance sheet and rely on insights provided by option pricing theory
- Holding stock in a company with risky outstanding debt can be viewed as a call option on the firm's assets
  - If the value of the assets exceeds the face value of the debt, the shareholders receive the difference remaining after debtholders are paid
  - If however, assets are insufficient to cover the debt, then the value of the stock is zero
  - This is why the minimum fair value of a firm's debt will simply equal the value of the assets at the point of maturity
  - The minimum value of stock however can fall to zero
- Debt investors can also be thought of as being short a put option on company assets
  - If assets are insufficient to cover the value of the debt, shareholders can "exercise the put option" to sell the assets at face value
- Structural models assume that company assets trade in a frictionless market with a mean return of $\mu$ and a variance of $\sigma^2$
  - The risk-free rate is assumed constant, and the balance sheet is assumed to be simple, in that it contains only a single issue of risky debt
- Appropriate for evaluating ABS risk as long as their complex structure is accounted for

## Reduced Form Models of Corporate Credit Risk

- Reduced form models do not impose assumptions on the balance sheet, instead imposing them on the output of a structural model
  - The inputs for reduced form models can be estimated using historical data, in a process called hazard rate estimation
  - Reduced form models assume that the firm has at least one issue of risky zero-coupon debt, with no restriction placed upon other liabilities
  - Risk-free rate, probability of default, and recovery rate, are all allowed to vary
- Input estimates are observable, allowing the use of historical estimation methods
  - Back-testing is still necessary
- Appropriate for evaluating ABS risk as long as their complex structure is accounted for

## Term Structure of Credit Spreads

- Credit spread is the difference between the yield of a risk-free bond, and of a risky bond
  - The term structure of credit spread illustrates how the spread varies with maturity

## Present Value of Expected Loss on a Bond

- The difference between the value of a risky bond and a risk free bond is the present value of the expected loss on the risky bond
  - This can also be understood as the maximum amount an investor would compensate an insurer for bearing the risk of the bond

## Asset Backed Securities

- ABS losses are borne by diffeent tranches of the ABS structure, based on the distribution of the waterfall, instead of simply defaulting
  - This means that credit analysis of asset backed securities requires evaluation of the collateral pool as well as the waterfall
  - Hence probability of default as a concept does not apply, instead "probability of loss" is used

## The Option Analogy

- If a hypothetical firm is financed by a mix of equity, and a single zero-coupon debt issue, then the value of the firm's assets is the sum of equity and debt
  - A shareholder owning the entirety of the firm's stock has the equivalent of a call option on the firm's assets, with a strike price equal to the value of the firm's debt
  - When the debt matures, if asset value exceeds the value of debt, the call is exercised, and the stockholder effectively buys the firm's assets, for the price of the firm's debt, keeping the residual
  - If, on the other hand, the value of debt exceeds assets, then the option expires worthless, and debtholders are left to cover the shortfall
- Similarly, owning the firm's debt is analogous to owning risk-free debt of the same value, as well as being short a put option on the firm's assets with a strike price equal to the value of debt
  - At maturity, the principal on the risk free bond is returned
  - However, if firm asset value is below the value of debt, then the put option is exercised, and the debtholder must pay the difference in return for the firm's assets
    - This leaves the debtholder with a loss equivalent to the difference in the value of firm assets, and the value of firm debt
  - If asset value is above the value of debt, then the debtholder has their principal returned, and the put expires worthless