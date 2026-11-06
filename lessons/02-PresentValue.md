
# 2. Present Value

[Back to contents](../README.md)

## Summary

Present value is a significant idea in financial maths since money you have now is better than the same amount of money you get in the future. That's because if you keep your money instead of spending it right away, you can put it into an account where it earns interest. The amount of money we'd have to invest now to get a future payment is called the present value of the future payment.

In order to determine the present value, we'll need to know what is called a "discount factor". A discount factor will take a future dollar amount and convert it to dollars today. The formula for the discount factor depends upon whether or not interest is compounded annually. If interest is compounded annually, then the discount factor formula can be determined from two variables: the annual interest rate and how many years it takes for the payment to arrive.

**Discount Factor (Annual Compounding):**

$$
D(t)=\frac{1}{(1+r)^t}
$$

**Present Value Formula:**

$$
PV=P\times D(t)=\frac{P}{(1+r)^t}
$$

Additionally, there is another formula for the discount factor depending upon if interest compounds continuously. The continuous compounding discount factor uses the e^(-rt) notation (where r is the annual interest rate expressed as a decimal, t is the total number of years, and e represents Euler's Number).

**Discount Factor (Continuous Compounding):**

$$
D(t)=e^{-rt}
$$

Net Present Value (NPV) allows us to find the present value of multiple cash inflows that occur at different points in time. We can't just add up all the cash flows that occur during different years because the value of money will change over time. Each individual cash flow needs to be discounted back to its current value prior to being summed with other values.

We can compute the NPV of a series of cash flows by multiplying each cash flow by its appropriate discount factor and summing them together. Any upfront costs associated with making an initial investment will be treated as a negative cash flow.

**Net Present Value Formula:**

$$
NPV=\sum_{i=0}^{n}C_iD(t_i)
$$

A geometric series can help us simplify our calculations when we have a series of cash flows received at equal intervals. If we make a consistent payment each year for some period of time, we can utilise a geometric series to determine the PV of those payments.

**Present Value of Regular Payments:**

$$
PV=C\sum_{i=1}^{n}\frac{1}{(1+r)^i}
$$

This can be simplified to:

$$
PV=C\frac{1-(1+r)^{-n}}{r}
$$

If the cash flows never cease; i.e., they go on indefinitely, we call these "perpetuities." With respect to a positive annual interest rate, we can easily solve for the PV of a perpetual cash flow by dividing the constant periodic payment by the applicable interest rate.

**Present Value of a Perpetuity:**

$$
PV=\frac{C}{r}
$$

Also, changes in interest rates impact present value. When interest rates rise, the PV of future payments fall because those payments are being discounted more heavily. Conversely, when interest rates drop, the PV rises. Therefore, this creates market risk since changing interest rates can impact the value of financial assets.

Finally, we should discuss Internal Rate of Return (IRR); which is used as an indicator of the return on an investment. The IRR is defined as that discount rate that produces a net present value (NPV) of zero for an investment.

**Internal Rate of Return Formula:**

$$
0=-C_0+\frac{C_1}{1+r}+\frac{C_2}{(1+r)^2}+\cdots+\frac{C_n}{(1+r)^n}
$$

Comparing IRR to available interest rates helps evaluate an investment. If IRR exceeds available interest rates, then presumably the investment has merit. However, if IRR falls short of prevailing interest rates, then perhaps the investment does not provide enough return.

Investments with one initial outlay followed only by additional positive returns will result in decreasing NPVs as the discount rate increases. In such cases, IRR will always be unique.

## My example

Suppose an investor pays £1,000 for an investment that provides £400 at the end of each year for three years. The prevailing annual effective interest rate is 5%.

To determine whether the investment is worthwhile, we calculate the present value of the three future payments.

The present value is:

$$
PV=\frac{400}{1.05}+\frac{400}{1.05^2}+\frac{400}{1.05^3}
$$

Discounting each payment gives:

$$
PV=380.95+362.81+345.54
$$

Therefore:

$$
PV\approx £1,089.30
$$

We then subtract the initial investment cost to calculate NPV:

$$
NPV=1089.30-1000
$$

$$
\boxed{NPV=£89.30}
$$

Since the NPV is positive, the present value of the future payments exceeds the initial investment cost. Therefore, the investment would be worthwhile at the given discount rate.

## Solved exercises

### Exercise 1 (from Tutorial Sheet 2)

*Add the first selected tutorial question and its solution here.*

### Exercise 2 (from Tutorial Sheet 2)

*Add the second selected tutorial question and its solution here.*

## Spreadsheet

[02-PresentValue.xlsx](../spreadsheets/02-PresentValue.xlsx)

*Add a short explanation of what the spreadsheet calculates, which input cells can be changed, and how the results respond to those changes.*
