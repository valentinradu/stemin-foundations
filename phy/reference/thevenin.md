---
title: Thévenin and Norton equivalents
uses: [voltage-divider, ohms-law]
---

::: equation
V_L = V_\text{th} \cdot \frac{R_L}{R_\text{th} + R_L} \qquad I_N = \frac{V_\text{th}}{R_\text{th}}
:::

::: legend
$V_L$: load voltage, in volts
$V_\text{th}$: Thévenin voltage, in volts
$R_\text{th}$: Thévenin resistance, in ohms
$R_L$: load resistance, in ohms
$I_N$: Norton current, in amperes
:::

Any network of sources and resistors, seen from two terminals, is one voltage source
$V_\text{th}$ in series with one resistance $R_\text{th}$ (Thévenin), or equivalently one current
source $I_N$ in parallel with the same $R_\text{th}$ (Norton).

::: derivation
With a load attached, the Thévenin form is a voltage divider of $V_\text{th}$ across
$R_\text{th}$ and $R_L$, giving $V_L$.
The Norton form agrees at both extremes: open the terminals and all of $I_N$ flows through
$R_\text{th}$, putting $I_N R_\text{th}$ across them, which must equal the open-circuit voltage
$V_\text{th}$; short the terminals and the current is $I_N$.
Agreeing at both ends, they agree for every load between, so $I_N = V_\text{th}/R_\text{th}$. ∎
:::