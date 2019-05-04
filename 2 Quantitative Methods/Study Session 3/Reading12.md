# Reading 12: Probabilistic Approaches - Scenario Analysis, Decision Trees, and Simulations

## Simulation Steps

1. Determine probabilistic variables
2. Define probability distributions for chosen variables
3. Check for correlation between chosen variables
4. Run simulation

## Defining Probability Distributions for Simulations

- There are multiple methods of selecting appropriate probability distributions for the chosen probabilistic variables:
  - Analysis of historical data
  - Analysis of cross-sectional data
  - Subjective analysis

## Treating Correlation Between Variables

- When strong correlation between variables is present, there are two possible remedies
  - Algorithmically compute one variable, allowing only the other to vary randomly according to the defined probability distribution
  - Build the correlation behaviour into the simulation

## Advantages of Using Simulations

- Simulation design as a process encourages more careful estimation of inputs
- The output takes the form of a distribution, rather than a single estimate, and is therefore more informative

## Simulation Constraints

- There are three types of constraints that are commonly introduced into simulations:
  - Book value constraints are restrictions on a firm's book value such that:
    - Minimum capital requirements are not violated
    - Negative values of equity are disallowed by the simulation
  - Earnings / cash flow constraints can be imposed to represent analyst expectations or targets
    - Additionally it may be important to keep earnings or cash flows above certain levels in order to comply with debt covenants
  - Market value constraints allow the use of simulation to identify values of input variables that may result in financial distress

## Potential Problems With Simulation

- The level of detail in simulation output can lead analysts to believe that the inputs were of high quality, when that is not necessarily the case
- The requirements of probability distributions can be easily violated by real data, leading to a poorly specified model
- Non-stationarity of market economic conditions can mean that the appropriate choice for things like probability distributions do not remain appropriate for long
- Additionally, coping with the changing nature of relationships between input variables themselves is also challenging

## Scenario Analysis, Decision Trees, and Simulation

- Scenario analysis entails establishing a finite set of scenarios, each of which defines a value for each independent variable, characterising 'worst-cases', or 'best-cases'
  - The combined probability of each scenario will be less than one, since the true number of possible scenarios is effectively infinite
- Decision trees are used to model risks that occur sequentially, and are discrete in nature, such as whether an investment is made or not, and then whether an option is exercised or not
  - Decision trees allow analysis of all possible states, hence the probabilities do sum to one
- Correlations between variables can be built into simulations, as well as the calculations in a scenario analysis
- Decision trees and simulations can be used as valuation tools, or as complements to the valuation process
  - Scenario analysis doesn't include the full range of possibilities in it's calculation, so it cannot be used as a valuation tool