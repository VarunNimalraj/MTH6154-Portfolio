
# 2. Present value

[Back to contents](../README.md)

## Summary

Present value is an important concept in financial mathematics because money received today is worth more than the same amount received in the future. This is because money held today can be invested to earn interest. The **present value** of a future payment is the amount of money we would need to invest today to receive that payment at a later date.

To calculate present value, we use a **discount factor**, which converts a future amount of money into its value today. If interest is compounded annually at rate $r$, the discount factor is:

$$
D(t)=\frac{1}{(1+r)^t}
$$

Therefore, the present value of a future payment $P$ received at time $t$ is:

$$
PV=P\times D(t)=\frac{P}{(1+r)^t}
$$

If interest is compounded continuously, the discount factor becomes:

$$
D(t)=e^{-rt}
$$

Another important concept is **Net Present Value (NPV)**. This allows us to calculate the present value of multiple cash flows received at different times. We cannot simply add together payments received in different years because the value of money changes over time. Instead, each payment must be discounted to its present value before they are added together.

For a series of cash flows, the NPV is:

$$
NPV=\sum_{i=0}^{n}C_iD(t_i)
$$

where $C_i$ represents each cash flow and $t_i$ represents the time at which it occurs. An initial investment cost is treated as a negative cash flow.

When equal payments are received regularly, we can use a **geometric series** to simplify the calculation. If the same payment $C$ is received every year for $n$ years, the present value is:

$$
PV=C\sum_{i=1}^{n}\frac{1}{(1+r)^i}
$$

This can be simplified to:

$$
PV=C\frac{1-(1+r)^{-n}}{r}
$$

If the payments continue forever, this is known as a **perpetuity**. For a positive annual interest rate, its present value is:

$$
PV=\frac{C}{r}
$$

Present value is also affected by changes in interest rates. When interest rates increase, the present value of future payments decreases because those payments are discounted more heavily. Similarly, when interest rates decrease, the present value increases. This creates **market risk**, as changes in interest rates can affect the value of financial investments.

Another important concept is the **Internal Rate of Return (IRR)**, which is used to measure the return on an investment. The IRR is the discount rate that makes the net present value of an investment equal to zero.

For an initial investment $C_0$ and future cash flows $C_1,\ldots,C_n$, the IRR satisfies:

$$
0=-C_0+\frac{C_1}{1+r}+\frac{C_2}{(1+r)^2}+\cdots+\frac{C_n}{(1+r)^n}
$$

Here, $C_0$ represents a positive initial cost, while the other cash flows are payments received in future years.

The IRR can be compared with the prevailing interest rate to assess an investment. If the IRR is higher than the prevailing rate, the investment may be worthwhile. If it is lower, the investment may not offer a sufficient return.

For an investment with one initial cash outflow followed only by positive future cash flows, the NPV decreases as the discount rate increases. This means the IRR is unique.

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
