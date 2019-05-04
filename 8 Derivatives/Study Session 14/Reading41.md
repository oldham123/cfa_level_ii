# Reading 41: Valuation of Contingent Claims

## Put-Call Parity for European Options

$$
C_0 + \left(\frac{X}{(1 + R_f)^T }\right) = P_0 + S_0
$$

- The above can interpreted as "holding a call option and a riskless bond is equivalent to holding a put option and a stock"
  - The formula can be rearranged to determine other relations, where a positive value indicates a long position in the asset, and a negative value indicates a short position in the asset
- Since dividends cause the value of a stock to fall, this relation also shows how dividends cause the value of calls to fall, and of puts to rise

## The Binomial Option Pricing Model

- This model allows for "up-movements" and "down-movements" in stock prices
  - Option payoff is calculated in the event of both an up-movement and down-movement
  - The expected value of the option is the weighted average of all possible payoffs
  - This value is then discounted to the present
- When evaluating a tree of rates or prices, it should be noted that a rate holds for the branch *following*, not the branch preceding
  - This means that when discounting expected payoffs to the present, you should use the rate at the previous node
- Probabilities for up and down movements can be derived from the premise that the market has an inbuilt tendency to appreciate at the risk-free rate
  - Hence $U \cdot \pi_U + D \cdot (1 - \pi_U) = 1 + R_f$
  - Rearrangement yields the relation below:
$$
\pi_U = \frac{1+R_f-D}{U-D}
$$
where
$$
\begin{aligned}
\pi_U& = \text{risk neutral probability of an up-move}\\
\pi_D& = \text{risk neutral probability of a down-move}\\
U& = \text{stock price multiple of an up-move}\\
D& = \text{stock price multiple of a down-move}
\end{aligned}
$$

## Interest-Rate Options

- Interest-rate options are options on forward rates
  - The rates are fixed in advance at the beginning of the loan term
  - They are also settled in arrears, with payout occurring at maturity of the loan
    - This is why short-put, long-call interest rate options on periods 1, 2, and 3 and replicate uncertain swap payments on periods 2, 3, and 4
- The payoff of an interest-rate option is calculated as the benefit of being able to borrow (call options) or lend (put options) a notional principal at an exercise rate instead of the reference rate
  - An interest rate call pays off when the reference rate is above the exercise rate, since it represents the right to borrow the notional principal at below-market rate
    - Such a right leads to profit, since the holder can simultaneously lend the borrowed funds at the reference rate, and keep the difference
    - $\text{Interest-rate call payoff} = \text{principal} \times \text{Max}(0, r_\text{rf} -r_\text{exercise})$
  - An interest rate put pays off when the reference rate is above the exercise rate, since it represents the right to lend at an above market-rate
    - Such a right leads to a profit, since the holder can simultaneously borrow at the reference rate, and keep the difference
- A similar procedure can be used for interest-rate options
  - The risk-neutral probabilities of up or down movements are equal in this case
  - Expected values at the end of each potential path are discounted at the rates in the tree

## The Black-Scholes Merton Option Pricing Model

$$
\begin{aligned}
C_0 &= S_0\cdot N(d1) - X \cdot e^{-r^c T} \cdot N(d2)\\
P_0 &= X \cdot e^{-r^c T} \cdot N(-d2) - S_0 \cdot N(-d1) 
\end{aligned}
$$
where
$$
\begin{aligned}
d_1& = \frac{\text{ln}(\frac{S}{X})+(r+\frac{\sigma^2}{2}) \cdot T}{\sigma \sqrt{T}}\\
d_2& = d_1 - \sigma \sqrt{T}\\
T& = \text{time until option expiration}\\
r& = \text{continuously compounded risk-free rate}\\
S_0& = \text{current asset price}\\
X& = \text{exercise price}\\
\sigma& = \text{annual volatility of asset returns}\\
N(*)& = \text{cumulative standard normal probability}\\
N(-x)& = 1 - N(x)
\end{aligned}
$$

## Key Interpretations of the Black-Scholes Merton Model

- A call can be viewed as a leveraged investment in $N(d_1)$ worth of stock for every $e^{-rT}N(d_2)$ worth of borrowed funds
- A put can be viewed as $N(-d2)$ worth of bonds for every short position in $N(-d1)$ worth of stock
- $N(d_2)$ is the risk-neutral probability of a call option expiring in the money
- $N(-d_2)$ is the risk-neutral probability of a put option expiring in the money
- For dividend paying stocks, the benefit of carrying them offsets the cost of carrying them (the risk free rate) and increases the value of the call
- For options on currencies, the interest rate earned on the currency is the carry benefit
- The value of a call is positively related to the risk-free rate, whilst the value of a put is negatively related
  - This is because as $r^c$ increases, $e^{-r^c T}$ decreases

