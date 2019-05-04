# Reading 42: Derivative Strategies

## Modifying Portfolio Risk and Return

- Combining a bond portfolio with a payer swap reduces the duration of the portfolio, changing its interest rate risk
  - Short bond futures can also reduce duration
- Equity swaps can be used to gain equity exposure 
- Currency swaps provide access to favourable financing in otherwise expensive FX markets

## Replicating an Asset Using Derivatives 

- A long futures contract on a stock, combined with a risk-free asset replicates a long stock position
- A protective put is the same as a long call, whilst a short put is the same as a covered call
- These positions can be derived using put-call parity
  - When doing so, the bond represented by $\text{PV}(X)$ can be disregarded since it is inconsequential when considering the impact of changes in the stock price 
- A call on EUR (vs. USD) is equivalent to a put on USD (vs. EUR)

## Covered Call 

- A covered call option strategy is a long position in a stock combined with a short call
  - This holding is usually for income generation, improving on the market, or target price realisation
- The risk of a covered call is the opportunity cost of giving up on the upside of the long stock position when the stock prices rises above the exercise price (and the long exercises the option)
  - The maximum possible gain is $X - S_0 + C_0$
  - The maximum loss is $S_0 - C_0$ 
  - The breakeven point is $S_0 - C_0$ 

## Protective Put 

- A protective put position involves a long stock and a long put
  - It can be considered akin to an insurance policy, where the put premium is the insurance premium, and the difference between the initial stock price and the exercise price representing the deductible
  - The maximum gain is $S_T - (S_0 + P_0)$
  - The maximum loss is $(S_0 - X) + P_0$ 
  - The breakeven point is $S_0 + P_0$ 

## Strategy Delta

- Covered calls and protective puts can be used to reduce the delta of a long stock position
  - Delta for a non-dividend paying stock is one
$$
\begin{aligned}
\text{covered call delta } = \text{delta of stock } - \text{ delta of call option}\\
\text{protective put delta } = \text{delta of stock } + \text{ delta of put option}
\end{aligned}
$$
## Bull and Bear Spreads

- Bull and bear spreads spread can be established using either calls or puts
  - The exercise price of the long option must be lower than that of the short to make a bull spread
  - The converse is true for a bear spread
  - A bull spread provides limited upside if prices rise, and limits downside if they fall, by combining a long call (lower exercise) with a short call (higher exercise)
    - If prices rise, then the payoff is the difference between the selling price in the short call, minus the (lower) buying price in the long call (option premiums must also be accounted for)
    - If prices fall, then both options expire worthless, leading to a loss of the net value of the option premiums
  - A bear spread provides limited upside if prices fall, and limits downside if they rise, by combining a long put (higher exercise) with a short put (lower exercise)
    - If prices fall, then the payoff is the difference between the selling price of the long put, minus the (lower) selling price of the short put (option premiums must also be accounted for)
    - If prices rise, then both options expire worthless,. with a loss equal to the net value of the option premiums
- For a bull spread:
  - Maximum profit is $X_H - X_L - C_{L0} + C_{L0}$
  - Maximum loss is $C_{L0} - C_{H0}$
  - Breakeven price is $X_L + C_{L0} - C_{H0}$
- For a bear spread:
  - Maximum profit is $X_H - X_L - P_{L0} + P_{H0}$
  - Maximum loss is $P_{L0} - P_{H0}$
  - Breakeven price is $X_L + P_{L0} - P_{H0}$

## Collars and Straddles

- A combination of a covered call and a protective put is a *collar*
  - The owner of a stock, purchases a put, using proceeds from selling a call
    - If the price rises, then the investor sells the stock, either buy exercising the put, or by having the call exercised, generating a payoff equal to the difference in stock purchase price and the exercise price of the used option
    - If the price falls, then the investor exercises the put, making a loss equal to the difference in stock purchase price and put exercise price
  - They limit upside and downside risk
  - Maximum profit is $X_H - S_0 - (P_0 - C_0)$
  - Maximum loss is $S_0 - X_L + (P_0 - C_0)$
  - Breakeven price is $S_0 + (P_0 - C_0)$
- A long straddle consist of a long call and a long put with the same strike price, on the same underlying stock
  - If the price rises then the investor can exercise the call and purchase the stock for the exercise price, then sell at a profit without exercising the put
  - If the price falls then the investor can purchase the stock without exercising the call, then exercise the put
  - Maximum profit is $S_T - X - (C_0 + P_0)$
  - Maximum loss is $C_0 + P_0$
  - Breakeven price is $X - (C_0 + P_0)$ and $X + (C_0 + P_0)$

## Calendar Spreads

- A long calendar spread includes two call options with different expiration dates
  - A long spread is a bet on a future rise, whilst a short spread is a bet on a future fall
  - The near-dated call is shorted, and the longer-dated call is long
  - These are used when volatility is expected to change 

## Investment Objectives

- Strategies employed should be consistent with expected market direction, and expected volatility
- Strong bullish sentiment can be expressed through long calls, with bearish sentiment expressed through long puts
- Moderate bullish sentiment can be expressed through long calls and short puts, and moderate bearish sentiment can be expressed through short calls

