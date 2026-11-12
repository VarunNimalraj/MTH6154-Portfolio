
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

**Part (a)**

For this task you will invest £700 for 3 years at a fixed nominal interest rate of 3%, and with 4 different methods of compounding.

When the investment has matured after 3 years with annual compounding, it would have grown to £764.91. When your investment was compounded semi-annually, it would have grown to £765.41. Your investment would have increased to £765.84 if it had been compounded monthly. Lastly, if it had been compounded continuously during those 3 years, the total amount would have been approximately £765.92.

**Annual compounding:**

$$
FV=700(1+0.03)^3\approx764.91
$$

**Semi-annual compounding:**

$$
FV=700\left(1+\frac{0.03}{2}\right)^6\approx765.41
$$

**Monthly compounding:**

$$
FV=700\left(1+\frac{0.03}{12}\right)^{36}\approx765.84
$$

**Continuous compounding:**

$$
FV=700e^{0.03\times3}\approx765.92
$$

Each example illustrates the advantage of increasing the frequency of compounding when attempting to achieve the largest growth possible in the total value of your investment.

**Part (b)**

Now, you will determine what the effective annual interest rates were for all four methods employed in part (a).

The effective annual interest rate for the method of annual compounding was 3%.

The effective annual interest rate for the method of semi-annual compounding was 3.0225%. The effective annual interest rate for the method of compounding monthly was 3.0416%. The effective annual interest rate for the method of continuous compounding was 3.0455%.

**Effective annual interest rate formula:**

$$
r_{\text{effective}}=\left(1+\frac{r}{n}\right)^n-1
$$

**Annual:**

$$
(1+0.03)^1-1=0.03
$$

**Semi-annual:**

$$
\left(1+\frac{0.03}{2}\right)^2-1=0.030225
$$

**Monthly:**

$$
\left(1+\frac{0.03}{12}\right)^{12}-1\approx0.030416
$$

**Continuous:**

$$
e^{0.03}-1\approx0.030455
$$

As shown by these figures, the larger the number of times interest is compounded in a single year the greater the effective interest rate that is achieved due to that compounding.

**Part (c)**

There are two other types of interest rates in addition to the nominal interest rates described in part (a): the annual inflation rate of 2%. We shall therefore describe what the real interest rates were for each type of compounding in part (a) based upon the previous nominal interest rates.

The real interest rate generated by the method of annual compounding was 0.9804%. The real interest rate generated by the method of semi-annual compounding was 1.0025%. The real interest rate generated by the method of compounding monthly was 1.0212%. The real interest rate generated by the method of continuous compounding was 1.0250%.

**Real interest rate formula:**

$$
r_{\text{real}}=\frac{r_{\text{effective}}-i}{1+i}
$$

**Annual:**

$$
\frac{0.03-0.02}{1.02}\approx0.009804
$$

**Semi-annual:**

$$
\frac{0.030225-0.02}{1.02}\approx0.010025
$$

**Monthly:**

$$
\frac{0.0304159569-0.02}{1.02}\approx0.010212
$$

**Continuous:**

$$
\frac{e^{0.03}-1-0.02}{1.02}\approx0.010250
$$

These comparative analyses show how beneficial it is to compound investments more frequently than annually in order to reduce or mitigate against inflation's impact on an investor's wealth.

**Part (d)**

The last task is to calculate how many years it will require for an original deposit of £700 to grow into £1,000 provided that it earns an annual interest rate of 3% compounded semi-annually.

The general formula for determining future values is:

$$
FV=PV\left(1+\frac{r}{n}\right)^{nt}
$$

Where:

- FV = Future Value.
- PV = Present Value (£700).
- r = Nominal Annual Interest Rate (3%).
- n = Number of Times Per Year That Interest Is Compounded (2).
- t = Time Period For Which You Are Calculating This Investment (x).

To solve this equation for x you may take natural logarithms on both sides and remember that ln(a^x) = xln(a):

$$
\ln\left(\frac{FV}{PV}\right)
=(nt)\ln\left(1+\frac{r}{n}\right)
$$

$$
\ln\left(\frac{1000}{700}\right)
=\left(2\ln\left(1+\frac{0.03}{2}\right)\right)x
$$

$$
x=\frac{\ln(1000/700)}{2\ln(1+0.015)}
$$

**x ≈ 11.98 Years**

Therefore, since your investment is compounded every 6 months, your investment will reach £1,000 for the first time at the end of Year 12


### Exercise 6

The purpose of this comparative analysis is to evaluate the comparative cost of borrowing from three different credit card companies. The primary differences among these credit card companies include the amount of nominal interest they charge and how frequently they compound interest. Credit Card Company A compounds daily and charges a 23.4% annual nominal interest rate. Credit Card Company B compounds monthly and charges a 23.5% annual nominal interest rate. Credit Card Company C compounds annually and charges a 24.2% annual nominal interest rate.

In order to compare the effective borrowing costs of each credit card company, one must calculate each credit card company's Effective Annual Interest Rate. As previously stated, since interest can be compounded in many different manners within a calendar year, calculating each credit card company's Effective Annual Interest Rate will allow one to ascertain whether or not one credit card company is charging a lower effective interest rate per pound borrowed than another credit card company.

**Effective Annual Interest Rate Formula:**

$$
r_{\text{effective}}=\left(1+\frac{r}{n}\right)^n-1
$$

The calculated Effective Annual Interest Rates of each credit card company are as follows:

**Company A: 26.35%**

$$
r_A=\left(1+\frac{0.234}{365}\right)^{365}-1
$$

$$
r_A\approx0.26355
$$

**Company B: 26.20%**

$$
r_B=\left(1+\frac{0.235}{12}\right)^{12}-1
$$

$$
r_B\approx0.26204
$$

**Company C: 24.20%**

$$
r_C=(1+0.242)^1-1
$$

$$
r_C=0.242
$$

As indicated above, based upon the Effective Annual Interest Rates, Company C had the lowest Effective Annual Interest Rate. This is somewhat unexpected since Company C has the highest nominal interest rate of all three credit card companies. Two factors contributed to this occurrence. First, Companies A and B have a greater ability to compound their interest at a faster rate than does Company C. Second, even though Company C has a high nominal interest rate, its lower compounding frequency limits the total amount of compounding that takes place over the course of an entire year.

Consequently, using interest rates alone, Company C appears to offer the least expensive borrowing option of the three options compared.
## Spreadsheet
