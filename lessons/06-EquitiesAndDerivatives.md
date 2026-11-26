
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

