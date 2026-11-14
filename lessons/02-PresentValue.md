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

## My Example

An investment with an initial cost of £900 would pay out £550 in one year's time, and £550 in two years' time. To determine if it's worth investing in at 10%, you need to calculate the present value of each payout as well as both payouts combined.

**Present Value Formula:**

$$
PV = \frac{FV}{(1+r)^t}
$$

**Present Value of the First Payment:**

$$
PV_1 = \frac{550}{1.10} = 500
$$

**Present Value of the Second Payment:**

$$
PV_2 = \frac{550}{(1.10)^2} \approx 454.55
$$

The total for the two payments is £1100 but because you don't get either of those until later, neither of the payments have their full values now. The first payment has a PV (present value) of £500; the second payment has a PV of about £454.55. The total PV of both payments is therefore £954.55.

**Total Present Value:**

$$
PV_{\text{total}} = 500 + 454.55 = 954.55
$$

Since your original investment was £900, your Net Present Value (NPV) from this investment would be roughly £54.55. With a positive NPV, the investment yields more than the 10% discount rate.

**Net Present Value Formula:**

$$
NPV = PV_{\text{total}} - I_0
$$

$$
NPV = 954.55 - 900
$$

$$
NPV = 54.55
$$

## Solved Exercises

### Exercise 1 – Internal Rate of Return

This task involves an investment of £1,000 at start-up. The first £500 payment occurs in year two. In year four, the second payment of £750 occurs.

The goal is to find out what the Internal Rate of Return (IRR) for the above investment would be.

In other words, this is the interest rate where the Net Present Value (NPV) of the investment is zero.

To achieve this, I have to discount each of the future cash flows to their current value.

Therefore, the sum of all the current value cash flows should equate to the amount of the original investment of £1,000.

**IRR Equation:**

$$
1000 = \frac{500}{(1+r)^2} + \frac{750}{(1+r)^4}
$$

Because the cash flows occur in years two and four, the calculations can be simplified using a single variable.

**Introducing a New Variable:**

$$
x = (1+r)^2
$$

After inserting this new variable into the existing formula, we get a quadratic equation.

$$
1000 = \frac{500}{x} + \frac{750}{x^2}
$$

Multiplying through by the squared variable:

$$
1000x^2 = 500x + 750
$$

Rearranging:

$$
x^2 - 0.5x - 0.75 = 0
$$

When you solve this quadratic equation, you will obtain two potential solutions for the new variable.

**Using the Quadratic Formula:**

$$
x = \frac{0.5 \pm \sqrt{0.25+3}}{2}
$$

$$
x_1 \approx 1.15139
$$

$$
x_2 \approx -0.65139
$$

However, as one of those potential solutions is negative and therefore could not possibly represent our needed growth factor, we must reject it.

**Calculating IRR:**

$$
(1+r)^2 = 1.15139
$$

$$
1+r = \sqrt{1.15139}
$$

$$
r = \sqrt{1.15139}-1
$$

$$
r \approx 0.0730 = 7.30\%
$$

Using the positive result from the previous step, we obtain an approximate IRR of 7.30%.

---

### Exercise 4 – Present Value of a Perpetuity

This question covers an infinite series of payments or a perpetuity that is paid £2,500 annually; the effective annual interest rate for this perpetual annuity is 4% p.a. A perpetuity refers to a sequence of equal, periodic payments that are made at fixed intervals indefinitely. This example examines the relationship between the timing of the first payment and the resultant present value of the perpetuity.

#### Part (a)

The initial payment is received after one year.

Because there will never be a final payment from this perpetuity, we may use a formula that divides the annual payment by the annual interest rate as follows:

**Present Value of a Perpetuity:**

$$
PV = \frac{C}{r}
$$

$$
PV = \frac{2500}{0.04}
$$

$$
PV = 62500
$$

£2,500 / .04 = £62,500

This represents the present value of the perpetuity, which begins with receipt of the first payment one year from now.

#### Part (b)

The first payment is received immediately.

Similar to Part (a), since we know the perpetuity's payments continue indefinitely, the present value will again be determined by dividing the annual payment by the effective annual interest rate.

However, unlike Part (a), we also have to add another £2,500 to the result from Part (a). This £2,500 is included in the present value because it is received today. Because this payment is received at the current time, we do not need to discount it. Therefore, the total present value of the perpetuity equals £65,000.

**Present Value Calculation:**

$$
PV = 2500 + \frac{2500}{0.04}
$$

$$
PV = 2500 + 62500
$$

$$
PV = 65000
$$

#### Part (c)

The first payment is received in ten years.

We have previously established that the perpetuity has a value of £62,500 at the end of Year 9. However, we wish to find its value at Time Zero. To accomplish this, we apply the discount factor for nine years to arrive at an approximate present value of £43,911.67.

**Discounting Back Nine Years:**

$$
PV_0 = \frac{62500}{(1+0.04)^9}
$$

$$
PV_0 = \frac{62500}{(1.04)^9}
$$

$$
PV_0 \approx 43911.67
$$

#### Summary

The above examples illustrate how the timing of receiving payments affects their present value. Receipts received earlier increase their present value while receipts delayed decrease their value.

## Spreadsheet

## Spreadsheet

[Download my Week 2 Excel spreadsheet](../spreadsheets/02-PresentValue.xlsx)
