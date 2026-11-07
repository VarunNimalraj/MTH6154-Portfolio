
# 1. Interest rates

[Back to contents](../README.md)

## Summary

To summarise, interest rates help us understand the way that the value of money changes over time. Once we have put our initial money into an investment, the profit we earn will be the result of subtracting what we started with from what it has grown to. We get the per cent return from dividing this difference by the initial investment.

**Percentage Return:**

$$
R = \frac{P_t-P_0}{P_0}
$$

If we invest some money for $t$ years, then the annualised simple rate of return will be equal to the total per cent return divided by the number of years you had the money invested.

**Annualised Rate of Return:**

$$
r = \frac{R}{t}
$$

Compounding is a very important term. Compounding occurs when the interest is made on top of the original amount of money that was invested plus all of the previous amounts of money that were gained due to interest. So basically, if you make 10% each year, you would earn more money in interest the following year because your account balance has grown. Simple interest does not work like this; instead, simple interest just calculates interest based on the original amount of money. Compound interest allows your money to grow at a higher rate as the interest is re-invested back into your account.

**Simple Interest Formula:**

$$
P_t=P_0(1+rt)
$$

**Compound Interest Formula:**

$$
P_t=P_0\left(1+\frac{r}{n}\right)^{nt}
$$

The more often you allow the bank to add or "compound" interest onto your principal, the higher your true or "effective" annual interest rate. This means that if you want to compare two investments with different compounding periods, you need to know the effective rate.

**Formula for Effective Annual Interest Rate:**

$$
r_{\text{effective}}=\left(1+\frac{r}{n}\right)^n-1
$$

It is possible for banks to continually add interest (compounded) to your principal. When they do this, they use the natural exponential growth function to find out how much your account will be worth at some future date.

**Continuously Compounding Interest Formula:**

$$
P_t=P_0e^{rt}
$$

Banks set their own lending rates. However, since interest rates fluctuate over time, commercial banks may use OIS's (Overnight Index Swaps) to manage their interest rate exposure. These OIS's exchange fixed payments for variable payments that are tied to the compounded overnight SONIA (Sterling Overnight Index Average) rate.

A key term is the "yield curve". It is a graph showing how lending rates change when you lend money for different lengths of time. A continuous yield curve represents the average instantaneous interest rate over an interval. A yield curve provides information about how interest rates vary between short-term and long-term investments.

**Yield Curve Equation:**

$$
\bar{r}(T)=\frac{1}{T}\int_0^T r(t)\,dt
$$

Lastly, inflation affects how valuable investments become. An investor may see their investment rise in monetary terms but experience a loss of purchasing power due to increased prices. Therefore, even though an investor may receive a certain interest rate on their loan or investment, he/she may lose purchasing power if inflation exceeds their investment return. To adjust for this effect of inflation on investing returns, the "inflation adjusted interest rate" should be considered. The inflation adjusted interest rate takes into consideration both the inflation rate and the effective interest rate.

**Inflation-Adjusted Interest Rate:**

$$
r_{\text{real}}=\frac{r_{\text{effective}}-i}{1+i}
$$

## My example

Suppose I invest £2,400 into a savings account offering a nominal annual interest rate of 4.8%, compounded quarterly. The investment will be held for three years.

### Step 1 – Compound Interest Calculation

In order to calculate the final amount for my £2,400 investment, I will utilise the compound interest formula. The investment earns interest quarterly; therefore, the interest is applied to the account 12 (four times per year * three years) times. Substituting the values for initial deposit, annual interest rate, number of times interest is compounded annually and length of time of the investment into the compound interest formula provides me with a final balance of approximately £2,769.35.

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
\boxed{P_3\approx \text{£2,769.35}}
$$

From this value, I can easily compute the profit by subtracting the original amount of £2,400 from the final amount. Therefore, the profit generated through compound interest over the three years is £369.35.

$$
\text{Profit}=2769.35-2400
$$

$$
\boxed{\text{Profit}=\text{£369.35}}
$$

