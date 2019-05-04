# Reading 16: Intercorporate Investments

## Accounting for Intercorporate Investments

- Percentage ownership used as a guide to determine level of control
- The key distinction is whether an investee is an integral part of the parent
  - Even ownership of between 20% and 50% could merit reporting as a passive investment in financial assets if there is no significant influence
  - Additionally, 

| Ownership | Degree of Control | Reporting Method |
| - | - | - |
| Less than 20% | No significant influence (passive) | As a financial asset |
| Less than 20% | Significant influence | Equity method |
| 20% to 50% | Significant control | Equity method[^1] |
| 20% to 50% | Control | Acquisition method |
| 50% each | Shared control | Equity method |
| More than 50% | Control | Acquisition |

## Classifications of Financial Securities

- *Debt securities held to maturity* are securities for which a company has the intend and ability to hold to maturity
  - Equity securities cannot hold this classification, and hence are always reported at fair value in the balance sheet
- *Debt and equity securities held for sale* may be sold to address liquidity needs
- *Debt and equity securities held for trading* are acquired for the purpose of selling in the near determine

| Classification | Balance Sheet Effect (GAAP) | Income Statement Effect (GAAP) | Differences for IFRS |
| - | - | - | - |
| Trading | Reported at fair market value | Interest, dividends, realised and unrealised gains/losses reported | No difference |
| Available for sale | Reported at fair market value (unrealised gains/losses go to Comprehensive Income) | Interest, dividends, realised gains/losses reported | Unrealised FX gains on debt also recognised |
| Held till maturity | Reported at historical cost | Interest and any realised gains/losses reported | No difference |

## IFRS 9

- Debt securities use the amortised cost method if:
    - They're held to collect cash flows, and
    - Cash flows must be principal or interest
    - $\text{Interest cost} = \text{Yield as of purchase} \times \text{PV( of debt at period start)}$
- Debt securities are classified as *fair value through profit/loss* if:
    - They are held for trading, or
    - Use of amortised cost would create a mismatch
    - Once classified, they cannot be changed

## Reclassification Under IFRS 9

- Reclassification of equity securities is not permitted
- Reclassification of debt securities is permitted in the event of a business model change
- For debt securities moving from *amortised cost* to *fair value through profit and loss*, gains/losses go to the income statement, or equity, depending on whether they are realised, and whether they are held for trading, or for sale
    - For movement in the opposite direction, fair value becomes the carrying value, with unrealised gains going to other comprehensive income, and being amortised over the remaining life of the security
- Analysts should be wary of the exclusive reclassification of securities with unrealised gains to trading securities, without reclassifying securities with unrealised losses
    - This allows a firm to increase the amount of recognised revenue

## Equity Method

- The equity method is used to account for investments in associates
- Investment listed at cost on the balance sheet
    - Note that the newly created investment account has the same value as the cash paid in the transaction, resulting in no affect on the buyer's assets
- Dividends received from the investee increase cash and decrease the investment account, but do not go to income
- Pro-rata share of investee income increases the asset account
    - Listed as income on the income statement
    - Dividends do not negatively affect the amount of additional income reported
      - Hence the equity method can result in higher net income than use of the passive method for investments in financial assets
- Two adjustments are required:
    1. Adjustment for additional depreciation due to the difference between the fair value and book value of investee fixed assets
    2. Removal of pro-rata share of unconfirmed profits
- The change in the carrying value of an investment in associates reported using the equity method is given by the following expression:
$$
\Delta\text{carrying value} = (\text{# of shares})\cdot(\text{EPS} - \text{dividend per share})
$$

## Acquisition Method

- The acquisition method is used to account for investments in subsidiaries
- Balance sheets are consolidated as follows:
    1. Add together assets and liabilities of the firm being acquired
    2. Subtract cash paid to exiting shareholders
    3. Add goodwill (according to applicable financial standards)
    4. List the minority interest as a component of stockholder's equity
- Assets of the investee no longer have a separate account on the balance sheet
- Minority interest is given by $\text{% not owned by parent}\times\text{investee net equity}$
- Income statement consolidated as follows:
    1. Add together revenues and expenses
    2. Subtract minority shareholders' share of investee income
       - Hence, recognised revenues are higher than the equity method, but net income is the same
- Minority interest is given by $\text{% not owned by parent}\times\text{investee net income}$
- Minority interest is considered equity under IFRS 9
- Cash flows between the investee and investor are neglected
- Proportionate consolidation is the same as the acquisition method, but the only a pro-rata share of the subsidiary is consolidated, and there is no minority interest account in equity

## Calculating Goodwill

- Only full goodwill is allowed by GAAP
  - $\text{Full goodwill}=\text{fair value} - \text{book value}$
- IFRS additionally allows partial goodwill
  - $\text{Partial goodwill} = \text{% owned} \times \text{full goodwill}$
- The total amount of goodwill allocated can be reduced if identifiable assets are appraised and found to have fair values in excess of their book values
  - The share of goodwill allocated is the size of the stake being acquired, multiplied by the difference in the fair and book values of the asset

## Effect of Method Choice on Reported Financial Performance

- Under the acquisition method:
    - Equity is higher (by amount of minority interest)
      - The implication here is that equity and proportionate consolidation both result in identical values for equity
    - Net income is however, the same
    - Assets and liabilities are higher
    - Sales and expenses are higher
- This leads to:
    - Lower net profit margin
    - Lower return on equity (assuming positive net income)
    - Lower return on assets (assuming positive net income)
- The equity method tends to result in better financial results than the acquisition method

## Impairment

- A security should be considered impaired when the decline in its value is "other than temporary"
  - The asset's value should be written down to the new fair value, with a loss recorded on the income statement
- Reversal of impairment losses on financial assets is not allowed under GAAP

 ## Special Purpose Entities and Variable Interest Entities

 - Special Purpose Entity (SPE):
     - Creates to isolate certain assets and obligations of the sponsor
     - Usually serve a specific purpose
     - Usually to obtain cheaper financing
     - Can take the form of a:
         - Corporation
         - Partnership
         - Joint venture
         - Trust
     - Sponsors normally lack decision-making rights
     - Sponsors usually receive pro-rata profits, or other residual interests, as opposed to a variable rate of return that is related to performance
     - An SPE does not necessarily need to have separate management or employees from that of the sponsor
 - A Variable Interest Entity (VIE) is an SPE that meets any of the following conditions:
     - Insufficient at-risk equity investment
     - Shareholders lack decision-making rights
     - Shareholders do not absorb losses
     - Shareholders do not receive residual benefits
 - The following are common examples of VIEs:
     - *At-risk equity investment* &rarr; Investor receives residual benefits and absorbs losses
     - *Debt guarantee*
         - Guarantor experiences a loss in the event of default
     - *Subordinated debt* &rarr; Debt with claims to cash flows junior to other debt
     - *Leave residual guarantee* &rarr; A lessee guarantees fair value of the asset at lease end
     - *Participation rights* &rarr; Holder receives a predetermined share of profits
     - *Asset purchase option* &rarr; Holder benefits from an increase in the fair value of the asset
 - VIEs must be consolidated by whichever firm is the primary beneficiary
     - The primary beneficiary is the firm exposed to the majority of the risk of loss, and/or the majority of the residual benefits
     - This means that due to consolidation, the establishment of a VIE can have little to no effect on many of the firm's financial ratios, such as leverage and receivables turnover

[^1]: In rare cases, proportionate consolidation is allowed in cases of significant control
