---
title: The laws and the dividers
---

::: exercise kirchhoff-q1
A node has three wires. $I_1 = 6$ A flows in and $I_2 = 2$ A flows in. What does the third wire
carry, and in which direction?

::: answer
8 A, flowing out. By the current law, $6 + 2 = 8$ A in must leave the node.
:::
:::

::: exercise kirchhoff-q2
A 9 V source, a 3 Ω resistor, and a 6 Ω resistor are in series. What is the drop across each, and
does the voltage law hold?

::: answer
$V_3 = 3$ V and $V_6 = 6$ V. The current is $9/(3+6) = 1$ A, the drops sum to 9 V, and
$9 - 3 - 6 = 0$, so the voltage law holds.
:::
:::

::: exercise dividers-q1
A voltage divider has $R_1 = 18$ kΩ and $R_2 = 2$ kΩ, fed from 10 V. What is $V_\text{out}$?

::: answer
1 V. $V_\text{out} = 10 \times 2/(18 + 2) = 1$ V.
:::
:::

::: exercise dividers-q2
Two resistors in parallel, $R_1 = 10$ Ω and $R_2 = 40$ Ω, carry a total of 5 A. How much flows
through each?

::: answer
$I_1 = 4$ A and $I_2 = 1$ A. Each branch takes the share set by the *other* resistor:
$I_1 = 5 \times 40/(10+40)$, $I_2 = 5 \times 10/(10+40)$. The smaller resistor takes the larger
share.
:::
:::