### Step 2 – Effective Annual Interest Rate Calculation

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
r_{\text{effective}}\approx0.0488709
$$

$$
\boxed{r_{\text{effective}}\approx4.89\%}
$$

By utilising the formula for effective annual interest rates, I am able to compute an effective annual interest rate of 4.89%. This clearly illustrates that the effective interest rate is larger than the nominal interest rate when compounding occurs more than once per year.

### Step 3 – Comparison of Results Using Simple Interest vs. Compound Interest

Finally, I will compute how large the investment would grow if simple interest were utilised versus compound interest.

As stated earlier, unlike compound interest which utilises prior investments and their associated interest earnings in calculating future amounts owed, simple interest uses only the principal invested at the beginning of the period. As a consequence, simple interest calculations require less effort than those involving compound interest since no new amounts need to be computed every year. Utilising the simple interest formula, the amount due after three years would be £2,745.60.

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
\boxed{P_3=\text{£2,745.60}}
$$

**Difference between compound and simple interest:**

$$
2769.35-2745.60=\text{£23.75}
$$

When comparing the results from step 1 and step 3 above, we see that the investment grew slightly larger with compound interest (£2,769.35) than with simple interest (£2,745.60). Thus, we see the benefits provided by compound interest for creating wealth through generating interest on both principal deposited initially and prior-earned interest.

## Solved exercises

### Exercise 1 – Interest Rates and Compounding

#### Question

Suppose you invest £700 in a bank with a 3% nominal annual interest rate. In addition to finding out what the final value would be for your investment after three years with four different compounding options, find the effective annual rate for each option.

#### Part A – Finding the End Value of Your Investment

To start off we need to determine how much money your initial investment of £700 will have grown over a period of time of three years with four types of compounding.

**(i) Annually Compounded**

In an annually compounded interest type of loan (or deposit), the interest is paid on the principal once every one year. By applying the compound interest equation, the end balance of your deposit after three years should be about £764.91.

$$
P_3=700(1+0.03)^3
$$

$$
P_3=700(1.03)^3
$$

$$
\boxed{P_3\approx \text{£764.91}}
$$

**(ii) Monthly Compounded**

In a month-by-month type of compounding, the interest is compounded twelve times per year. Since you are investing for three years, there will be thirty-six monthly compounding periods. As previously described, the ending balance of your monthly type deposit can be calculated by applying the compound interest equation, and it is approximately £765.84.

$$
P_3=700\left(1+\frac{0.03}{12}\right)^{12\times3}
$$

$$
P_3=700(1.0025)^{36}
$$

$$
\boxed{P_3\approx \text{£765.84}}
$$

**(iii) Twice Per Year Type of Compounding (Semi-annually)**

A type of loan where interest is compounded two times per year has been referred to as semi-annually compounded. In a case like this, the number of compounding periods would equal six since the investor will be investing for three years. After plugging in all of the numbers in the compound interest equation, your deposit will be worth approximately £765.41.

$$
P_3=700\left(1+\frac{0.03}{2}\right)^{2\times3}
$$

$$
P_3=700(1.015)^6
$$

$$
\boxed{P_3\approx \text{£765.41}}
$$

**(iv) Continuously Compounded**

Continuous compounding is a type of compounding that happens infinitely often. Therefore instead of using the regular compound interest equation, we would apply the exponential growth formula to solve our problem. Based upon this information your continuously compounded deposit should equal approximately £765.92 after three years.

$$
P_3=700e^{0.03\times3}
$$

$$
P_3=700e^{0.09}
$$

$$
\boxed{P_3\approx \text{£765.92}}
$$

From looking at our answers from above, it can clearly be seen that the deposit which had continuous compounding produced the largest final value of deposits. Next was monthly compounding, followed by semi-annually compounding, and lastly annual compounding. It also shows that more frequent compounding will result in earning more interest based upon the fact that the nominal annual interest rate remained constant throughout this example.

#### Part B – Determining the Effective Rate of Return for Each Type of Loan/Deposit

