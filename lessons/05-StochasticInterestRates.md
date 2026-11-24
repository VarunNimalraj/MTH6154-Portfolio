
# 5. Stochastic Interest Rates

[Back to contents](../README.md)

## Summary

Previously it was presumed that interest rates would remain constant (or at least predictable) throughout the duration of an investment. In actuality, however, there may be changes in interest rates or they may have some degree of uncertainty. To allow for such uncertainty, stochastic interest rate models treat interest rates as random variables.

### Fixed Interest Rate Model

The fixed interest rate model states that an investment will have one interest rate that is unknown, but will remain unchanged during the time frame of the investment. Because compound interest is not a linear process, using the average interest rate in the calculation may not produce the same results as calculating the average future value of an investment.

**Accumulated Value:**

$$
P(n)=P(1+R)^n
$$

**Expected Accumulated Value:**

$$
E[P(n)]=P E[(1+R)^n]
$$

In general:

$$
E[(1+R)^n]\neq(1+E[R])^n
$$

Where:
- \(P\) = Initial investment
- \(R\) = Random interest rate
- \(n\) = Number of years

### Varying Interest Rate Model

A variable interest rate model permits interest rates to vary from year to year. The total value of a single investment will depend on the interest rates experienced during the time period of the investment. With regular deposits, both the size and timing of payments must also be taken into consideration. Annual interest rates are modelled independently to facilitate calculation of expected values and variances in the accumulated value.

**Accumulated Value of a Single Deposit:**

$$
P(n)=P\prod_{i=0}^{n-1}(1+R_i)
$$

If the annual interest rates are independent and identically distributed, with mean \(\mu\) and variance \(\sigma^2\):

**Expected Value:**

$$
E[P(n)]=P(1+\mu)^n
$$

**Variance:**

$$
Var(P(n))=P^2\left[\left((1+\mu)^2+\sigma^2\right)^n-(1+\mu)^{2n}\right]
$$

For regular deposits, the accumulated value can be calculated recursively:

$$
A_n=(A_{n-1}+P_{n-1})(1+R_{n-1})
$$

Where \(P_{n-1}\) is the new deposit made at the start of the period and \(A_{n-1}\) is the previously accumulated value.

### Log-Normal Interest Rate Model

Finally, the log-normal model presumes that the annual growth factors follow a log-normal distribution. As such, we can compute probabilities and establish a range of possible values for our investments at any point in the future.

If the annual growth factors are independent and identically distributed:

$$
1+R_i\sim LogNormal(\mu,\sigma^2)
$$

Then the accumulated growth factor over \(n\) years is:

$$
S_n=\prod_{i=0}^{n-1}(1+R_i)
$$

And:

$$
S_n\sim LogNormal(n\mu,n\sigma^2)
$$

This allows probabilities of future investment values to be calculated using the normal distribution.


## My Example – Fixed Stochastic Interest Rates

If an individual invests £1000 in a savings account for three years; and the potential (and unknown) interest rate is fixed at one of two levels: either 2% per year, or 10% per year.

The interest rates have a 50/50 chance of occurring.

The total accumulated value after three years, assuming the interest rate is 2% would be £1061.21. The total accumulated value after three years, assuming the interest rate is 10% would be £1331.00.

**Calculations:**

At 2% interest:

$$
FV_1=1000(1.02)^3
$$

$$
FV_1=1061.21
$$

At 10% interest:

$$
FV_2=1000(1.10)^3
$$

$$
FV_2=1331.00
$$

Because both scenarios are equally likely to occur; the "expected" value after three years can be calculated by finding the midpoint of the two amounts.

**Expected Accumulated Value:**

$$
E[FV]=0.5(1061.208)+0.5(1331)
$$

$$
E[FV]=1196.104
$$

Thus the expected accumulated value after three years is £1196.10.

Also, rather than calculating the expected accumulation value, we could find the average annual interest rate.

**Average Interest Rate:**

$$
E[R]=0.5(0.02)+0.5(0.10)
$$

$$
E[R]=0.06=6\%
$$

**Accumulated Value Using the Average Rate:**

$$
FV=1000(1.06)^3
$$

$$
FV=1191.016
$$

An average annual interest rate of 6% yields an accumulated value of £1191.02.

