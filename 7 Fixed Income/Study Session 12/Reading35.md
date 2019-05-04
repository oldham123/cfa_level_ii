# Reading 35: The Term Structure and Interest Rate Dynamics

## Spot Rates and Forward Rates

- The spot rate for a given maturity is the geometric average of the current one-period spot rate, and a series of one-period forward rates
- The spot rate curve indicates expectations of future rates
  - Upward sloping  - Forward rate curves will be above the spot curve
    - Hence, the yield for a maturity of $T$ will be less than the sport rate $S_T$
- The $A$-year forward rate, $B$ years from now can be calculated from the $(A+B)$ and $B$ year spot rates
  - $1 + f(A,B) = \left(\frac{1 + S_{(A+B)}}{1 + S_B}\right)^\frac{1}{A}=\left( \frac{P_B}{P_{(A+B)}}\right)^\frac{1}{A}$

## Evolution of Spot Rates Relative to Forward Rates

- If forward rates represent a good prediction of the future movement of spot rates, bonds of any maturity will provide a one-period return equal to the one-period sport rate
  - This will leave forward rates unchanged
- If an investor believes that spot rates will be lower than the corresponding forward rates (and is correct), then a profit can be made by purchasing bonds
- Volatility in short-term rates is mostly linked to monetary policy
- Volatility in long-term rates is mostly determined by uncertainty about the real economy and inflation

## Riding the Yield Curve

- Maturity matching is a normal strategy for a bond investor, where they purchase bonds with a maturity equal to their investment horizon
  - If the yield curve is sloping upward, an investor can purchase bonds with longer maturities for lower prices
  - As the bond approaches maturity it is valued using successively lower yields, hence increasing its price
  - The bond can then be sold at the end of the investor's investment horizon, generating an additional return

## The Swap Rate Curve

- The swap rate curve is a benchmark measure of interest rates, where the rates used represent the swap fixed rates of interest rate swaps
  - Swap rates reflect the credit risk of commercial banks, not governments
  - Since they don't reflect sovereign credit risk, they are more comparable across countries
  - The swap market is less regulated
  - The swap curve has yields quoted at more maturities
  - Retail banks tend to have little exposure to swaps and hence are more likely to use the government spot rate
- The swap spread is the additional interest paid by the fixed-payer in a swap over the rate of a government bond of the same maturity

## The Swap Spread

- The swap spread is the difference between the swap fixed rate, and the rate on a Treasury bond of equal maturity

## The Z-Spread

- The Z-spread, when added to each spot rate on the yield curve, makes the present value of a bond's cash flows equal the market price
- There is an implicit assumption that interest rates have no volatility

## The TED Spread

- The TED spread is computed by subtracting the Treasury yield from the LIBOR yield, and hence it is expected to be positive due to higher implied risk in LIBOR relative to sovereign debt
- This spread is used as an indicator of the overall level of credit risk in an economy

## The LIBOR-OIS Spread

- The LIBOR-OIS spread is the difference between the LIBOR rate and the overnight indexed swap rate
- This spread is another useful measure of credit risk

## Theories of the Term Structure of Interest Rates

- *Unbiased expectations* theory suggests that forward rates are an unbiased predictor of future spot rates
- *Local expectations* theory suggests that over long periods, risk premiums should exist, meaning that over short periods every bond should earn the risk free rate
- *Liquidity preference* theory suggests that investors require a liquidity premium that is related to a bond's maturity
  - This liquidity premium is in addition to investor expectations of what future rates should be
  - Note that whilst this theory implies that there is a risk premium attached to bonds of longer maturities, this yield curve can still have any shape
- *Segmented markets* theory suggests that the shape of the yield curve is the result of the interactions of supply and demand for funds in different maturity segments
  - This is supported by the assumption that investors will refuse to move into other maturity markets
- *Preferred habitat* theory suggests that market participants will leave their preferred market segments if compensated

## Modern Term Structure Models

- Cox-Ingersoll-Ross
  - $dr = a(b-r)dt + \sigma \sqrt{r} dz$
  - This model implies that there is a stable interest rate that rates revert to in the long run
- Vasicek
  - $dr = a(b-r)dt + \sigma dz$
  - A small change to Cox-Ingersoll-Ross that removes the relation between volatility and short-term rates
- Ho-Lee
  - $dr_t = \theta_tdt+\sigma dz_t$
  - This model assumes that the market is efficiently and correctly setting prices
  - The model is then calibrated using current prices to deduce a *drift term* that defines the current term structure
- Since Ho-Lee is the only model that is calibrated to replicate the prices seen in the market, the other two models can produce results that diverge from reality

## Managing Bond Exposure to the Factors Driving Yield

- *Effective duration* is the sensitivity of bond prices to parallel shifts in the benchmark yield curve
- *Key rate duration* measures bond price sensitivity to changes in a specific par rate