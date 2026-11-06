# 1. Interest rates

[Back to contents](../README.md)

## Summary

To summarise, interest rates help us understand the way that the value of money changes over time. Once we have put our initial money into an investment, the profit we earn will be the result of subtracting what we started with from what it has grown to. We get the per cent return from dividing this difference by the initial investment.

**Percent Return:**

$$
R = \frac{P_t - P_0}{P_0}
$$

If we invest some money for $t$ years, then the annualised simple rate of return will be equal to the total per cent return divided by the number of years you had the money invested.

**Annualised Rate of Return:**

$$
r = \frac{R}{t}
$$

Compounding is a very important term. Compounding occurs when the interest is made on top of the original amount of money that was invested plus all of the previous amounts of money that were gained due to interest. So basically, if you make 10% each year, your account would be making 11% next year. Simple interest does not work like this; instead, simple interest just calculates interest based on the original amount of money. Compound interest allows your money to grow at a higher rate as the interest is re-invested back into your account.

**Simple Interest Formula:**

$$
P_t = P_0(1 + rt)
$$

**Compound Interest Formula:**

$$
P_t = P_0\left(1 + \frac{r}{n}\right)^{nt}
$$

The more often you allow the bank to add or "compound" interest onto your principal, the higher your true or "effective" annual interest rate. This means that if you want to compare two investments with different compounding periods, you need to know the effective rate.

**Formula for Effective Annual Interest Rate:**

$$
r_{\text{effective}} = \left(1 + \frac{r}{n}\right)^n - 1
$$

It is possible for banks to continually add interest (compounded) to your principal. When they do this, they use the natural exponential growth function to find out how much your account will be worth at some future date.

**Continuously Compounding Interest Formula:**

$$
P_t = P_0 e^{rt}
$$

Banks set their own base lending rates. However, since these rates fluctuate over time, most commercial banks choose to lock their borrowing costs using OIS's (Overnight Index Swaps). These OIS's essentially replace fixed payments with variable payments that are tied to the compounded overnight SONIA (Sterling Overnight Interbank Average) rate.

A key term is the "yield curve". It is a graph showing how lending rates change when you lend money for different lengths of time. A continuous yield curve is actually the average interest rate per unit time over an interval. A yield curve provides information about whether long term loans carry a greater risk than short term loans.

**Yield Curve Equation:**

$$
\bar{r}(T) = \frac{1}{T}\int_0^T r(t)\,dt
$$

Lastly, inflation affects how valuable investments become. An investor may see their investment rise in monetary terms but experience a loss of purchasing power due to increased prices. Therefore, even though an investor may receive a certain interest rate on their loan or investment, he/she will lose purchasing power. To adjust for this effect of inflation on investing returns, the "inflation adjusted interest rate" should be considered. The inflation adjusted interest rate takes into consideration both the inflation rate and the effective interest rate.


## My example

A situation you made up (your own numbers, not the ones in the lecture
notes), worked step by step.

## Solved exercises

### Exercise 1.x (from Exercise Sheet 1)

Question, then your solution.

## Spreadsheet

[01-InterestRates.xlsx](../spreadsheets/01-InterestRates.xlsx): what it
does, which cells to change and what to look at.
