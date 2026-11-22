
# 4. Bonds and the Term Structure of Interest Rates

[Back to contents](../README.md)

## Summary

Bonds (debt securities) are created in order for organisations and/or government agencies to acquire funds. When purchasing a bond, an investor has the possibility of receiving periodic interest payments called "coupons" along with acquiring the face amount (redemption value) at maturity. A zero-coupon bond does not issue periodic interest payments; it issues one payment at maturity.

**Present Value of a Zero-Coupon Bond:**

$$
PV=\frac{R}{(1+r)^T}
$$

An investor will use the present value method when calculating the cost of a bond. The present value is determined by using a formula that discounts both the future coupon payments from the bond and the redemption value of the bond.

**Present Value of a Coupon Bond:**

$$
PV=\sum_{t=1}^{T}\frac{C_t}{(1+r)^t}+\frac{R}{(1+r)^T}
$$

Where:

- \(C_t\) = Coupon payment at time \(t\)
- \(R\) = Redemption value
- \(r\) = Effective annual interest rate
- \(T\) = Time until maturity in years

According to the no-arbitrage principle, if there were two different investments available which had the exact same type and timing of cash flows then those investments would be priced identically otherwise, an investor could profit with virtually no risk.

**Law of One Price:**

$$
P_A=P_B
$$

A bond's yield represents the percentage rate of interest that will equate the present value of all future coupon payments and the redemption value of the bond with the current market price of the bond.

**Bond Yield Formula:**

$$
P_B=\sum_{t=1}^{T}\frac{C_t}{(1+y)^t}+\frac{R}{(1+y)^T}
$$

Where \(y\) is the bond yield and \(P_B\) is the market price of the bond.

Interest rates may differ based upon how long an individual invests their monies. The relationship that exists between time and interest rates is commonly referred to as the term structure of interest rates.

Spot rates are the effective annual interest rates for investments with different maturity dates. The forward rate represents the interest rate agreed to today for borrowing/lending money in future periods. These two rates are tied together by the no-arbitrage principle, which states that investing over consecutive time periods using the relevant forward rates will provide the same return as investing over the entire period at the corresponding spot rate.

**Spot Rate Discount Factor:**

$$
D(T)=\frac{1}{(1+s_T)^T}
$$

**Forward Rate Formula:**

$$
(1+f_{a,b})^{b-a}=\frac{(1+s_b)^b}{(1+s_a)^a}
$$

Where:

- \(s_T\) = Spot rate for maturity \(T\)
- \(f_{a,b}\) = Forward rate between years \(a\) and \(b\)
- \(a,b\) = Future times, with \(b>a\)

These formulas use effective annual rates and annual compounding.


## My Example – Calculating the Price of a Bond

Suppose an investor is considering purchasing a bond with a face value of £1,000, an annual coupon rate of 4%, and a maturity of 3 years. The market yield is 5%.

The investor's total cash receipts from the bond would consist of the periodic interest received (coupon income) and the amount received upon maturity. For example, in Year 1 the investor would have earned £40 as coupon income.

In addition to this, in Year 3, the investor would also receive the face amount of £1000. Therefore, for that year alone, the investor would receive £1040.

Each of these future cash flows should be discounted by the 5% market yield.

Therefore, we can determine the fair value of the investment by adding up all of the present value of each of these cash flows.

The sum of the present value of each of the cash flows is calculated as follows:

**Year 1:**

$$
PV_1=\frac{40}{1.05}=38.10
$$

**Year 2:**

$$
PV_2=\frac{40}{1.05^2}=36.28
$$

**Year 3:**

$$
PV_3=\frac{1040}{1.05^3}=898.39
$$

Therefore, the total present value is:

$$
PV=38.10+36.28+898.39
$$

$$
PV=972.77
$$

Thus, we find that the estimated price of the bond is approximately £972.77.


## Solved Exercises

### Exercise 1 – Bond Cash Flows

We have been provided with a 3 year bond, which has a nominal amount of £200,000 and has an annual coupon rate of 6%, paid semi-annually. The bond will be redeemed at par when it expires.

As we know that semi-annually, the investor will receive their coupon interest (and therefore the annual coupon rate is halved), we can calculate what each semi-annual payment will be as follows;

Annual Coupon Rate = 0.06

Coupon Interest Halved for Semi-Annually = 0.06 /2 = 0.03

Semi-Annual Payment = £200,000 x 0.03 = £6000

**Calculations:**

$$
\text{Semi-Annual Coupon Rate}=\frac{0.06}{2}=0.03
$$

$$
C=200,000\times0.03=6,000
$$

There will be six semi-annual payments made to the investor over the next three years. For the first five of these payments, the investor will receive £6000 on each occasion. On the sixth occasion (after the third year) the investor will receive both the last coupon interest of £6000 and the repayment of the bond's nominal amount of £200,000.

The sixth payment (£206,000) is comprised of both the last coupon payment (£6000) and the redemption value of the bond (£200,000).

$$
C_6=6,000+200,000=206,000
$$

Therefore, the investor’s cash flow stream is:

**(£6,000, £6,000, £6,000, £6,000, £6,000, £206,000).**

---

### Exercise 6 – Spot Rates and Forward Rates

We are told there are 1000 zero coupon bonds maturing after one year with an aggregate value of £931.00. There are also 1000 zero coupon bonds maturing after 3 years and they have an aggregate value of £785.00.

Hence each bond is valued at £0.931 and £0.785 respectively.

$$
V_1=\frac{931}{1000}=0.931
$$

$$
V_3=\frac{785}{1000}=0.785
$$

**Part (a) – Calculating Spot Rates**

To solve for the spot rates of the one year and three year bonds in (a) we will apply the zero-coupon bond pricing equation in reverse order to determine the appropriate interest rates.

The zero-coupon bond pricing formula is:

$$
V_T=\frac{1}{(1+s_T)^T}
$$

For the one-year bond:

$$
0.931=\frac{1}{1+s_1}
$$

$$
s_1=\frac{1}{0.931}-1
$$

$$
s_1\approx0.0741=7.4\%
$$

For the three-year bond:

$$
0.785=\frac{1}{(1+s_3)^3}
$$

$$
s_3=\left(\frac{1}{0.785}\right)^{1/3}-1
$$

$$
s_3\approx0.0840=8.4\%
$$

Spot rates were calculated to be 7.4% for the one year bond and 8.4% for the three year bond.

**Part (b) – Calculating the Forward Rate**

In (b) we want to compute the two year forward rate from Years 1-3. The forward rate can be found using the relationships among spot rates and forward rates. Forward rate was approximated as 8.9%.

Using the relationship:

$$
(1+f_{1,3})^2=\frac{(1+s_3)^3}{1+s_1}
$$

We can also express this using the zero-coupon bond prices:

$$
(1+f_{1,3})^2=\frac{V_1}{V_3}
$$

$$
(1+f_{1,3})^2=\frac{0.931}{0.785}
$$

$$
f_{1,3}=\sqrt{\frac{0.931}{0.785}}-1
$$

$$
f_{1,3}\approx0.089=8.9\%
$$

This is the agreed upon annual effective interest rate which has been agreed on today for the interval from the end of Year 1 to the end of Year 3.

