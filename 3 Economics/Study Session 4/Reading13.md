# Reading 13: Currency Exchange Rates - Understanding Equilibrium Value

## Currency Cross Rates

- A *cross rate* is the rate of exchange between two currencies that is implied by their exchange rates with a common third currency
- Currency cannot be sold for a better price than for which it was bought, due to the *bid-ask spread*
- Arbitrage can be possible if implied cross rates fall outside bid-ask spreads
  - The three currencies in the cross spread relationship form a triangle around which one can proceed in one of two ways, given a starting currency
  - One can check if either path yields an arbitrage profit
  - The implied cross rates can help deduce whether a dealer is overvaluing, or undervaluing a currency, which can be a clue to which way around the triangle will yield a profit

  ## Mark to Market Value of a Forward Contract

- *Mark-to-market* value reflects the profit that is realised if a forward contract position to buy base currency at a future time is closed at current prices
  - This is done by offsetting the position by another that is equal and opposite
  - For example, a long CAD contract (to buy CAD), priced in AUD with a size of 1 million, would be offset with a short CAD contract, priced in AUD of 1 million
  - The results of the offsetting contract can be used to settle the original contract
  - Note that forward prices are often given in terms of a change to the spot rate in basis points
$$
V_t = \frac{(FP_t - FP)\cdot(\text{contract size})}{1 + R\left(\frac{\text{days}}{360}\right)}
$$

where:
$$
\begin{aligned}
V_t& = \text{value of the contract at time }t\text{ to the currency buyer}\\
FP_t& = \text{forward price to sell the same amount of base currency at time of expiry }T\\
\text{days }& = \text{days remaining until contract maturity }(T - t)\\
R& = \text{interest rate of the price currency}
\end{aligned}
$$
## International Parity Conditions

- *Covered interest rate parity* is when differences in interest rates are offset by forward premiums or discounts
  - This ensures identical returns when investing in either currency, and therefore holds by arbitrage
- *Uncovered interest rate parity* is when the expected change in spot prices is reflected by differences in interest rates
  - $E( \% \Delta S)_{\frac{A}{B}}=R_A - R_B$
  - This holds if forward rates are unbiased predictors of future spot rates
- *Real interest rate parity* suggestions that real interest rates should converge to the same level across different markets
- *Absolute purchasing power parity* holds that a given basket of goods should cost the same globally, when accounting for exchange rates
  - This does not hold due to other factors such as uniformity of goods and services, and transportation costs
- Covered interest rate parity can be used to determine forward rates (assuming no arbitrage)
  - Uncovered interest rate parity cannot, since it is related to the expected future spot rate, which is not actively traded
- The *International Fischer relation* relates expected inflation rates in two countries, and the difference in their interest rates
  - $R_A-R_B = E(\text{inflation}_A)-E(\text{inflation}_B)$
- *Relative purchasing power parity* is when changes in exchange rate offset the impacts of differences in inflation
  - Whilst this relation fails to hold in the short run, it does hold in the long run
  - $\%\Delta S_\frac{A}{B}=\text{inflation}_A - \text{inflation}_B$
- The International Fischer relation and relative purchasing power parity can be combined to give uncovered interest rate parity

## FX Carry Trades

- *FX Carry Trades* seek to profit from uncovered interest rate parity not holding in the short run
  - They involve borrowing in a low-yield currency, and investing in a high-yield currency
  - If the expected change in spot prices fails to occur, then there is a profit
- FX Carry Trades are leveraged and exposed to crash risk, with non-normal return distributions exhibiting negative skewness and excess kurtosis

## Balance of Payments Analysis

- *Flow mechanism*
  - Current account deficits encourage currency depreciation
  - This may eliminate the deficit, depending on the starting deficit, the importance of exchange rates on prices, and the price elasticity of demand of traded goods
- *Portfolio composition mechanism*
  - Investor country portfolios may be dominated by countries with capital account surpluses
  - If and when their portfolios are rebalanced, there may be a resulting currency depreciation for the investee countries
- *Debt sustainability mechanism*
  - A country with a current account deficit may have a capital account surplus by borrowing from abroad
  - If the level of debt gets too high there may be a crisis of confidence, leading to rapid depreciation

## Effects of Monetary and Fiscal Policy On Exchange Rates

- *Mundell-Fleming model*
  - The effects of monetary and fiscal choices on exchange rates depend on whether capital mobility is high or low
    - If it is high:
      - Complimentary monetary and fiscal policies (both expansionary or both restrictive) have uncertain effects
      - If policies are opposing, fiscal policy choice will dominate (i.e. restrictive &rarr; depreciation)
    - If it is low:
      - Opposing monetary and fiscal policies (one expansionary and one restrictive) have uncertain effects
      - If policies are complimentary, currency will tend to move in the opposite direction (i.e. expansionary &rarr; depreciation)
- *Pure monetary model*
  - Assumes that PPP holds, and therefore that expansionary monetary policy causes inflation, and currency depreciation
- *Dornbusch overshooting model*
  - Restrictive monetary policy causes significant appreciation in the short run, and then slow depreciation, until the long run PPP value is reached
- *Portfolio balance model*
  - States that a running a fiscal deficit leads to increased borrowing, and eventual currency depreciation, and investor-perceived risk increases
  - When combined with the Mundell-Fleming model, in cases of high capital mobility, expansionary fiscal policy leads to appreciation in the short term, and then depreciation in the long term
  - Also known as the asset market approach

## Capital Controls and Central Bank Intervention

- The purpose of central bank intervention is to prevent speculative bubbles by reducing excessive capital inflows
  - The size of FX reserves determine the success of intervention (relative to average trading volume in the domestic currency)
  - Usually only developing countries can hold FX reserves large enough to have a meaningful impact, due to trading volume of developed currencies being significantly larger

## Signs of Impending Currency Crises

- Deterioration in trade terms
- Reduced FX reserves
- Uncharacteristically high currency value
- Increased inflation
- Free flow of capital 
- Increased money supply relative to bank reserves
- Banking crises
- Fixed (or partially fixed) exchange rates
