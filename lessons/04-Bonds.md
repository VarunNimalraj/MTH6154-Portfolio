
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

