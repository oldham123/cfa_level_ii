# Reading 40: Pricing and Valuation of Forward Commitments

## Pricing vs. Valuation of Forward Contracts

- The price of a forward contract is the price at which the counterparties have agreed to exchange the underlying asset at expiry
- The value of a forward contract is the amount a counterparty would be willing to pay, or would need to be paid, in order to terminate the contract
  - The amount that one side would be willing to pay, is the amount that the other would demand in return for termination 
- The *no-arbitrage* price of the contract is the price at which the value to both sides is zero:
$$
\text{FP} = S_0 \times (1 + R_f)^T
$$
where:
$$
\begin{aligned}
\text{FP}& = \text{no-arbitrage forward price}\\
S_0 & = \text{spot price of the underlying asset}\\
R_f & = \text{risk-free rate}\\
T & = \text{years until contract expiry}
\end{aligned}
$$
- The value of a forward contract at initiation is zero, because the price is set to prevent arbitrage
  - As prices and interest rates fluctuate during the life of the forward, the value can change
  - Value can be extracted by from the difference between the forward price and the spot price 
    - Value at contract expiry is simply the current spot price minus the forward price
    - Value during the contract is the current spot price minus the forward price discounted to time $t$ at the risk-free rate

 ## Forward Contract On a Stock

 - Forward contracts on stocks require adjustment for additional cash flows from dividends
   - This can be done by adjusting the spot price for the present value of expected dividends
   - Or by adjusting the forward price for the future value of expected dividends 
$$
\begin{aligned}
\text{FP} &= (S_0 - \text{PV(dividends)}) \times (1 + R_f)^T\\ &=  S_0 \times (1 + R_f)^T - \text{FV(dividends)}
\end{aligned}
$$
- Adjusting the value of a forward contract on a stock is done by subtracting the present value of expected dividends from the current spot price

## Forward Contract on Equity Index
- Dividends on an equity index are approximately continuous
  - Price and value calculations are the same, adjusted to use the continuously compounded risk free rate, and dividend yield
$$
\text{FP(equity index)} = S_0 \times e^{(R^c_f - \delta^c) \times T}
$$

- In the above formula, $T$ is integer number of periods until forward expiration, e.g. for a 30-day forward, $T=\frac{30}{365}$
- It should be noted that if no dividends are expected within the time period relevant to the forward then the dividend yield is irrelevant
- Note that if the dividend yield is sufficiently high, the forward price may fall below the spot price, due the benefit of carrying the asset in the intermediate time be greater than the benefit of holding the amount of cash equivalent to the spot price until the date of contract expiration
- *Backwardation* is defined as a future's price falling below the spot price, due to the risk aversion of hedgers with long asset positions

## Forward Contract on Fixed Income Securities

- Calculating the no-arbitrage forward price on a coupon-paying bond is done in the same way as for stocks
  - Present value of expected dividends is exchanged for present value of coupon payments

## Futures Contracts on Fixed Income Securities

- The difference between a future's price and the spot price must be zero at expiration to prevent arbitrage
- The short in a futures contract may be able to decide which bond to offer when settling
  - In this case the quoted futures price should be adjusted using a conversion factor related to the cheapest-to-deliver bond
$$
\text{QFP} = \left[\text{(full price)}(1+R_f)^T-\text{AI}_T-\text{FVC}\right]\left(\frac{1}{\text{CF}}\right)
$$
where:
$$
\begin{aligned}
\text{QFP}& = \text{quoted futures price}\\
\text{full price} & = \text{clean price} + \text{accrued interest at } t = 0\\
\text{AI}_T & = \text{accrued interest at point of bond maturity}
\end{aligned}
$$

## Futures Contracts on Currencies

- To calculate the price of a currency future, use the following formula:

$$
V_0=S_0 \times \frac{(1 + r_\text{DC})^t}{(1 + r_\text{FC})^t}
$$

- In this equation, $t$ is the integer number of years for which the future lasts

## Forward Rate Agreements

