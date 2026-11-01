# 1. Interest rates

[Back to contents](../README.md)

## Summary

Interest rates determine how the value of money changes over time. If an initial amount of money is invested, the return is the difference between the final value and the initial investment. The percentage return is calculated using:

$$
R = \frac{P_t-P_0}{P_0}
$$

For an investment lasting $t$ years, the annualised simple rate of return is $r=R/t$.

An important concept is **compounding**, where interest is earned on both the original investment and previously accumulated interest. Under simple interest, the final amount is:

$$
P_t=P_0(1+rt)
$$

However, if interest is compounded $n$ times per year, the formula becomes:

$$
P_t=P_0\left(1+\frac{r}{n}\right)^{nt}
$$

Increasing the frequency of compounding increases the effective annual interest rate for a given positive nominal rate. The effective rate is:

$$
r_{\text{eff}}=\left(1+\frac{r}{n}\right)^n-1
$$

This is useful when comparing financial products that quote interest rates using different compounding frequencies.

Interest can also be **compounded continuously**, meaning that interest is added infinitely frequently. Using the exponential function, the accumulated amount is:

$$
P_t=P_0e^{rt}
$$

In practice, interest rates can change over time. The Bank of England sets its Bank Rate, while SONIA represents the average interest rate paid on eligible overnight sterling transactions. Banks also use overnight index swaps (OIS), which exchange fixed-rate payments for payments linked to compounded overnight rates.

Another important concept is the **yield curve**, which shows how interest rates vary depending on the maturity of an investment. For a continuously compounded instantaneous interest rate $r(t)$, the yield curve can be expressed as:

$$
\bar{r}(T)=\frac{1}{T}\int_0^T r(t)\,dt
$$

This represents the average continuously compounded interest rate over the period from 0 to $T$. Yield curves are useful because longer-term interest rates may differ from short-term rates.

Finally, **inflation** affects the real value of investment returns. Although an investment may increase in monetary value, rising prices reduce its purchasing power. The inflation-adjusted interest rate is:

$$
r_{\text{real}}=\frac{r_{\text{eff}}-i}{1+i}
$$

where $i$ is the inflation rate. This shows why the real return is more useful than the nominal return when assessing changes in purchasing power.


## My example

A situation you made up (your own numbers, not the ones in the lecture
notes), worked step by step.

## Solved exercises

### Exercise 1.x (from Exercise Sheet 1)

Question, then your solution.

## Spreadsheet

[01-InterestRates.xlsx](../spreadsheets/01-InterestRates.xlsx): what it
does, which cells to change and what to look at.
