
# 3. Immunisation

[Back to contents](../README.md)

## Summary

The idea behind immunisation is to minimise the impact on a portfolio of changing interest rates. As interest rates change, so does the present value of all future cash inflows (e.g., dividends) and outflows (e.g., debt repayment). Immunising the cash flow structure of an asset/liability pair involves managing those risks by structuring the cash flows from assets such that they offset the potential risks associated with the cash flows of the liability side of the same pair.

The net present value of an asset/liability position is:

$$
NPV(r)=V_A(r)-V_L(r)
$$

There are three levels of immunisation:

### 1. Zero-Order Immunisation

Zero order immunisation is achieved when, at the current market rate, the present value of assets equals the present value of liabilities. However, this equilibrium is generally destroyed when interest rates change.

The condition is:

$$
V_A(r_0)=V_L(r_0)
$$

Therefore:

$$
NPV(r_0)=0
$$

### 2. First-Order Immunisation

First Order Immunisation achieves some level of protection against rate risk by requiring the assets and liabilities to have equal durations, alongside zero-order immunisation. A bond's duration is the weighted average time until its cash flows are received, with the payments weighted according to their present values. The longer the duration, the greater the bond's sensitivity to changes in yields (i.e., interest rates).

The duration formula is:

$$
\tau=
\frac{\sum_{i=1}^{n}t_iC_iD(t_i;r)}
{\sum_{i=1}^{n}C_iD(t_i;r)}
$$

where \(D(t_i;r)\) is the discount factor for a payment received at time \(t_i\).

For first-order immunisation:

$$
\tau_A(r_0)=\tau_L(r_0)
$$

### 3. Redington Immunisation

Redington Immunisation further limits the rate risk by adding a requirement that the assets' convexity be at least as great as that of the liabilities. Convexity is a measure of how sensitive the sensitivity of present value is to changes in yield.

Convexity is calculated using:

$$
c(r)=\frac{V''(r)}{V(r)}
$$

The additional condition is:

$$
c_A(r_0)\geq c_L(r_0)
$$

Redington immunisation therefore requires matching present values and durations, alongside the convexity condition.

## My Example

Suppose you need to repay an amount of £1,050 in 2 years time. In order to plan for this repayment, you currently hold a couple of investments. One investment is expected to earn £500 in one year; the other investment will be worth £551.25 in three years. You also know the interest rate is 5% per annum, and that the interest is compounded on an annual basis.

You can now calculate the PV of both your investments and compare them to the PV of the payment you will make in two years. The combined PV of your investments and the PV of your liability are each approximately equal to £952.38. Therefore, at the given interest rate (and therefore at the same point in time), the position is zero-order immunised. However, having equal PVs will not protect you from a change in the interest rate. The payments are made at different times i.e. the first after one year and the second after three years. As long as they have equal PVs, their average payment time will be equivalent to two years. Similarly, your liability has a term of two years so the position is first-order immunised.

### Step 1: Present Values

The present value of the assets is:

$$
V_A=\frac{500}{1.05}+\frac{551.25}{(1.05)^3}
$$

$$
\boxed{V_A\approx £952.38}
$$

The present value of the liability is:

$$
V_L=\frac{1050}{(1.05)^2}
$$

$$
\boxed{V_L\approx £952.38}
$$

Therefore:

$$
V_A=V_L
$$

The zero-order immunisation condition is satisfied.

### Step 2: Duration

The duration of the assets is:

$$
\tau_A=
\frac{
1\left(\frac{500}{1.05}\right)
+
3\left(\frac{551.25}{(1.05)^3}\right)
}{
\frac{500}{1.05}
+
\frac{551.25}{(1.05)^3}
}
$$

$$
\boxed{\tau_A=2\text{ years}}
$$

The liability consists of one payment after two years:

$$
\boxed{\tau_L=2\text{ years}}
$$

Therefore:

$$
\tau_A=\tau_L
$$

The first-order immunisation condition is satisfied.

### Step 3: Convexity

Now, we can determine whether or not convexities of the investments are larger than those of the liabilities. If they are, then all of the conditions required by Redington's model have been met. The implications of Redington's model are that such a portfolio should provide a degree of protection against 'small' changes in interest rates (although there is no absolute guarantee).

With annual compounding, convexity is:

$$
c(r)=\frac{V''(r)}{V(r)}
$$

The convexity of the assets is:

$$
c_A=
\frac{
\frac{1(2)(500)}{(1.05)^3}
+
\frac{3(4)(551.25)}{(1.05)^5}
}{
\frac{500}{1.05}
+
\frac{551.25}{(1.05)^3}
}
$$

$$
\boxed{c_A\approx6.35}
$$

The convexity of the liability is:

$$
c_L=
\frac{
\frac{2(3)(1050)}{(1.05)^4}
}{
\frac{1050}{(1.05)^2}
}
$$

$$
\boxed{c_L\approx5.44}
$$

Since:

$$
c_A>c_L
$$

All three Redington immunisation conditions are satisfied.

---

## Solved Exercises

### Exercise 1: Duration of a Perpetuity

Finding the duration of a perpetuity is an example of determining the duration of a periodic series of payments that continue indefinitely and are equal in size.

Duration measures the average time at which the payments are received, with each payment weighted by its present value.

To find the duration I initially determine the present value of a perpetuity using the perpetuity formula. Then I apply the duration formula, and simplify this using a geometric series.

**Step 1: Present value of a perpetuity**

For an annual payment of \(C\) and an annual interest rate \(r\):

$$
PV=\sum_{t=1}^{\infty}\frac{C}{(1+r)^t}
=\frac{C}{r}
$$

**Step 2: Apply the duration formula**