Now, we need to figure out what your effective annual rate of return will be for each type of compounding used within this example.

Effective rate of return refers to your true annual return after adjusting for how many times during the course of a year interest is compounded.

**Effective Annual Interest Rate Formula:**

$$
r_{\text{effective}}=\left(1+\frac{r}{n}\right)^n-1
$$

**(i) Annually Compounded**

Your effective interest rate for annually compounded loans/deposits is going to be 3 per cent. As stated earlier in this solution section, interest on an annually compounded loan/deposit is only compounded once per year. Therefore, if you were to compare the nominal rate to your new effective rate they are going to be identical.

$$
r_{\text{effective}}=(1+0.03)^1-1
$$

$$
\boxed{r_{\text{effective}}=3.00\%}
$$

**(ii) Monthly Compounded**

If you choose to do monthly compounding, you will add your interest 12 times a year. To get your new effective rate of return, I will use the effective annual interest rate calculation. If you take the effective annual rate calculation formula and substitute in all of your values, you will arrive at an approximate rate of 3.0416 per cent.

$$
r_{\text{effective}}=\left(1+\frac{0.03}{12}\right)^{12}-1
$$

$$
\boxed{r_{\text{effective}}\approx3.0416\%}
$$

**(iii) Semi-annually Compounded**

Interest on a semi-annually compounded loan/deposit is compounded twice yearly. For semi-annually compounded loans/deposits, your effective annual rate of return will be approximately 3.0225 per cent.

$$
r_{\text{effective}}=\left(1+\frac{0.03}{2}\right)^2-1
$$

$$
r_{\text{effective}}=(1.015)^2-1
$$

$$
\boxed{r_{\text{effective}}=3.0225\%}
$$

**(iv) Continuously Compounded Interest**

The last type of compounding is continuous compounding. To calculate the effective annual interest rate in this method of compounding, you will need to use an exponential equation to calculate it. Continuous compounding differs from the others as there are no limits to how often interest is compounded.

**Effective Rate for Continuous Compounding:**

$$
r_{\text{effective}}=e^r-1
$$

$$
r_{\text{effective}}=e^{0.03}-1
$$

$$
\boxed{r_{\text{effective}}\approx3.0455\%}
$$

For example, if a person's nominal annual interest rate is 3%, their effective annual interest rate would be around 3.0455% using continuous compounding.

The best or highest of these four types of compounding was the continuously compounded interest rate. This demonstrates that for a fixed positive nominal rate, the more frequent the compounding interval, the higher your effective interest rate.

#### Part C – Finding Inflation-Adjusted Interest Rates

As we continue with the next part of the assignment, we are instructed to assume that there will be an average yearly inflation rate of 2%. Using this information, we must determine the inflation-adjusted interest rates for each of the four compounding types (annually, monthly, semi-annually, continuously).

As you might recall from previous coursework, inflation decreases your ability to purchase goods and services due to increasing costs. As such, even though investments may generate additional income through the interest they produce, their "real" return on investment will be affected by inflation. For example, if an investment produced a 10 per cent increase in the amount of money that you have available, but the cost of living increased by 9 per cent, then your actual increase in spending capacity was approximately 0.92 per cent.

There is a method that calculates the impact of inflation on investment returns; it is based on calculating both the effective annual interest rate associated with your investment and the inflation rate. This method is defined by the formula:

**Inflation-Adjusted Interest Rate Formula:**

$$
r_{\text{real}}=\frac{r_{\text{effective}}-i}{1+i}
$$

where $i$ is the inflation rate.

**(i) Annual Compound Interest Rate**

The effective interest rate for annually compounded investments is 3%. When the inflation factor of 2% is factored into this number, the resulting "true" interest rate is approximately 0.980%.

$$
r_{\text{real}}=\frac{0.03-0.02}{1.02}
$$

$$
\boxed{r_{\text{real}}\approx0.980\%}
$$

**(ii) Monthly Compound Interest Rate**