## BSM Assumptions and Limitations

- Assumptions and limitations of the BSM model include:
  - Return on the underlying asset follows a lognormal distribution
  - Price changes smoothly
  - The continuous risk-free rate is constant and known
  - The volatility and yield of the underlying asset is constant and known
    - This results in the BSM being a poor choice for pricing options, since volatility is a key variable in those calculations
  - Markets are frictionless 
  - The options are European
- The BSM model can be modified to deal with cash flows such as coupon payments or dividends
  - This is done by determining a continuously compounding yield

## Options On Futures

- The model can be used to value European futures by substituting $S_0$ for $e^{-r^c T} \cdot F_T$

## Equivalencies in Interest Rate Derivative Contracts

- Combinations of interest rate contracts can be used to replicate other contracts:
  - A long interest rate call and a short interest rate put can be used to replicate a long FRA (with $X = \text{current FRA})$
  - An interest rate call allows the owner to pay a fixed rate in return for floating payments, which pays off if the floating rate rises above the fixed rate
    - A series of these calls can be combined into an effective cap, since the payoffs received as a result of the higher floating rate compensate for the costs caused by higher rates
    - Writing a series of puts on fixed income securities is another method of synthesising a cap
  - An interest rate put allows the owner to pay a floating rate in return for fixed payments, which pays off if the floating rate falls below the fixed rate
    - A series of these puts can be combined into an effective floor, since the payoffs received as a result of the lower floating rate compensate for the costs caused by lower rates
    - A series of calls on fixed income securities is another method of synthesising a floor
      - These call options provide the right to buy fixed income securities at locked in prices that are lower than newly increased prices due to falling rates
  - A series of interest rate call options with different maturities and the same exercise price can be combined to form an interest rate cap
  - A long cap and a short floor can replicate a payer swap (if the exercise rate on each is the same)
  - If the exercise rate on a floor and a cap are both equal to the market swap fixed rate, then the values of each will be equal

## Swaptions

- A *payer swaption* is the right to enter into a specific swap at a future date as the fixed payer
  - If interest rates increase, the right to enter the pay-fixed side becomes more valuable
  - This is because the floating rate that one would receive would be getting further the above the fixed rate that one would need to pay in return
  - The reverse exists for *receiver swaptions*
- A long fixed-receiver swaption and a short fixed-payer swaption can replicate a receiver forward swap
- A callable bond can be replicated by a portfolio of a straight bond and a receiver swaption

## Inputs to the BSM Model

- There are five inputs to the BSM model:
  - Asset price $S_0$
  - Exercise price $X$
  - Asset price volatility $\sigma$
  - Time to expiration $T$
  - Continuously-compounded risk-free rate $r^c_f$

## The Greeks

- *The Greeks* are a group of sensitivity factors that capture the relationship between each input and the option price
  - *Delta* describes the relationship between changes in underlying asset prices and changes in option prices
    - Call option deltas are positive, put option deltas are negative
    - When the price of the underlying is very low, and a put option is deeply in the money (maximum payoff occurs when the price is zero), put option delta reaches a minimum bound of $-1$
      - This is because option value moves in the opposite direction of price
    - When the price of the underlying is very high, and a put option is far out of the money, put option delta reaches a maximum of $0$
      - This is because regardless of small movements there is very little chance that the put option will become valuable
  - *Gamma* measures the rate of change in delta as the underlying asset prices changes
    - Gamma is highest for at-the-money options
  - *Vega* measures the sensitivity of the option price to changes in the volatility of returns on the underlying asset
    - Options are more valuable when prices are more volatile
    - Vega increases as an option approaches the money 
  - *Rho* measures sensitivity of the option price to changes in the risk-free rate
    - Sensitivity to the risk-free rate is not high in general
    - Rho is positive for calls, and negative for puts
  - *Theta* measures the sensitivity of the option price to the passage of time 
    - As an option approaches expiration, the speculative value of the option declines
    - Deeply in-the-money options may get more value as expiration approaches

## Delta-Neutral Hedging 

*Delta-neutral portfolios* combine short call options with the underlying stock so that the value of the portfolio remains static as the underlying asset price changes 
$$
\text{\# of call options needed for delta-hedging} = \frac{\text{number of shares}}{\text{delta of call options}}
$$
- This only holds for small changes in price, so the portfolio must be continuously re-balanced
- In general, a delta-neutral portfolio should have a delta of 0
- Delta-neutral portfolios can also be constructed using put options by utilising the fact that $\delta_p = \delta_c - 1$

## Gamma Risk
- Gamma risk arises when the change in stock price is abrupt and discontinuous, rather than smooth 
  - This change will remove the hedging quality of delta-neutrality

## Implied Volatility in Options Trading 

- Implied volatility is that which yields the market price of an option when used in the BSM model
