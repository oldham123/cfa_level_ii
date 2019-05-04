# Reading 39: Credit Default Swaps

## Credit Default Swaps

- A CDS is a contract in which one party purchases protection from another against losses from the default of a third party, the *reference entity* on a senior unsecured liability, the *reference obligation*
  - If a pre-defined credit event occurs, the buyer of the protection is compensated by the seller
  - In return for this insurance, the seller receives a premium, the CDS spread
- The payoff on a single-name CDS is based on the market value of the *cheapest-to-deliver* bond with the same seniority as the reference obligation
  - The CDS pays off to the protection buyer not only in the event that the reference entity defaults on the reference obligation, but if there is default on any issue that is of equal or greater seniority to the reference obligation
- An index CDS covers an equally weighted combination of borrowers
  - When one of the constituents of the index defaults, there is a payoff and the notional principal is adjusted downward
  - An index CDS allows protection against exposure to multiple credit issuers at once
  - The pricing of an index CDS is dependent on the level of correlation of probabilities of default amongst the constituents of the index

## CDS Pricing

- CDS prices are determined by probability of default, loss given default, and the swap's coupon rate
- The conditional probability of default (probability of default given that default has not already occurred) is the hazard rate
- The upfront premium is approximately equal to the difference between the CDS coupon (cash payments by the buyer in return for protection) and the CDS spread, multiplied by the duration of the CDS
- This upfront payment is the difference between the present values of coupon payments from the protection buyer in return for protection, and payments from the protection seller in the event of default

## CDS Uses

- Investors with no exposure to the underlying securities can purchase protection, by purchasing a *naked CDS*
- Investors can engage in a long/short trade, in which they provide protection on one debt issue, and purchase protection on another
  - A variety of this trade is a curve trade, in which the two CDSs are for different maturities