The effective interest rate for investments compounded monthly is 3.0416%. To calculate the true interest rate after taking inflation into account (an average inflation rate of 2%), we apply our inflation adjustment formula. The result is approximately 1.021%.

$$
r_{\text{real}}=\frac{0.0304159569-0.02}{1.02}
$$

$$
\boxed{r_{\text{real}}\approx1.021\%}
$$

**(iii) Semi-annual Compound Interest Rate**

The effective interest rate for investments compounded semi-annually is 3.0225%. By applying our inflation adjustment factor of 2%, we find that the true interest rate is approximately 1.002%.

$$
r_{\text{real}}=\frac{0.030225-0.02}{1.02}
$$

$$
\boxed{r_{\text{real}}\approx1.002\%}
$$

**(iv) Continuous Compound Interest Rate**

Continuous compounding results in an effective annual interest rate of 3.0455%. Once we adjust for an inflation factor of 2%, we find that the resulting true interest rate is approximately 1.025%.

$$
r_{\text{real}}=\frac{e^{0.03}-1-0.02}{1.02}
$$

$$
\boxed{r_{\text{real}}\approx1.025\%}
$$

**Comparison of Results**

When comparing all four methods, we can clearly see that all have had their real return decreased due to inflation. However, as before, continuous compounding generated the highest real return of all the methods.

It should come as no surprise that many financial experts agree that understanding the impact of inflation is essential when assessing whether an investment's return on investment has truly been successful.

#### Part D – How Long Will It Take to Grow Your Investment to £1,000?

Part D of this assignment asks us to determine how long it will take to grow an original investment of £700 to £1,000. We are given a nominal interest rate of 3% and informed that we will also be compounding interest twice during each year. In order to solve this problem we begin by substituting our variables into the compound interest formula. Unlike Parts A-C however, we are now looking for the length of time needed for our investment to become equal to £1,000.

We rearrange our compound interest formula to allow us to isolate our time variable.

**Compound Interest Formula:**

$$
P_t=P_0\left(1+\frac{r}{n}\right)^{nt}
$$

**Substituting the values:**

$$
1000=700\left(1+\frac{0.03}{2}\right)^{2t}
$$

$$
\frac{1000}{700}=(1.015)^{2t}
$$

Because our unknown quantity is raised to a power, we utilise natural logarithms in order to isolate and solve for our time variable.

$$
\ln\left(\frac{1000}{700}\right)=2t\ln(1.015)
$$

Rearranging:

$$
t=\frac{\ln(1000/700)}{2\ln(1.015)}
$$

$$
\boxed{t\approx11.98\text{ years}}
$$

Upon completion of these calculations, we determine that the investment would require approximately 11.98 years to grow from an initial investment of £700 to an ending investment value of £1,000.

Since interest is being added to your principal every six months, you would reach or surpass the value of £1,000 at the end of the twenty-fourth compounding interval or in twelve years.

As illustrated above, logarithmic techniques can provide a useful tool for determining how long an investment will need to grow in order to achieve a specific value.

### Exercise 6 – Comparing Credit Card Interest Rates

#### Question

Three credit card companies offer the following nominal annual interest rates:

- Company A: 23.4%, compounded daily.
- Company B: 23.5%, compounded monthly.
- Company C: 24.2%, compounded annually.

Which company offers the best deal for someone borrowing money?

#### Solution

In order to determine which of the three credit card companies (A, B & C) is offering the most competitive loan terms, we will have to make some calculations. We can do this by calculating the effective annual interest rate charged by each of them.

We cannot simply compare the nominal interest rates offered by each company as each has a differing compounding schedule. Thus, to accurately compare each of the three credit card companies' interest rates, we will have to use their respective compounding schedules to create an "effective" annual interest rate for each of the credit card companies. The effective annual interest rate takes into account the number of times interest is applied in one year.

**Company A – Daily Compounding**

Credit card Company A is advertising a 23.4% annual interest rate. This is the lowest nominal rate of all the credit cards being compared here, but it also states that it adds or compounds interest DAILY. Since there are 365 days in a calendar year, this means that interest will be added to your principal amount 365 times during the year. As you may recall from previous sections, we can convert the annual interest rate to an equivalent periodic interest rate using the following equation:

