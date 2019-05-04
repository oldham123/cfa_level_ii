# Reading 21: Capital Budgeting

## Cash Flow Estimation for Expansion Projects

- *Expansion projects* have the following components:

  - *Initial investment outlay*
    - Purchase price, transportation and installation costs, training costs, and any required increase in net working capital
    - If an asset is purchased halfway through the year
  - *After-tax operating cash flow* 
    - $\text{CF} = (\text{sales} - \text{cash operating costs})(1 - \text{tax rate}) + (\text{tax rate} \times \text{depreciation})$
    - Note: Changes to working capital occurring mid-project should also be accounted for here
  - *Terminal year after-tax non-operating cash flow*
    - $\text{TNOCF} = \text{Sal} + \text{net WC investment} - \text{tax rate} \cdot (\text{Sal} -\text{book value of fixed capital})$
      - $\text{Sal}=\text{cash proceeds from sale of fixed capital}$

  ## Depreciation

  - In the US, most firms use straight line depreciation for financial reporting, and *modified accelerated cost recovery system* for tax purposes
    - Capital budgeting calculations should always use whichever method is used for tax purposes, since the analysis uses after-tax cash flows
    - The depreciable basis is equal to the purchase price, as well as any additional costs incurred, such as those of installation
    - When an asset is purchased halfway through a year, the half-year convention applies, halving depreciation expense in the first year, and extended the recovery period of the asset by an extra year

  ## Capital Budgeting and Inflation

  - Expected inflation is accounted for in the capital budgeting process by making two adjustments:
    - Use a nominal WACC that accounts for the effect of inflation
    - Adjust cash flows so that they are nominal

  ## Cash Flow Estimation for Replacement Projects

  - Calculations for *replacement projects* use the same process as for expansion projects, with some alterations
    - Proceeds from the sale of the asset to be replaced will reduce the initial outlay for the replacement asset
    - Depreciation of the old asset can be subtracted from the depreciation of the new asset
  - If the expected useful life of the new asset is the same as the remaining life of the existing asset then a positive NPV is sufficient to justify replacement
  - It is important to be aware of the tax implications of the sale of the replaced asset on cash flows
    - If the sale price of the asset being replaced is greater than the book value, tax must be paid on the gain
    - If the sale price is less than the book value, then taxes are reduced by an amount equal to the tax rate times the size of the loss
  - When estimating incremental after-tax cash flows:
    - Ignore sunk costs
    - Ignore financing costs
    - Include externalities, such as cannibalisation
    - Include opportunity costs

  ## Mutually Exclusive Projects With Unequal Lives

  - NPVs of projects cannot be compared for projects with unequal timespans without putting them on an equal footing with regards to duration

    - The *replacement chain* approach assumes that the shorter project will be repeated until its duration is equal to that of the longer project
    - The *equivalent annual annuity* converts NPV into an annual payment, which can be directly compared across projects
      - This is done by modelling the project as a TVM problem:

    $$
    \begin{aligned}
    \text{PV} &= \text{NPV}\\
    \text{FV} &= 0\\
    \text{N} &= \text{project lifespan}\\
    \frac{I}{Y} &= \text{project cost of capital}
    \end{aligned}
    $$

- If projects cannot be repeated however, then the project with the largest NPV should be selected regardless

## Project Risk Analysis

- *Sensitivity analysis* involves recalculating NPV after a slight alteration of a variable, to determine NPV sensitivity to that variable
  - The dependent variable is plotted on the y-axis, and the independent variable is plotted on the x-axis
    - Hence, greater sensitivity to the variable is illustrated by a steeper slope
- *Scenario analysis* involves calculating NPV for certain scenarios ('best-case', 'worst-case', etc...), each of which has a defined value for each variable
- *Monte-Carlo simulation* assigns an assumed probability distribution to each variable, and repeatedly selects a random value for each to calculate an NPV, in order to create an NPV distribution, from which expected values and a standard deviation can be calculated

## Capital Rationing

- If a firm has insufficient capital to continue investing in position NPV projects until marginal returns equal the marginal cost of capital, then it must engage in capital rationing
- *Capital rationing* is the allocation of limited capital among a set of possible projects so as to create maximum value for shareholders
  - This is done by maximising overall NPV, not simply picking the highest NPV projects

## Using CAPM to Determine the Discount Rate

- The CAPM can be altered to determine an appropriate *project* discount rate
  - Project beta $\beta_\text{project}$ measures a projectr's systematic risk
  - The SML (security market line) is used as a required return (also known as a *hurdle rate*)

$$
R_\text{project} = R_f + \beta_\text{project} \cdot \left(E(R_M) - R_f\right)
$$

## Real Options

- *Real options* represent the right (but not the obligation) to make decisions, similar to financial put or call options
  - Real options however are based on real assets
  - They offer management the flexibility sometimes required to maximise NPV
- Types of real options include:
  - Timing options
  - Abandonment options
  - Expansion options
  - Price setting options
  - Production-level options
  - Fundamental options

## Approaches to Evaluating the Profitability of Real Options

- Determine NPV of a project without the option
  - A real option always makes a project more valuable, so if NPV is already positive, then valuing the option may be unnecessary to support an investment decision
    - If capital rationing is in place, or projects are mutually exclusive, valuing the option may still be necessary to facilitate comparisons
- Use decision trees
- Use option pricing models

## Accounting Income and Economic Income

- *Economic income* of a project is the after-tax cash flow, plus change in the investment’s market value
  - Interest is accounted for in the discount rate
- *Accounting income* is the reported net income resulting from investment in a project
- Differences between economic and accounting income can arise from:
  - Different definitions of depreciation
    - The accounting approach defines depreciation based on the original investment cost
    - The economic approach defines depreciation as the change in market value
  - Different methods of accounting for financing costs
    - The accounting approach subtracts interest expense from net income
    - The economic approach accounts for financing costs in the discount rate
- Calculating depreciation for economic income calculations requires calculating the market value of a project
  - This can be done by estimating project cash flows, discounting them to the year for which market value is being calculated, and summing them together
  - Depreciation is simply the change in market value

## Other Valuation Models

- Alternative valuation techniques should lead to the same NPV
  - $\text{Economic profit} = \text{NOPAT} - (\text{WACC} \times \text{capital})$
    - This reflects the income earned by all capital holders, and is discounted at the WACC to give NPV
    - The value for capital is the remaining book value of the asset (accounting for depreciation)
  - *Residual income* is focused on returns to equity holders only, and is therefore discounted at the cost of equity to give NPV
  - *Claims valuation* separates cash flows based on the differing claims on the asset owned by debtholders (discounted at the cost of debt) and shareholders (discounted at the cost of equity), before summing the present values of each