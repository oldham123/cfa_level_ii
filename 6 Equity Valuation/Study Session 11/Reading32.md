# Reading 32: Market-Based Valuation - Price Multiples

## Price Multiples

- Price multiples are ratios of a stock price to some fundamental variable
  - Price-to-earnings (P/E) is a common example
- A justified multiple can be determined in two ways:
  - The *method of comparables* utilised an average multiple of similar stocks within a peer group
    - The *law of one price* assets that two similar assets should sell at similar prices, and thus have similar multiples
  - The *method of forecasted fundamentals* involves estimating stock value using a DCF model, and dividing by some fundamental variable
    - This method is based on the notion that the value of any asset should be the present value of future cash flows
    - Typically this involves substituting the Gordon growth model for pricse into multiples
    - In addition the Du Pont formula for sustainable growth rate is often used

## The Price to Earnings Ratio

- The idea that earnings power (as measured by EPS) is the main determinant of investment value supports the use of P/E valuation
- Limitations of P/E valuation include:
  - Earnings can be negative, rendering P/E meaningless
  - Earnings can be volatile, making interpretation difficult
  - Management discretion over reported earnings must be considered
  - Since the value of the ratio can never fall below zero, a large sample of ratios will tend to be biased upwards as outliers accumulate
- The P/E ratio can be calculated on a *leading* or *trailing* basis
  - Trailing P/E uses earnings over the last period
  - Leading P/E uses expected earnings
- The earnings value used is usually normalised EPS, determined using either:
  - Historical average EPS, taken over the most recent complete business cycle
  - Average ROE taken over the most recent complete business cycle, multiplied by current book value per share
$$
\begin{aligned}
\text{justified leading }\frac{P}{E}& = \frac{P_0}{E_1} = \frac{1 - b}{r - g}\\
\text{justified trailing }\frac{P}{E}& = \frac{P_0}{E_0} = \frac{(1 - b) \cdot (1 + g)}{r - g}
\end{aligned}
$$

- These expressions are determined using two theoretically justified relations:
  $$
  \begin{aligned}
  P_0 &= \frac{D_0 \cdot (1 + g)}{r - g}\\
  D_0 &= E_0 \cdot (1 - b)
  \end{aligned}
  $$


## The PEG Ratio

- The PEG ratio gives a firm's P/E multiple per unit of growth
  - Assuming similar levels of risk, firms with lower PEG are understood to be undervalued, relative to firms with high PEG ratios
  - This ratio gives a view of a firm that allows a high P/E ratio to be compensated for by high growth
$$
\text{PEG ratio} = \frac{P/E}{g}
$$

- For traditional growth firms, PEG ratios typically fall between one and two
  - PEG ratios above two are thought to indicate that a firm is overvalued
  - Firms with very low expected dividend growth are likely to have PEG ratios that indicated unrealistic levels of overvaluation

## The Price-to-Book Ratio

- The P/B ratio is market price per share divided by the book value per share
- Strengths of using this ratio include:
  - Book value is usually positive, leading to a meaningful value in cases of negative earnings
  - Book value is more stable than EPD
  - Book value is a better indicator of net asset value (especially for firms holding liquid assets)
- Weaknesses of the P/B ratio include:
  - When comparing firms of very different sizes, P/B ratios can be misleading
  - Book value is heavily influenced by management discretion
  - Inflation and technological advances can cause book values and market values to differ significantly
$$
\text{justified }\frac{P}{B} = \frac{\text{ROE} - g}{r - g}
$$
- These expressions are determined using two theoretically justified relations:
  $$
  \begin{aligned}
  g &= \text{ROE} \times b\\
  E_1 &= \text{ROE} \times B_0
  \end{aligned}
  $$

- Common adjustments to book value include the exclusion of intangible assets

  - Book value forecasts are typically not widely available, so trailing values are used instead

## The Price-to-Sales Ratio

- The P/S ratio is calculated by dividing stock price by revenue per share
- Advantages of using this ratio include:
  - The ratio retains meaning even for firms that are in financial distress
  - Sales revenue is resistant to manipulation
  - Revenue is less volatile than earnings
  - P/S ratios are particularly useful in valuing mature, cyclical, and zero-income firms
- Limitations and weaknesses of P/S include:
  - High sales does not necessarily lead to profitability
  - The P/S ratio ignores differences in the cost structure between firms
  - Revenue recognition practices can still distort sales figures
$$
\begin{aligned}
\text{justified P/S ratio} &=\frac{ \left( \frac{E_0}{S_0} \right) \cdot (1 - b) \cdot (1 + g)}{r - g}\\
&= \text{net profit margin} \times \frac{P_0}{E_0}
\end{aligned}
$$

- These expressions are determined using the following relations:
  $$
  \begin{aligned}
  \frac{P_0}{S_0} &= \frac{P_0}{E_0} \times \frac{E_0}{S_0}\\
  \frac{E_0}{S_0} &= \text{net profit margin}
  \end{aligned}
  $$


## Price-to-Cash Flow Ratios

- Since value depends on the ability of a firm to generate cash, there is an intuitive justification for the use of price-to-cash-flow multiples
  - Cashflow is difficult to manipulate
  - Price-to-cash-flow is more stable than P/E
  - Price-to-cash-flow mitigates reporting quality concerns
- Disadvantages of using price-to-cash-flow multiples include:
  - Determining true cash flow may be complicated
  - FCFE may be better tan cash flow to the entire firm, but it is more volatile

## EV-EBITDA Ratios

- Enterprise value combines the market values of common stock, preferred equity, and debt, with any minority interests, and subtracts cash and investments
  - This subtraction is justified by the fact that ay acquisition price would be lowered by the amount of any liquid assets included in the transfer
- EBITDA is a pretax, pre-interest measure representing a flow to both equity and debt
  - It is best used as an indicator of total firm value
- This ratio is useful when:
  - Comparing firms with differences in financial leverage
  - Analysing firms with large values for depreciation and amortisation
  - Analysing firms with negative EPS
- However:
  - EBITDA will overstate CFO is working capital is increasing
  - FCFF better captures the impact of capital expenditures, thus making it a better measure in general

## Methods of Comparables

- The method of comparables entails comparison to a benchmark
  - Firms with multiples below the benchmark are undervalued, and vice versa
- Stock fundamentals should be similar to the fundamentals of the stocks used to create the benchmark, otherwise the comparison will not be valid