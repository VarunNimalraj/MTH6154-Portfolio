
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


## My Example – European Call Option

Suppose you buy a European call option on a single share that has a strike price of £50. You pay £3 as your option premium (the amount of money required to purchase the option). In 90 days, the option expires.

Assume when the option matures, the stock is trading at £60. Then you have the right to buy the stock for £50. As the stock was selling for £60, you will make a gain of £10 by exercising your option. But remember, the total cost of acquiring the stock will be £53 (£50 + £3), so your net profit is £7.

**Calculations:**

Strike price:

$$
K=50
$$

Share price at expiry:

$$
S_T=60
$$

Call option payoff:

$$
C_T=\max(S_T-K,0)
$$

$$
C_T=\max(60-50,0)=10
$$

Net profit after deducting the £3 premium:

$$
\text{Net Profit}=10-3=7
$$

**Net Profit: £7**

### If the Share Price Falls

On the other hand, assume the stock price falls to £45. Because it is cheaper to buy the stock outright for £45 than to buy it for £50, there is no reason to use your option to buy the stock.

**Calculations:**

Share price at expiry:

$$
S_T=45
$$

Call option payoff:

$$
C_T=\max(S_T-K,0)
$$

$$
C_T=\max(45-50,0)=0
$$

Net profit after deducting the £3 premium:

$$
\text{Net Profit}=0-3=-3
$$

**Net Loss: £3**

As such, the option lapses, or "dies," at expiration and you lose only your original premium of £3.

### Conclusion

In conclusion, the way a call option works gives investors a chance to earn profits when stocks are rising, but limits losses to just the amount of money invested in premiums.


## Solved Exercises

### Exercise 1 – Financial Derivatives

**(a) – A Forward Contract**

A forward contract is one that is entered into by two parties who agree to either buy or sell an investment product for a pre-determined price on some future date. Neither party in a standard forward contract has to make an initial payment when they enter the agreement.

**(b) – A European Call Option**

A European call option provides the buyer with the right, but not the obligation, to purchase an underlying investment at a predetermined strike price. A European option may be exercised only on its expiration date.

**(c) – An American Put Option**

An American put option provides the buyer with the right, but not the obligation, to sell an underlying investment at a predetermined strike price. Unlike a European option, this type of option may be exercised at any point prior to and including its expiration date.

### Exercise 4 – Put-Call Parity

We have a stock with a present price of £12.00. Options (both European call and European put) are available for this same stock. Both call and put options have the same strike price of £30.00, as well as the same expiration date -- 10 years from now. A call option has a cost of £12.50, whereas a put option has a cost of £14.50.

The objective here is to determine the implied interest rate (assuming it is compounded continuously).

The method I am going to describe allows you to utilise the Put-Call Parity Relationship. This relationship ties together the values of European call options and European put options; as well as the current value of the underlying share and its strike price, using the discount factor.

**Put-Call Parity Formula:**

$$
C-P=S_0-Ke^{-rT}
$$

Where:

- \(C\) = Call option price
- \(P\) = Put option price
- \(S_0\) = Current share price
- \(K\) = Strike price
- \(r\) = Continuously compounded annual interest rate
- \(T\) = Time until expiration

Once we plug in all known quantities into the Put-Call Parity Equation, we can manipulate this equation so as to obtain our discount factor.

**Substituting the Values:**

$$
12.50-14.50=12-30e^{-10r}
$$

$$
-2=12-30e^{-10r}
$$

$$
30e^{-10r}=14
$$

$$
e^{-10r}=\frac{14}{30}
$$

$$
D(10)=0.466667
$$

Our discount factor turns out to be about 0.467.

**Calculating the Interest Rate:**

Taking the natural log of this value, and dividing by -10, since our options are scheduled to expire in ten years, we get an annual continuously compounded interest rate of approximately 7.62%.

$$
-10r=\ln\left(\frac{14}{30}\right)
$$

$$
r=-\frac{\ln(14/30)}{10}
$$

$$
r\approx0.076214
$$

**Final Answer: 7.62%**



