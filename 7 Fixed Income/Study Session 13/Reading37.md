# Reading 37: Valuation and Analysis - Bonds with Embedded Options

## Valuation of Embedded Bonds

- The value of an option embedded in a bond is the difference in values between a straight bond, and a bond with the option embedded
- Using a binomial interest rate tree, a callable bond can be valued
  - The value of the straight bond is replaced by the exercise price of the option at any node where the price exceeds it
    - This is because instead of receiving the cash flows of the straight bond, the issuer would exercise the option
  - The procedure is similar for a putable bond, where the value of the straight bond price is replaced with the exercise price if it falls below the exercise price
- Recall that the purchaser of a callable bond is *short* the call, and the purchaser of a putable bond is *long* the put
- An embedded soft put can be redeemed with cash, subordinated notes, or common stock
  - Hard puts can only be redeemed with cash

## Impact on Values

- Option values increase with interest rate volatility
  - Hence, callable bonds fall in value, and putable bonds increase in value, as interest rate volatility increases
- An upward sloping yield curve implies that interest rates are expected to rise, and hence bond prices are likely to fall
  - This reduces the likelihood that a callable bond will enter the money, reducing the value of the option to the bond issuer
  - Furthermore, as the curve flattens, call options gain in value
- A put option is more likely to enter the money if the yield curve is upward sloping
  - The put option also loses value if the curve flattens

## Option Adjusted Spreads

- If risk-free rates are used in a binomial interest rate tree to calculate values for a risky bond, then the final computed value will be too high (since the discount rates used will be too low)
- The OAS can be interpreted as the average spread over the Treasury spot rate curve
- The OAS is a constant spread added to forward rates in a binomial interest rate tree, causing the sum of present values of a risky bond's cash flows equal the market price
- An OAS spread is calculated given a set of benchmark interest rates, and their volatility
- The option adjusted spread is "option adjusted" because it is equal to the Z-spread minus the option cost
  - Hence it includes compensation for taking on credit and liquidity risk, but not for taking on option risk (as in a callable bond)
- If the value of a bond with an embedded option changes due to a change volatility then the OAS will shift in the same direction as the value of the bond

## Effective Duration

$$
\text{ED} = \frac{\text{BV}_{-\Delta \text{y}} - \text{BV}_{+\Delta \text{y}}}{2 \cdot \text{BV}_0 \cdot \Delta\text{y}}
$$

- This expression computes the effective duration of a bond, by applying a small shift up and down in interest rates to the bond, and inputting the resulting prices into the numerator
- The effective duration of a bond with an embedded option is always lower or equal to that of a straight bond, since options reduce the risks posed by interest rate volatility
- The size of the theoretical shift in yields is irrelevant to the calculation, since the formula produces the expected percentage change in price for a 100 basis point change in yields regardless
- The duration of option-free bonds is always greater than that of bonds with embedded options

## Evaluating Interest Rate Sensitivity

- One-sided durations are more informative than regular durations with regards to interest rate sensitivity of bonds with embedded options
  - When the underlying option is near, or at, the money, callable bonds have lower one-sided down-duration than up-duration
  - Conversely, putable bonds have lower one-sided up-duration than down-duration
- As options approach the money, the most critical rate switches from being the maturity matched rate, to the time-to-exercise rate

## Effective Duration and Convexity for Bonds With Embedded Options

- Effective duration and convexity of bonds with embedded options is calculated using the following procedure
  - Calculate the OAS
  - Impose a small parallel shift in the benchmark yield curve
  - Build two new binomial trees using this new curve, one for a shift up, the other for a shift down
  - Add the computed OAS to each rate
  - Compute the new prices of the bond using the tree
  - Input these prices into the formulae for convexity and duration

## Capped and Floored Floating-Rate Bonds

- A capped floating bond has an embedded option preventing the coupon rate rising above a predetermined value

## Convertible Bonds

- Convertible bonds can be exchanged in return for common shares in the issuer
- The conversion ratio specifies how many shares the bond can be exchanged for
- Hence a convertible bond can have two separate values:
  - It's value as a bond
  - It's value as common shares
  - The value of the bond itself is always the greater of these two
- The value of a bond with embedded options (from the perspective of the bondholder) can be calculated by adding the value of options the bondholder is long, and subtracting the value of options that the bondholder is short, from the value of the straight option-free bond

## Risk-Return Characteristics of a Convertible Bond

- Investors can derive additional value from convertible bonds in the form of the appreciation of common stock
  - However, the bondholder pays a premium to enjoy this advantage in the form of a conversion premium
  - If stock prices fall, the straight value of the bond limits downside risk

## Mortgage and Asset-Backed Securities

- MBSs have an embedded prepayment option, and hence their values are path dependent, making Monte-Carlo simulation useful
- ABSs have no embedded options, hence use of the Z-spread is sufficient