- The long counterparty to an FRA borrows money, with an interest rate equal to the contract price
  - The contract can be viewed as a right to borrow at *below* market rates, if the price of the contract is below LIBOR
    - Hence, the long receives a payment equal to the value of this right
  - Conversely, if LIBOR is below the FRA price, then the short counterparty will receive a payment, equal to the value of the right to lend at *above* the market rate
  - Functionally, the lending still occurs at the prevailing rate as of the onset of the loan, but a payment exchanges hands so that the effective price of the loan is as specified in the forward
- FRA notation specifies the number of months until contract expiry, and the number of months until settlement of the underlying loan
  - Both dates are measured from the date of contract initiation
- The price of the FRA is the forward rate implied by the current spot rates at the dates in question
- FRA payments are settled at the *initiation* of the notional borrowing period, not the end

## Valuing FRAs

- FRA value emerges from interest savings on a hypothetical loan initiations at the settlement date
  - The value is the present value of interest savings as of the end of the loan
- For example, consider a 2x3 FRA (a 30-day loan to be initiated in 60 days), now 40 days after initiation
  - First, calculate the implied 30-day forward rate, 20 days from now $L_{30(20)}$, using the current 20-day and 50-day spot rates, $S_{20}$ and $S_{20}$.
    - This procedure involves de-annualising the rates, dividing the shorter out of the larger rate, and then re-annualising, as seen in the example below:
    - $L_{30(20)} =\left( \frac{1 + S_{50} \cdot \frac{50}{365}}{1 + S_{20} \cdot \frac{20}{365}} - 1 \right) \cdot \frac{365}{30}$.
  - Multiply the notional principal on the hypothetical loan by the difference between the FRA price, and this implied forward rate
  - Discount the final value to the present day
$$
V_t = \frac{(\text{F}_t-\text{F}_0) \cdot (\text{contract size})\cdot T}{1+r}
$$
- Here, $T$ represents the integer number of annual periods for which the notional borrowing period lasts
- $r$ represents the current $T$-day LIBOR
- Forward rates occasionally use the following notation:
  - $L_{10(20)}$ is the 10-day forward rate, in 20 days

## Currency Forwards

- Covered interest parity gives the no-arbitrage forward price of a unit of foreign currency in terms of a home currency
$$
\text{FP}_t = S_t \times \frac{(1+R_\text{PC})^{T-t}}{(1+R_{\text{BC}})^{T-t}}
$$
- $S_t$ is the spot rate at time $t$ for the foreign (base) currency in terms of the home (price) currency
- The value of a currency forward depends on the difference between the current forward rate and the original forward price, discounted at the price currency interest rate
  - Note that the contract size term below should be in the base currency, since it is then multiplied by the difference in the forward rates, and converted into price currency
$$
V_t = \frac{(\text{FP}_t-\text{FP}_0) \cdot (\text{contract size})}{(1+r_{\text{PC}})^{(T-t)}}
$$

## Arbitrage Using Currency Forwards

- If a one year currency forward is trading above the arbitrage-free forward price, then there is an arbitrage opportunity
  - The implication is that the amount an investor would gain by investing a unit of the currency at its risk free rate for a year, is less than the amount an investor would receive for agreeing to sell a unit of currency in a year's time
  - Profit can be earned using the following steps:
    - Sell the forward, agreeing to deliver the currency in a year's time
    - Borrow one's own currency, and use it to purchase enough currency to deliver on the forward
    - Invest (lend) the purchased foreign currency, allowing it to appreciate to the amount required to deliver
    - Use the proceeds from the forward to settle the initial debt

## Pricing and Valuation of Swaps

- The price of a vanilla swap is the price which ensures the value of the swap is zero
  - i.e. The present value of fixed rate payments equals the present value of floating rate payments
  - As rates fluctuate, the value of the swap becomes non-zero, whilst the price remains fixed
  - The quoted rate is annualised, and needs to be adjusted for calculations involving swaps lasting a non-integer number of years

## Swaps as Combinations of Other Instruments

