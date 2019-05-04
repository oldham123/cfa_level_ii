# Reading 33: Residual Income Valuation

## Definition Residual Income

- *Residual income* is the net income of a firm less a charge measuring stockholder opportunity costs in generating that income
  - This measure recognises that accounting profit overstates economic profit, since the cost of capital committed to the firm is not accounted for
$$
\text{RI}=\text{net income}-(\text{equity capital} \times \text{cost of equity})
$$

## Residual Income Models

- Residual income models break the firm into two components:
  - Adjusted current book value of equity
    - The value of equity used in this calculation is beginning equity
  - Present value of expected future RI
$$
V_0 = B_0 + \frac{(\text{ROE} - r) \cdot B_0}{r - g}
$$

- Note that when there are no dividends, ROE is equal to the growth rate

## Strengths and Weaknesses of Residual Income Valuation

- Strengths of residual income valuation include:
  - Terminal value does not dominate the valuation
  - Residual income uses readily available accounting data
  - This method is application to firms that do not pay dividends
  - Residual income provides a focus on economic profit
- Limitations of the model are as follows:
  - Accounting data is vulnerable to manipulation
  - Accounting data may require significant adjustment
  - The model assumes a clean surplus relationship between beginning and ending book value

## Accounting Issues

- Any accounting procedure leading to a direct charge to equity (for example foreign currency translation losses or gains) will cause the approach to break down
  - Balance sheet adjustments required include:
    - Changing from LIFO to current value inventory
    - Capitalisation of operating leases
    - Pension asset/liability issues
    - Goodwill

## Multistage Residual Income Model

- In two stage residual income valuation models, intrinsic value is composed of three components:
  - Current book value
  - Present value of interim high-growth RI
  - Present value of continuing RI

- Continuing RI will continue beyond a specified earnings horizon, depending on multiple factors
  - The expected rate at which RI is expected to fade over the life of the firm is captured by a persistence factor between zero and one
    $$
    \text{PV(continuing residual income for year T - 1)} = \frac{\text{RI}_T}{1 + r - \omega}
    $$

  - To simplify the model, one of the following assumptions is made:
    - RI is expected to persist at its current level forever $(\omega = 1)$
    - RI is expected to drop immediately to zero $(\omega = 0)$
    - RI is expected to decline to a long-run average level consistent with the industry $(0 < \omega < 1)$
    - RI is expected to decline over time as ROE approaches the cost of equity
      - This final approach neglects use of a persistence factor, in favour of noting that the present value of future RI is simply $P_T - B_T = B_T \cdot (\frac{P}{B} - 1)$
      - This final contribution may also be expressed as a premium over book value, representing perceived additional economic value

- The third is the most realistic if we assume that industry competition reduces economic profit until firms leave the industry

- The strength of the persistence factor depends on the sustainability of competitive advantages and industry structure

##  EVA and MVA

- *Economic Value Added*  measures additional value for shareholders created in a given year
  $$
  \begin{aligned}
  \text{EVA}&=\text{net operating profit after tax} - (\text{WACC} \times \text{total capital})\\
  &= \left[ \text{EBIT} \times (1- \text{tax rate} ) \right] - \text{WACC}
  \end{aligned}
  $$

  - The following adjustments should be made before calculating NOPAT and invested capital:
    - Capitalise and amortise R&D, instead of expensing
    - Add back charges on investments that will generate future returns
    - Only consider cash taxes as an expense
    - Treat operating leases as capital leases
    - Add the LIFO reverse to invested capital, and add back the change in the LIFO reserve to NOPAT

- *Market Value Added*  is the difference between the market value of a firm's long-term debt and equity, and the book value of invested capital

  - It measures the value of managements decisions since the origination of the firm

  $$
  \text{MVA} = \text{market value} - \text{total capital}
  $$

  