# Reading 51: Analysis of Active Portfolio Management

## Value Added by Active Management

$$
\begin{aligned}
\text{Value added} &= \text{active return}\\&=\text{active portfolio return} - \text{active benchmark return}
\end{aligned}
$$

$$
\text{Active return} = \Sigma(\Delta \text{w}_i)\times (\text{return on security }i)
$$

- Active return is composed of return due to asset allocation and return due to security selection

$$
\text{E(R}_A)=\Sigma \Delta \text{w}_\text{j} \text{E(R}_\text{B,j}) + \Sigma \Delta \text{w}_\text{P,j} \text{E(R}_\text{A,j})
$$

where:
$$
\begin{aligned}
\text{E(R}_\text{A,j}) &= \text{E(R}_\text{P,j}) - \text{E(R}_\text{B,j})\\
\Delta \text{w}_\text{j} &= \text{w}_\text{P,j} - \text{w}_\text{B,j}
\end{aligned}
$$

- Another way of expressing active return is the following:

$$
\Sigma\Delta\text{w}_\text{j}\text{E(R}_\text{B,j})
$$

## Sharpe Ratio and Information Ratio

$$
\begin{aligned}
\text{Sharpe ratio} &= \frac{\text{R}_\text{P} - \text{R}_\text{rf}}{\sigma_\text{P}}\\
\text{Information ratio} &= \frac{\text{R}_\text{P} - \text{R}_\text{B}}{\sigma_{(\text{R}_\text{P}- \text{R}_\text{B})}}\\
\text{Optimal active risk} &= \frac{\text{IR}}{\text{SR}_\text{B}}\times\sigma_\text{B}
\end{aligned}
$$

- The Sharpe ratio of an optimal portfolio is $\sqrt{\text{SR}^2_\text{B}+\text{IR}^2_\text{P}}$
- The optimal risky portfolio is always that with the highest Sharpe ratio



## The Fundamental Law of Active Portfolio Management

- The information ratio has three inputs:
  - The information coefficient
  - The breadth
  - The transfer coefficient
- $\text{IR}=\text{TC}\cdot\text{IC}\cdot\sqrt{\text{BR}}$
- $\text{E(R}_\text{A}) = \text{IR}\cdot\sigma_\text{A}$
- An investor should always choose the manager with the highest information ratio regardless of risk aversion
- The information coefficient of a market timer is $2 \cdot (\% \text{ correct}) - 1$

## Strengths and Limitations of the Fundamental Law of Active Management

- Strengths of the fundamental loaw of active mangement include an ability to evaluate market timing performance, security selection, and sector rotation strategies
- Limitations include bias in measurement of the ex-ante information coefficient, and a lack of true independence whilst measuring the breadth of an active strategy