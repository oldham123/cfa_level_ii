# Reading 17: Employee Compensation - Post-Employment and Share-Based

## The Pension Obligation for a Defined-Benefit Plan

- *Projected Benefit Obligation (PBO)* &rarr; Actuarial present value of all pension benefits earned to date
  - Based on expected salary increases
  - Assumes the firm is a going concern
$$ \text{fair value of plan assets} = \text{beginning fair value} + \text{contributions} + \text{actual return} - \text{benefits paid} $$
$$ \Delta\text{PBO} = \text{service cost} + \text{interest cost} + \text{past service cost due to amendments} \pm \text{actuarial gains/losses} - \text{benefits paid} $$
- *Accumulated Benefit Obligation (ABO)* &rarr; Same as PBO but neglected projected salary increases

## Balance Sheet Effects

- A plan's *funded status* reflects its economic standing
- The funded status appears as a balance sheet item
  $$ \text{funded status} = \text{fair value of plan assets} - \text{PBO} $$
- The fair value of plan assets at the beginning of the period is increased by the actual return on plan assets, as well as employer contributions, and is reduced by benefits paid
- The balance sheet should reflect the true economic position of the pension plan, since deferred and unrecognised items are accounted for in calculation of the net pension asset / liability

## Pension Expense Components

| Component | GAAP | IFRS |
| - | - | - |
| Current service cost | Income statement | Income statement |
| Past service cost | OCI, amortised over service life | Income statement |
| Interest cost | Income statement | Income statement |
| Expected return | Income statement | Income statement[^1] |
| Actuarial gains/losses | Amortised portion to income statement, unamortised to OCI | All in OCI, not amortised |

- *Service cost* is the PBO increase due to newly earned benefits
- *Interest cost* is the BO increase resulting from interest owed on the current benefit obligation
- *Expected return on plan assets*
  - Under GAAP, the assumed long run rate of return used to smooth out volatility of real returns
  - Under IFRS, the discount rate used for calculating the PBO
  - &rarr;Under IFRS, the discount rate used for calculating the PBO
- *Amortisation of unrecognised prior service cost*
  - Under GAAP, amortised costs for changes in the PBO that result from amendments to the plan
  - Under IFRS, prior service costs are expensed immediately
- *Amortisation and deferral of gains/losses* &rarr; Caused by changes in assumptions and differences in expected and actual returns
  - Under GAAP, recognised in OCI and amortised using the corridor method
  - Under IFRS, recognised in OCI and not amortised

## Classification of Operating and Non-Operating Items

- $\text{IFRS Operating Inc.} = \text{GAAP Operating Inc.} + \text{TPPC} - \text{service cost}$
- $\text{IFRS Interest Expense} = \text{GAAP Interest Expense} + \text{interest cost}$
- $\text{IFRS Non-Op Income} = \text{GAAP Non-Op Income} + \text{actual return}$

## Reclassification from Operating to Financing Cash Flows

- Whilst firms are required to show the economic reality of the funded status of a pension plan in the balance sheet, the view captured from the income statement may differ
  - If the difference between cash flows and reported economic pension expense are considered material, an analyst may consider reclassifying the difference from operating activities to financing activities
  - This is to reflect that the discrepancy is considered as a source of borrowing

$$
\text{CFO to CFF} = (\text{TPPC} - \text{contribution})\times(1-\text{tax rate})
$$

## Adjustment of Operating Profit

- Pension expense should be added back to operating profit, with service cost subtracted
- Interest cost should be added to interest expense
- Actual return on plan assets should be added to other income

## Total Periodic Pension Cost

- Eliminates smoothing amounts and uses actual return on assets
  - Includes pension expense recognised in the income statement and pension cost bypassing the income statement that is recognised in OCI
  - Represents true pension cost
  - If TPPC exceeds contributions, the difference can be seen as a source of borrowing
  - Inversely, contributions exceeding TPPC can be viewed as a reduction in the overall obligation 
- Due to TPPC being a net smaller amount, it is usually more sensitive to changes in actuarial assumptions than the PBO

$$
\begin{aligned}
\text{TPPC } & = \Delta \text{PBO} + \text{benefits paid} - \text{actual return on plan assets} \\
\text{TPPC } & = \text{contributions} - \Delta\text{funded status} \\
\text{TPPC } & = \text{service cost} + \text{interest cost} + \text{plan amendments} − \text{actual return on plan assets}
\end{aligned}
$$

## Fundamental Pension Assumptions

- The following assumptions must appear in pension footnotes
  - The discount rate used to compute the PBO
  - The rate of compensation increase
  - The expected return on plan assets (GAAP only)
- Even small changes can have a large impact on the net pension asset/liability and net pension expense
- High discount rates, low compensation growth rates, and high expected rates of return will minimise pension expense, and the pension liability

## Non-Pension Postretirement Benefits

- Accounting for non-pension benefits is similar to accounting for pension benefits:
  - Accumulated postretirement benefit obligation is the actuarial present value of the expected benefit
  - Many postretirement benefit plans are unfunded, meaning no plan assets, and contributions are simply benefits paid
- There is a broadly held-assumption regarding health care costs that they will, over time, taper off to a lower, constant rate
  - This future rate is the ultimate health care trend rate

## Share-Based Compensation

- Under SFAS No. 123(R) firms are required to use a fair value method to value stock option plans
  - Fair value is estimated using an option pricing model, but in the absence of a market-based instrument, with Black-Scholes,Monte-Carlo, and binomial models are acceptable choices
- Compensation expense related to stock (call) option plans are reported on the income statement based on value at issuance
  - Expense is amortised over the course of the period required for option vestment (service period)
  - This results in lower net income and retained earnings
  - This is offset by an increase to paid-in capital
- The value of stock options offered, and thus the compensation expense and effect on reported net income, can be affected by a number of factors
  - The payment of dividends reduces the value of the underlying stock, and therefore reduces option value
  - The value of call options is positively related to the risk-free rate
  - An increase in the assumed stock price volatility increases the value of call options on stock
- The grant date of an award of stock-based compensation is the date that the options are given to the employee, and is approved by the board of directors, or a compensation committee
- If shares are granted, but cannot be sold for a given amount of time, then the compensation expense recorded is spread over that period of time, called the service period
- When two or more performance conditions must be satisfied, the requisite service period ends when the first is met
- Stock appreciation rights give recipients the right to compensation based on the appreciation of their employer's stock price
- Phantom stock provides a payoff based on the performance of hypothetical stock, as opposed to actual shares
- Performance stock is a type of stock grant, contingent on meeting predetermined performance goals
- Restricted stock is stock that cannot be sold until vesting

[^1]: Under IFRS the expected rate of return is the discount rate, and net interest expense/income is reported