**Difference:**

$$
1196.104-1191.016=5.088
$$

Therefore, there is a difference of £5.09 between the two calculations, showing that using the average interest rate does not necessarily produce the same result as the expected accumulated value.


## Solved Exercises

### Exercise 1 – Uncertain Interest Rates

We have an investment of P for 1 year in which the interest rate is unknown. The possibilities are a 30% chance that the interest rate will be 3%, and a 70% chance that the interest rate will be 3.5%.

**Part (a) – Continuously Compounded Interest**

Part (a) states that the rates are compounded continuously. This means the growth of our investment can be described using the exponential function. For example, if the interest rate was 3% then the amount would grow to about 1.030455P. If the interest rate was 3.5%, then it would grow to about 1.035620P.

Using the continuous compounding formula:

$$
A=Pe^R
$$

At 3%:

$$
A_1=Pe^{0.03}=1.030455P
$$

At 3.5%:

$$
A_2=Pe^{0.035}=1.035620P
$$

If we multiply each possibility by the associated likelihood and add those results together, we get an expected value of accumulation of 1.034070P.

**Expected Accumulated Value:**

$$
E[A]=P(0.3e^{0.03}+0.7e^{0.035})
$$

$$
E[A]\approx1.034070P
$$

**Part (b) – Effective Annual Interest**

Part (b) treats the interest rate as an effective annual interest rate. In this case, our investment increases in size by being multiplied by one plus the interest rate. Therefore, there are two possible accumulated values after one year, namely 1.03P and 1.035P.

Using the annual compounding formula:

$$
A=P(1+R)
$$

At 3%:

$$
A_1=P(1.03)=1.03P
$$

At 3.5%:

$$
A_2=P(1.035)=1.035P
$$

Taking the weighted average of these values gives an expected accumulated value of 1.0335P.

**Expected Accumulated Value:**

$$
E[A]=P(0.3(1.03)+0.7(1.035))
$$

$$
E[A]=1.0335P
$$

The two expected values differ slightly because the methods of compounding interest are different.

---

### Exercise 4 – Log-Normal Interest Rates

We have been given an initial deposit of £1,000 to invest for one year at an unknown and uncertain interest rate. Thus the interest rate is modelled by some form of probability distribution.

**Part (a) – Log-Normal Growth Factor**

In Part (a) the random annual growth factor is specified as having a lognormal distribution with parameters 0.03 and 0.01 squared.

$$
1+R\sim\mathrm{LogNormal}(0.03,0.01^2)
$$

Because the interest rate is random, we don't know exactly how much the £1,000 will be worth at the end of a year. However, we can calculate its average value across the possible outcomes. That average value is called the expected value.

The accumulated value is:

$$
A=1000(1+R)
$$

Using the formula for calculating the expected value of a lognormally distributed variable, the expected accumulated value after a year is about £1,030.51.

For a log-normal random variable:

$$
X\sim\mathrm{LogNormal}(\mu,\sigma^2)
$$

$$
E[X]=e^{\mu+\frac{\sigma^2}{2}}
$$

Therefore:

$$
E[A]=1000e^{0.03+\frac{0.01^2}{2}}
$$

$$
E[A]=1000e^{0.03005}
$$

$$
E[A]\approx1030.51
$$

**Expected Accumulated Value: £1,030.51**

**Part (b) – Normally Distributed Continuous Interest Rate**

In Part (b), the interest rate is compounded continuously and has a normal distribution with a mean of 0.03 and a variance of 0.01 squared.

$$
R\sim N(0.03,0.01^2)
$$

The accumulation of value from continuously compounding is based on the exponential of the interest rate. Therefore this produces the same log-normal distribution for the investment's growth factor as produced in Part (a).

The accumulated value is:

$$
A=1000e^R
$$

Since R is normally distributed:

$$
e^R\sim\mathrm{LogNormal}(0.03,0.01^2)
$$

Therefore:

$$
E[A]=1000e^{0.03+\frac{0.01^2}{2}}
$$

$$
E[A]\approx1030.51
$$

Thus, again, the expected accumulated value is £1,030.51.


## Spreadsheet

[Download my Week 5 Excel spreadsheet](../spreadsheets/05-StochasticInterestRates.xlsx)