- By issuing a fixed-coupon bond, and investing the proceeds in a floating rate bond with the same maturity and payment dates, a position equivalent to a vanilla interest rate swap can be created
  - On each payment date, a fixed coupon payment is paid, and the floating rate payment is received
- In general, a swap is equivalent to a series of off-market FRAs
  - This is because, as the rate on the swap is fixed, as economic conditions change, the FRA price will no longer be such that their value is zero, hence they are considered 'off-market'
- An equity swap is equivalent to borrowing at a fixed rate, and investing in an equity security
- A currency swap is equivalent to issuing a bond in one currency, exchanging the proceeds for another currency at the spot rate, and purchasing a bond denominated in the other 

## Pricing and Valuing a Plain Vanilla Interest Rate Swap

- The price of a vanilla interest rate swap can be determined as the fixed rate required to ensure that the present values of the fixed payments and the floating payments are equal
$$
\begin{aligned}
\text{SFR}_\text{annual}& = \text{SFR}_\text{periodic} \times \text{yearly settlement periods}\\
\text{SFR}_\text{periodic}& = \frac{1 - \text{last discount factor}}{\Sigma(\text{remaining discount factors})}\\
\text{discount factor }Z& = \frac{1}{\text{deannualised implied spot rate}}
\end{aligned}
$$
where $Z_i$ is the present value of a payment of \$1 to be received on the $i$th 
- The value of such a swap to the fixed rate payer is the present value of the difference in swap payments based on the new swap rate (i.e. the swap rate yielded by calculating the no arbitrage swap rate again with current rates)
$$
V_\text{fixed payer} = \Sigma Z \times (\text{SFR}_\text{New} - \text{SFR}_\text{Old}) \times \frac{\text{days}}{360} \times \text{principal}
$$
- Note that in the case of an interest rate swap, the price and value will never be equal, since the price is expressed as a rate, whilst the value is a cash amount

## Pricing and Valuing a Currency Swap

- A currency swap is used to obtain funding in a foreign currency with favourable terms
  - A notional principal in the domestic currency is paid at the outset, in return for a notional principal in the foreign currency
  - Interest is paid in the foreign currency, and received in the domestic currency during the life of the swap
  - At the swap's conclusion, the notional principals are exchanged once again
- The procedure for currency swaps is the same as for an interest-rate swap
  - However, there is a term structure (and thus a fixed swap rate, or 'price') for each currency
  - In a fixed-for-fixed USD / EUR swap, the USD fixed rate is determined using the USD term structure, and the EUR fixed rate is determined using the EUR term structure
- Valuing a currency swap involves calculating the difference between cash flows paid and cash flows received
  - Given a notional principal of the swap in dollars, convert to euros using the initial exchange rate
    - These values are the "notional face values" of the hypothetical underlying bonds denominated in each currency
    - The two bonds can then be valued using the usual procedure
    - The value of the euro denominated bond should be converted to USD using the rate in effect on the date of valuation
    - The value to the party paying USD is the value of the euro bond minus the value of the dollar bond
- The aim of a currency swap is usually to obtain favourable borrowing terms in a foreign currency
  - For example, a US firm using a currency swap to borrow and invest in Europe would receive EUR, and pay USD at the outset, paying EUR interest and receiving USD interest over the life of the swap
  - The interest paid is determined by the rates of the foreign country
  - At the swaps conclusion, the principals are returned to each party, along with a final interest payment
$$
\begin{aligned}
\text{interest paid} &= \text{USD notional principal}\\
&\cdot \text{USD/EUR spot rate}\\
&\cdot \text{EUR interest rate adjusted for period length}
\end{aligned}
$$

## Equity Swaps

- The fixed-rate side of an equity swap is priced and valued identically to an interest rate swap
  - Each interest payment $(\text{SFR}\cdot\text{notional principal})$ should be discounted to the current time using the appropriate deannualised rate
    - Note that the final payment should also include the notional principal
- The equity side can be valued by appreciating the notional principal by the appreciation of the equity since the last settlement
  - Take care to ensure that the hypothetical 'invested capital' is set at the notional principal at each settlement date, for the purposes of calculating the equity return to be paid