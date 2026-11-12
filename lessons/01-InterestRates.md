
# Week 1 – Interest Rates

[Back to contents](../README.md)

## Summary

Interest rates are about how much the value of money will change from one period to another. A way that you can express an investment return is as a percent of what you originally put into the investment so it’s easy to compare two or more investments.

$$
R=\frac{P_t-P_0}{P_0}
$$

There are two ways to calculate interest. Simple interest is just based on the original amount of money (the principal), compound interest is like simple interest but it's the original amount plus all the interest you've already been paid. This means your investment grows faster than if you were earning just the simple type of interest.

**Simple interest:**

$$
P_t=P_0(1+rt)
$$

**Compound interest:**

$$
P_t=P_0\left(1+\frac{r}{n}\right)^{nt}
$$

When you see a quoted nominal interest rate this is usually just the annual interest rate. The effective annual rate is what takes into account how often your interest is compounded. For example, if you have a positive nominal interest rate that doesn’t change then the more times your interest compounds per year then the greater your effective rate of interest will be. There is continuous compounding which is really the highest possible compounding frequency.

**Effective annual interest rate:**

$$
r_{\text{effective}}=\left(1+\frac{r}{n}\right)^n-1
$$

**Continuous compounding:**

$$
P_t=P_0e^{rt}
$$

Like anything else that has a price tag and therefore can go up or down over time interest rates do too. While we don't control our own interest rates there are some organisations that are involved in helping us make decisions regarding our use of those interest rates. As I mentioned earlier Bank Rate is controlled by the Bank of England. Additionally, SONIA (Sterling Overnight Index Average) calculates average rates on eligible overnight sterling transactions. Using overnight index swaps helps mitigate the risks associated with interest rate volatility.

As previously discussed, one method for managing inflation and changes in the purchasing power of an investment is through using inflation adjusted returns.

**Inflation-adjusted interest rate:**

$$
r_{\text{real}}=\frac{r_{\text{effective}}-i}{1+i}
$$


## My Example

Suppose I invested £2,400 for three years at a fixed nominal annual interest rate of 4.8% on a savings account that is compounded every quarter. I wish to determine what my total investment will be worth by the end of the third year using both compound interest and simple interest.

Interest is compounded each quarter which means there are 4 quarters within one year. There are therefore 4 x 3 = 12 quarters (or compounding periods) over the course of three years. Therefore the quarterly interest rate is 1.2%.

$$
\frac{0.048}{4}=0.012
$$

I can use the Compound Interest Formula to work out how much the initial investment has grown by the end of the three years (£2,769.35). Using this formula we find I have made an additional £369.35 in interest.

$$
P_t=P_0\left(1+\frac{r}{n}\right)^{nt}
$$

$$
P_t=2400\left(1+\frac{0.048}{4}\right)^{12}
$$

$$
P_t\approx2769.35
$$

**Total interest earned:**

$$
2769.35-2400=369.35
$$

Therefore the effective annual interest rate of the savings account is approximately 4.89%, which is a little bit greater than the nominal rate as a result of compounding throughout the year.

$$
r_{\text{effective}}=\left(1+\frac{0.048}{4}\right)^4-1
$$

$$
r_{\text{effective}}\approx0.04887
$$

**Effective annual interest rate: 4.89%**

If I had used simple interest rather than compound interest my total investment would have been worth £2,745.60. This is approximately £23.75 less than the total value of my compound interest investment.

$$
P_t=P_0(1+rt)
$$

$$
P_t=2400(1+0.048\times3)
$$

$$
P_t=2745.60
$$

**Difference between compound and simple interest:**

$$
2769.35-2745.60=23.75
$$


## Solved exercises

### Exercise 1

### Exercise 2

## Spreadsheet