$$
\tau=
\frac{
\sum_{t=1}^{\infty}\frac{tC}{(1+r)^t}
}{
\sum_{t=1}^{\infty}\frac{C}{(1+r)^t}
}
$$

Substituting the present value:

$$
\tau=
\frac{
\sum_{t=1}^{\infty}\frac{tC}{(1+r)^t}
}{
\frac{C}{r}
}
$$

$$
\tau=r\sum_{t=1}^{\infty}\frac{t}{(1+r)^t}
$$

**Step 3: Simplify using a geometric series**

Let:

$$
\beta=\frac{1}{1+r}
$$

Using the geometric series identity:

$$
\sum_{t=1}^{\infty}t\beta^t
=\frac{\beta}{(1-\beta)^2}
$$

Therefore:

$$
\tau=r\frac{\beta}{(1-\beta)^2}
$$

Substituting:

$$
\tau=
r\frac{\frac{1}{1+r}}
{\left(1-\frac{1}{1+r}\right)^2}
$$

$$
\tau=
r\frac{\frac{1}{1+r}}
{\left(\frac{r}{1+r}\right)^2}
$$

$$
\boxed{\tau=\frac{1+r}{r}}
$$

**Step 4: Interpretation**

My final answer determines the duration of a perpetuity as (1+r)/r. It illustrates how interest rates affect the duration. As interest rates increase, payments made at a later date are worth less than those made earlier. Therefore, since the interest rate has increased the duration will be decreased. Also if interest rates get close to zero, the duration approaches infinity.

Mathematically:

$$
\lim_{r\to\infty}\tau(r)=1
$$

$$
\lim_{r\to0^+}\tau(r)=\infty
$$

---

### Exercise 2: Present Value, Duration, Effective Duration and Convexity

This question calculates the present value, duration, effective duration and convexity for two different types of cash flow. In this case, we are given an interest rate of 4%, which will be compounded on a continuous basis.

Firstly, for Part (A) of the question, we have two payments; one payment of £1,000 after 2 years, and another payment of £500 after 3 years. We begin by calculating the present value. To do so, we apply the formula for compound interest with continuous compounding to discount both payments and sum them up. Therefore, our calculated present value was approximately £1,366.58.

We then go on to calculate the duration as follows: we multiply each discounted payment by the year it is due for receipt. Finally, we divide this result by the present value. As such, the resulting duration is approximately 2.32 years. Due to the fact that there is continuous compounding of interest, the effective duration is also equal to the duration. The convexity is approximately 5.62.

For Part (B) of the question, we are required to make payments of £1,500 in each of years 3 and 4. Therefore, we follow the same method of calculation as previously stated above. Consequently, we obtain a present value of approximately £2,608.60. Then we proceed to calculate the duration and effective duration for this type of liability, both of which are 3.49 years. Furthermore, the convexity is also calculated to be approximately 12.43.

Therefore, from the previous results we can see that the liability has a greater duration and convexity compared to the investment. The reason why this is the case is because of when the payments are due i.e. the liability had later payment times. Hence, the liability's present value is more sensitive to changes in the level of interest rates than that of the investment.

#### Part (A): Mathematical Working

**Step 1: Present Value**

With continuous compounding:

$$
PV=\sum_{i=1}^{n}C_i e^{-rt_i}
$$

Therefore:

$$
PV=1000e^{-0.04(2)}+500e^{-0.04(3)}
$$

$$
\boxed{PV\approx £1,366.58}
$$

**Step 2: Duration and Effective Duration**

Duration is:

$$
\tau=
\frac{\sum_{i=1}^{n}t_iC_ie^{-rt_i}}{PV}
$$

Therefore:

$$
\tau=
\frac{
2(1000e^{-0.08})+3(500e^{-0.12})
}{
1366.57656
}
$$

$$
\boxed{\tau\approx2.32\text{ years}}
$$

For continuous compounding:

$$
\nu=-\frac{V'(r)}{V(r)}=\tau
$$

Therefore:

$$
\boxed{\nu\approx2.32}
$$

**Step 3: Convexity**

For continuous compounding:

$$
c=
\frac{\sum_{i=1}^{n}t_i^2C_ie^{-rt_i}}{PV}
$$

Therefore:

$$
c=
\frac{
2^2(1000e^{-0.08})+3^2(500e^{-0.12})
}{
1366.57656
}
$$

$$
\boxed{c\approx5.62}
$$

#### Part (B): Mathematical Working

**Step 1: Present Value**

The liability consists of two payments of £1,500.

$$
PV=1500e^{-0.04(3)}+1500e^{-0.04(4)}
$$

$$
\boxed{PV\approx £2,608.60}
$$

**Step 2: Duration and Effective Duration**

$$
\tau=
\frac{
3(1500e^{-0.12})+4(1500e^{-0.16})
}{
2608.59634
}
$$

$$
\boxed{\tau\approx3.49\text{ years}}
$$

Since interest is compounded continuously:

$$
\boxed{\nu=\tau\approx3.49}
$$

**Step 3: Convexity**

$$
c=
\frac{
3^2(1500e^{-0.12})+4^2(1500e^{-0.16})
}{
2608.59634
}
$$

$$
\boxed{c\approx12.43}
$$

#### Comparison of Results

| Measure | Investment (A) | Liability (B) |
|---|---:|---:|
| Present Value | £1,366.58 | £2,608.60 |
| Duration | 2.32 years | 3.49 years |
| Effective Duration | 2.32 | 3.49 |
| Convexity | 5.62 | 12.43 |

---

## Spreadsheet

[Download my Week 3 Excel spreadsheet](../spreadsheets/03-Immunisation.xlsx)

