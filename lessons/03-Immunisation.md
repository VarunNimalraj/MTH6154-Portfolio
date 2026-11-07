
# 3. Immunisation

[Back to contents](../README.md)

## Summary

Financial Mathematics employs immunisation techniques to provide protection to investors from changing interest rates. In the last week's session, I learned that Net Present Value (NPV) of a series of cash inflows/outs depend upon the current interest rate. A change in interest rate will result in a change to the NPV of future cash payments. As a consequence, an investment that was previously fairly priced could experience increased/decreased value due to this change. Thus creating Market Risk.

For a series of cash flows under continuous compounding, NPV is calculated using:

$$
NPV(r)=\sum_{i=0}^{n}C_i e^{-rt_i}
$$

When considering whether a financial transaction is fair/balanced in terms of Net Present Value (NPV), the consideration is based upon the fact that there is currently a zero NPV at the existing interest rate. If there were a change to the interest rate either upward/downward then the NPV would no longer be zero. The goal of Immunisation is to minimise the effects of such changes to the value of the investment.

There are several types of methods employed in achieving immunisation. One type is referred to as **First-Order Immunisation**. It takes place when the NPV is initially zero and its first derivative with respect to the prevailing interest rate is also equal to zero. Essentially, as long as small interest rate changes do not significantly affect the NPV; then the investment is insensitive to these changes.

**First-Order Immunisation Conditions:**

$$
NPV(r_0)=0
$$

$$
NPV'(r_0)=0
$$

First Order Immunisation does not guarantee protection from larger changes in interest rates. Therefore, an additional method of immunisation has been developed. This method is known as **Redington Immunisation**. There are three requirements to achieve Redington Immunisation. First, the NPV must be equal to zero at the existing interest rate. Second, the first derivative of NPV with respect to the interest rate must also be equal to zero. Thirdly, the second derivative of NPV must be greater than zero. This third condition guarantees that the NPV will have a local minimum of zero, so even if small changes occur in the interest rate they will not negatively affect the NPV.

**Redington Immunisation Conditions:**

$$
NPV(r_0)=0
$$

$$
NPV'(r_0)=0
$$

$$
NPV''(r_0)>0
$$

Understanding the differences between assets and liabilities is an equally important aspect of immunising investments. Assets include all positive cash flows you receive and liabilities represent those payments you must make. The total NPV is therefore derived by calculating the present value of your assets minus the present value of your liabilities. In order for the investment to be in balance at inception, both your asset(s) and liability(ies) must have present values that are equal.

**Net Present Value of Assets and Liabilities:**

$$
NPV(r)=NPV_+(r)-NPV_-(r)
$$

For the investment to be balanced at the prevailing interest rate:

$$
NPV_+(r_0)=NPV_-(r_0)
$$

Duration is another key factor related to immunising investments. Duration is defined as a measure of the weighted average amount of time until you receive your cash flows and their respective weights being established by the present values of each individual cash flow. Understanding duration provides insight into how sensitive your investment will be to potential changes in interest rates. Additionally, for investments involving positive cash flows and utilising continuous compounding; duration may also be expressed through use of the first derivative of present value.

**Duration Formula:**

$$
\tau=\frac{\sum_{i=1}^{n}t_iC_i e^{-rt_i}}{\sum_{i=1}^{n}C_i e^{-rt_i}}
$$

**Duration Using the Derivative of Present Value:**

$$
\tau=-\frac{PV'(r)}{PV(r)}
$$

In order for an investment to be immunised to first order, both the durations of your assets and liabilities must be equal and their respective present values must also be equal. This minimises the effect on your financial position resulting from small changes in interest rates.

**First-Order Immunisation of Assets and Liabilities:**

$$
NPV_+(r_0)=NPV_-(r_0)
$$

$$
\tau_+=\tau_-
$$

Finally, interest rates can vary depending on the compounding convention employed (e.g., annual vs. continuous). While differing compounding conventions require varying calculations, equivalent rates under these conventions give identical present values and therefore the criteria required for achieving Redington immunisation remains consistent across differing compounding conventions.

**Relationship Between Equivalent Interest Rates:**

$$
\frac{1}{1+r_a}=e^{-r_c}
$$

where $r_a$ is the annually compounded rate and $r_c$ is the continuously compounded rate.

Overall, Immunisation represents an important tool within financial institutions to manage interest rate risk. Through equating the durations and balancing your assets/liabilities, financial institutions are able to limit exposure from small variations in interest rates.

## My example

*Add your own worked example demonstrating immunisation of assets and liabilities.*

## Solved exercises

### Exercise 1 (from Tutorial Sheet 3)

*Add the first selected tutorial question and its solution here.*

### Exercise 2 (from Tutorial Sheet 3)

*Add the second selected tutorial question and its solution here.*

## Spreadsheet

[03-Immunisation.xlsx](../spreadsheets/03-Immunisation.xlsx)

*Add an explanation of what the spreadsheet calculates, which input cells can be changed, and how changes in interest rates affect the results.*
