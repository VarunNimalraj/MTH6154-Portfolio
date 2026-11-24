
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


