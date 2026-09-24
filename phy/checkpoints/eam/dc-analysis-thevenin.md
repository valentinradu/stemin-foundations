---
title: Thévenin equivalents
---

::: exercise thevenin-q1
A Thévenin equivalent has $V_\text{th} = 6$ V and $R_\text{th} = 2$ Ω. What load draws maximum
power, and what is that power?

::: answer
$R_L = 2$ Ω draws maximum power, 4.5 W. Maximum transfer is at $R_L = R_\text{th}$; then
$I = 6/(2+2) = 1.5$ A and $P = I^2 R_L = 4.5$ W.
:::
:::

::: exercise thevenin-q2
A 24 V source has $R_1 = 6$ Ω in series, and $R_2 = 12$ Ω from the junction to the negative
terminal. A load $R_L = 4$ Ω connects across $R_2$. Find the Thévenin equivalent the load sees
and the voltage across it.

::: answer
$V_\text{th} = 16$ V, $R_\text{th} = 4$ Ω, and $V_L = 8$ V. Open the load for $V_\text{th}$, kill
the source for $R_\text{th}$, then treat it as a divider.
:::

::: solution
Remove $R_L$. With the terminals open, the source still drives current through $R_1$ and $R_2$ in
series; the drop across $R_2$ is the open-circuit voltage:

$$ I = \frac{24}{6 + 12} = 1.33\ \text{A}, \qquad V_\text{th} = I R_2 = 16\ \text{V} $$

Kill the source (a wire). From the terminals, $R_1$ and $R_2$ are in parallel:

$$ R_\text{th} = \frac{R_1 R_2}{R_1 + R_2} = \frac{6 \times 12}{18} = 4\ \Omega $$

Connect the load. The equivalent is 16 V in series with 4 Ω:

$$ I_L = \frac{16}{4 + 4} = 2\ \text{A}, \qquad V_L = I_L R_L = 8\ \text{V} $$

∎
:::
:::
