# 2. Present Value

[Back to contents](../README.md)

## Summary

The "present value" concept is used to calculate what money received in the future is worth today. Since money that you currently have available can earn interest, future money received by you must be multiplied by a discount factor to reflect its present-day value.

**Present Value Formula:**

$$
PV = F \times D(t)
$$

This discount factor depends on three elements; the interest rate or discount rate you are receiving; when you receive your money (the time period); and how often you compound the interest.

**Discount Factor (Annual Compounding):**

$$
D(t) = \frac{1}{(1+r)^t}
$$

**Discount Factor (Continuous Compounding):**

$$
D(t) = e^{-rt}
$$

When evaluating investments that result in many cash inflows at various points in time, net present value (NPV), which represents the total present value of all cash inflows and outflows, including the initial investment cost, can help you evaluate if the investment was a good one. To do this, each individual cash flow is discounted to present day value, then all of the values are added together, with costs treated as negative cash flows.

**Net Present Value Formula:**

$$
NPV = \sum_{i=0}^{n} C_i D(t_i)
$$

If there are regular cash inflows over long periods of time, geometric series may be able to assist in simplifying some of these calculations.

**Present Value of Equal Annual Payments:**

$$
PV = C\left(\frac{1-(1+r)^{-n}}{r}\right)
$$

In addition to regular and periodic cash inflows, there are perpetual cash flows, which are referred to as perpetuities.

**Present Value of a Perpetuity:**

$$
PV = \frac{C}{r}
$$

Additionally, changes in the interest rate will also cause changes in the present value of future cash inflows. An example would be; if the current interest rate increases, the present value of all future cash inflows associated with an investment will decrease. This creates a form of market risk for investors.

Internal Rate of Return (IRR) is defined as the interest rate where the Net Present Value (NPV) of an investment equals zero.

**Internal Rate of Return Formula:**

$$
0 = -I_0 + \sum_{i=1}^{n}\frac{C_i}{(1+IRR)^{t_i}}
$$

By comparing the IRR of an investment with other opportunities at the same point in time, it becomes easier to decide if an investment is a viable option.
