# Reading 52: Algorithmic Trading and High-Frequency Trading

## Algorithmic Trading

- Execution algorithms break large orders down into smaller pieces that are then strategically executed to minimise negative price impacts
  - Volume-weighted average price algorithms split an order into pieces that are sized according to the normal trading pattern of the security in question
  - Implementation shortfall algorithms continually adjust trade execution speed and as market conditions change in an attempt to minimise the difference between the price on which the trade was decided, and the price at which the trade settles in the market
  - Market participation algorithms try to match the pace of overall trading of the security
- High-frequency algorithms trade repeatedly using real-time rapidly updated market data to identify market inefficiencies and sources of profit
  - Statistical arbitrage algorithms trade securities that have historically moved together, in the hope of profiting from their convergence after a divergence in price
  - Liquidity aggregation and smart order routing algorithms send orders to whichever market has the best combination of price and liquidity, or by spreading the order over multiple markets to benefit from their combined liquidity
  - Real-time instrument pricing algorithms attempt to derive instantaneous price and liquidity information from the market itself
  - Trade on news algorithms react to breaking stories or releases of new economic data
  - Genetic tuning involves the evolutionary selection of profitable strategies

## Market Fragmentation

- Market fragmentation refers to the trading of a security across multiple markets, leading to one market only representing a fraction of the total liquidity available
- Liquidity aggregators develop a "super book" that sums the liquidity for a security across all markets

## Technology in Risk Management

- Methods of mitigating the risk of algorithmic trading include:
  - Real-time-trade risk firewalls, which calculate risk exposures on trades constantly to ensure that risk limits are not exceeded
  - Backtesting and simulations provide information on how an algorithm would have reacted in response to hypothetical or historical scenarios
- Regulatory oversight can benefit from real-time market monitoring to identify unusual market movements

## Suspicious Trading Practices

- Insider trading
  - Trading with the benefit of material, non-public information
- Front running
  - Trading with advance knowledge of a large pending transaction
- Painting the tape
  -  A group of traders may trade a security amongst themselves to increase trading activity, and the market price, before selling the security on to unsuspecting investors attracted by the spike in activity for a profit
- Quote stuffing
  - Entering large numbers of orders and then cancelling them
- Quote layering / spoofing
  - Placing legitimate orders on one side of the market, and fictitious orders on the other side
- Wash trading
  - Involves an investor buying and selling the same instrument simultaneously, in order to artificially boost trading volume