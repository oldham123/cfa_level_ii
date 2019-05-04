# Reading 31: Free Cash Flow Valuation

## Definitions of Free Cash Flow
- Free cash flow to the firm is the cash available to investors (including all stock and bondholders) after business activity concludes, operating expenses are paid, and investments are made
- Free cash flow to equity is the cash available to common stockholders after capital requirements, working capital needs, and debt financing is dealt with
- FCFF and FCFE are used analogously to dividends in the DDM, and they should be used 

## Free Cash Flow to the Firm
- There are four possible formulations of free cash flow to the firm:
$$
\begin{aligned}
\text{FCFF}_\text{NI} &= \text{NI} + \text{NCC} + \text{interest}\cdot (1-\text{tax rate})- \text{FCInv} - \text{WCInv}\\
\text{FCFF}_\text{CFO} &= \text{CFO} + \text{interest}\cdot (1-\text{tax rate}) - \text{FCInv}\\
\text{FCFF}_\text{EBIT} &= \text{EBIT} \cdot (1-\text{tax rate}) + \text{NCC} - \text{FCInv} - \text{WCInv}\\
\text{FCFF}_\text{EBITDA} &= \text{EBITDA} \cdot (1-\text{tax rate}) + \text{NCC}\cdot \text{tax rate} - \text{FCInv} - \text{WCInv}
\end{aligned}
$$
## Free Cash Flow to Equity

- There are four possible formulations of free cash flow to equity:
  $$
  \begin{aligned}
  \text{FCFE}_\text{FCFF} &= \text{FCFF} - \text{interest}\cdot (1-\text{tax rate})+ \text{net borrowing}\\
  \text{FCFE}_\text{CFO} &= \text{CFO} - \text{FCInv} + \text{net borrowing}\\
  \text{FCFE}_\text{NI} &= \text{NI} + \text{non-cash charges} - \text{FCInv} - \text{WCInv}+ \text{net borrowing}\\
  \text{FCFE}_\text{DR} &= \text{NI} - \left((1-\text{DR}) \cdot (\text{FCInv - non-cash charges}) \right)- \left( (1 - \text{DR}) \cdot \text{WCInv} \right)
  \end{aligned}
  $$

- Note the similarity between the final two formulations:

  - They are essentially identical, merely using different approaches to accounting for the effects of borrowing

- Dividends, share repurchases, and share issues have no effect on FCFF or FCFE
- Leverage changes have only a minor effect on FCFE

## Single-Stage Free Cash Flow Models

- Single stage valuation is formulated similarly as in a dividend discount model
  - Forecast free cash flow for the next period is divided by the appropriate discount rate minus firm growth:
$$
V_0 = \frac{\text{FCFF}_1}{\text{WACC} - g}=\frac{\text{FCFE}_1}{r_\text{equity} - g}
$$

- It is important to note that valuation using FCFF gives the value of the firm, whilst valuation using FCFE gives the value of equity

## Two-Stage Free Cash Flow Models

- Two-stage free cash flow valuation is also analogous to a dividend discount model, involving the same three steps:
  1. Estimate growth periods for both a high growth, and low growth period
  2. Use a single-stage FCF model to calculate a terminal value for the eternal low-growth period
  3. Discount the FCF for each period within the initial high growth stage, as well as the terminal FCF value, to $t = 0$, using the appropriate discount rate

