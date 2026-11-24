
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