**Nominal Annual Rate:**

$$
r=n\times r_{\text{periodic}}
$$

Therefore, if we were to take the annual rate and divide it by the number of periods per year (365), we could get our periodic interest rate.

**Periodic Rate:**

$$
r_{\text{periodic}}=\frac{r}{n}
$$

$$
r_{\text{periodic}}=\frac{0.234}{365}
$$

$$
r_{\text{periodic}}\approx0.000641096
$$

Now that we know what the periodic interest rate is, we can apply the formula below to obtain our effective annual interest rate.

**Effective Annual Interest Rate:**

$$
r_{\text{effective}}=(1+r_{\text{periodic}})^n-1
$$

Substituting the value obtained above for the periodic rate into this formula we arrive at the following result.

$$
r_A=\left(1+\frac{0.234}{365}\right)^{365}-1
$$

$$
r_A\approx0.26354975
$$

$$
\boxed{r_A\approx26.35\%}
$$

As mentioned previously, we determined that Company A is charging an effective annual interest rate of 26.35%. While it is true that it has the lowest nominal interest rate of the three companies (at 23.40%), it also compounds every day. When we compound interest every day, we add or compound it 365 times per year. In contrast to both Companies B and C (which will be discussed next), Company A's compounding frequency creates an extremely high effective annual interest rate of 26.35%.

**Company B – Monthly Compounding**

While Company B has a slightly higher nominal annual interest rate than Company A at 23.50%, they only compound interest 12 times during any given year. Thus, although they advertise a nominal annual rate higher than Company A (23.5 vs. 23.4), due to their compounding occurring fewer times per year than Company A, they have a lower effective annual interest rate than does Company A.

Using similar reasoning as was used when obtaining the effective annual interest rate for Company A, we can substitute the appropriate values for this formula.

**Number of Times Interest Applied per Year:**

$$
n=12
$$

**Periodic Rate:**

$$
r_{\text{periodic}}=\frac{0.235}{12}
$$

$$
r_{\text{periodic}}\approx0.01958333
$$

**Effective Annual Interest Rate:**

$$
r_{\text{effective}}=(1+r_{\text{periodic}})^n-1
$$

Substituting in our values, we arrive at the following result.

$$
r_B=\left(1+\frac{0.235}{12}\right)^{12}-1
$$

$$
r_B\approx0.26203887
$$

$$
\boxed{r_B\approx26.20\%}
$$

Thus, after determining both the periodic and effective annual interest rates for Company B, we found that the effective annual interest rate is approximately 26.20%.

**Company C – Annual Compounding**

Company C's annual interest rate is stated as 24.2% with an annual compounding rate. The main difference between this company and the other two is that there is only one interest compounding period per year.

Because of this the annual compounding factor will equal 1 plus the nominal interest rate and thus the effective annual interest rate is also 24.20% using the effective annual interest rate equation.

$$
r_C=(1+0.242)^1-1
$$

$$
r_C=0.242
$$

$$
\boxed{r_C=24.20\%}
$$

**Interest Rate Comparison**

The calculated interest rates from above are compared in order to see which company would provide the best opportunity for a borrower.

| Company | Nominal Interest Rate | Compounding Frequency | Effective Annual Rate |
|---|---|---|---|
| A | 23.4% | Daily | 26.35% |
| B | 23.5% | Monthly | 26.20% |
| C | 24.2% | Annually | 24.20% |

**Summary Conclusion**

It can be seen by the comparison of the above calculated interest rates, Company C provides the most attractive terms for someone borrowing money due to having the smallest percentage interest charged annually.

## Spreadsheet

[01-InterestRates.xlsx](../spreadsheets/01-InterestRates.xlsx)

*Add a description of your Excel spreadsheet here, explaining what it calculates, which input cells can be changed and how the results respond to different interest rates or compounding frequencies.*
