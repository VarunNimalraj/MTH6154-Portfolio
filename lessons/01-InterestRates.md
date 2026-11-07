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


### My example


Suppose I invest £2,400 into a savings account offering a nominal annual interest rate of 4.8%, compounded quarterly. The investment will be held for three years.

## Step 1 – Compound Interest Calculation

In order to calculate the final amount for my £2400 investment, I will utilise the compound interest formula. The investment earns interest quarterly; therefore, the interest is applied to the account 12 (four times per year * three years) times. Substituting the values for initial deposit, annual interest rate, number of times interest is compounded annually and length of time of the investment into the compound interest formula provides me with a final balance of approximately £2769.35.

**Compound Interest Formula:**

$$
P_t=P_0\left(1+\frac{r}{n}\right)^{nt}
$$

**Substituting the values:**

$$
P_3=2400\left(1+\frac{0.048}{4}\right)^{4\times3}
$$

$$
P_3=2400(1.012)^{12}
$$

$$
\boxed{P_3=£2,769.35}
$$

From this value, I can easily compute the profit by subtracting the original amount of £2400 from the final amount. Therefore, the profit generated through compound interest over the three years is £369.35.

$$
\text{Profit}=2769.35-2400
$$

$$
\boxed{\text{Profit}=£369.35}
$$

## Step 2 – Effective Annual Interest Rate Calculation

The effective annual interest rate reflects how often interest is compounded during the course of one year. In this case, since interest is compounded quarterly and the nominal annual interest rate offered was 4.8%, the effective annual interest rate will be greater than the nominal interest rate as a result of being based upon compounded interest.

**Effective Annual Interest Rate Formula:**

$$
r_{\text{effective}}=\left(1+\frac{r}{n}\right)^n-1
$$

**Substituting the values:**

$$
r_{\text{effective}}=\left(1+\frac{0.048}{4}\right)^4-1
$$

$$
r_{\text{effective}}=0.0488709
$$

$$
\boxed{r_{\text{effective}}\approx4.89\%}
$$

By utilising the formula for effective annual interest rates, I am able to compute an effective annual interest rate of 4.89%. This clearly illustrates that the effective interest rate is larger than the nominal interest rate when compounded interest is utilised in lieu of simple interest.

## Step 3 – Comparison of Results Using Simple Interest vs. Compound Interest

Finally, I will compute how large the investment would grow if simple interest were utilised versus compound interest.

As stated earlier, unlike compound interest which utilises prior investments and their associated interest earnings in calculating future amounts owed, simple interest uses only the principal invested at the beginning of the period. As a consequence, simple interest calculations require less effort than those involving compound interest since no new amounts need to be computed every year. Utilising the simple interest formula, the amount due after three years would be £2745.60.

**Simple Interest Formula:**

$$
P_t=P_0(1+rt)
$$

**Substituting the values:**

$$
P_3=2400(1+0.048\times3)
$$

$$
P_3=2400(1.144)
$$

$$
\boxed{P_3=£2,745.60}
$$

**Difference between compound and simple interest:**

$$
2769.35-2745.60=£23.75
$$

When comparing the results from step 1 and step 3 above, we see that the investment grew significantly larger with compound interest (£2769.35) than with simple interest (£2745.60). Thus, we see the benefits provided by compound interest for creating significant wealth creation opportunities through generating interest on both principal deposited initially and prior-earned interests.

## Solved exercises

### Exercise 1.x (from Exercise Sheet 1)

Question, then your solution.

## Spreadsheet

[01-InterestRates.xlsx](../spreadsheets/01-InterestRates.xlsx): what it
does, which cells to change and what to look at.
