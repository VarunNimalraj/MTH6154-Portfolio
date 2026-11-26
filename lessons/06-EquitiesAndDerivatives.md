
# 6. Equities and Derivatives

[Back to contents](../README.md)

## Summary

### Log-Normally Distributed Interest Rates (Section 4.3)

Log-normally distributed annual growth factors enable the modelling of uncertainty in future investment values. Using log-normal assumptions about future one-year growth factor distributions, we can calculate the probability of possible accumulated investment outcomes.

Assuming the annual growth factors are independent and identically distributed:

$$
1+R_i\sim\mathrm{LogNormal}(\mu,\sigma^2)
$$

The accumulated growth factor over n years is:

$$
S_n=\prod_{i=1}^{n}(1+R_i)
$$

Therefore:

$$
S_n\sim\mathrm{LogNormal}(n\mu,n\sigma^2)
$$

The accumulated value of an initial investment P is:

$$
A_n=PS_n
$$

This allows us to calculate probabilities of different future investment values using the normal distribution.

### Shares

Stocks represent fractional ownership in a company. In addition to potentially increasing stock prices over time, investors may receive dividend income as payments made by companies to their shareholders.

**Percentage Ownership:**

$$
\text{Ownership Percentage}=\frac{\text{Shares Owned}}{\text{Total Shares Outstanding}}\times100
$$

**Market Capitalisation:**

$$
\text{Market Cap}=\text{Share Price}\times\text{Total Shares Outstanding}
$$

The market capitalisation represents the total market value of a company's outstanding shares.

### Forward Contracts

Forward contracts involve agreements between two parties to purchase (or sell) a specific underlying asset on a pre-determined date, at a previously agreed upon price. Forward contracts can be employed to hedge against changes in underlying assets' future price levels, or to speculate on future price movement. The no-arbitrage pricing relationship provides a basis for determining the fair forward price.

**Fair Forward Price:**

$$
F=\frac{S}{D(T)}
$$

Where:

- \(F\) = Fair forward price
- \(S\) = Current spot price of the underlying asset
- \(D(T)\) = Discount factor to maturity time \(T\)

For a continuously compounded interest rate \(r\):

$$
D(T)=e^{-rT}
$$

Therefore:

$$
F=Se^{rT}
$$

These formulas assume that the underlying asset provides no income before maturity and that there are no storage costs.

**Payoff of a Long Forward Position at Maturity:**

$$
\text{Payoff}=S_T-K
$$

Where:

- \(S_T\) = Market price of the underlying asset at maturity
- \(K\) = Agreed forward delivery price

A long forward position gains value when the asset price at maturity exceeds the agreed delivery price.


### Options

Financial Options provide the holder with the "right", but not the obligation, to buy or sell a designated underlying asset at a specific price ("strike"). There are two types of options: Call Options -- where the buyer has the right to purchase the underlying asset; Put Option -- where the buyer has the right to sell the underlying asset. European style options are exercisable at expiration only, while American style options have the ability to be exercised at any time up to and including expiration. Unlike forward contracts, option buyers can choose not to exercise if the price moves unfavourably, but they pay a premium for this right.

**Payoff of a European Call Option:**

$$
C_T=\max(S_T-K,0)
$$

**Payoff of a European Put Option:**

$$
P_T=\max(K-S_T,0)
$$

Where:

- \(S_T\) = Price of the underlying asset at expiry
- \(K\) = Strike price
- \(C_T\) = Call option payoff at expiry
- \(P_T\) = Put option payoff at expiry

For a call option, the holder benefits when the market price exceeds the strike price. For a put option, the holder benefits when the market price falls below the strike price.

If exercising an option would be unfavourable, the holder can let it expire without exercising.

These formulas represent the payoffs at expiry and do not deduct the premium paid to purchase the option.

