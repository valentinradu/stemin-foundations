---
title: Nodal analysis
---

::: card
**Nodal analysis** attacks the same deadlock from the other end: instead of loop currents, work
with the voltage at each junction. Pick one junction as ground (0 V); every other voltage is
measured from it. Then at each remaining junction apply the current law: the currents leaving
must sum to zero.
:::

::: card
Take one free node A. A 12 V source feeds A through $R_1 = 2$ Ω; from A, $R_2 = 6$ Ω and
$R_3 = 3$ Ω drain to ground. Write the current law at A as the sum of currents leaving, using
(this node − far node)/R for each branch:

$$ \frac{V_A - 12}{2} + \frac{V_A}{6} + \frac{V_A}{3} = 0 $$
:::

::: card
The first term comes out negative when $V_A < 12$ V, meaning current actually enters A from the
source. The sign handles direction automatically. Multiplying through by 6:

$$ 3(V_A - 12) + V_A + 2V_A = 0 $$

$$ 6V_A = 36 \;\Rightarrow\; V_A = 6\ \text{V} $$
:::

::: card
Branch currents check out: $I_1 = (12-6)/2 = 3$ A in, $I_2 = 6/6 = 1$ A out, $I_3 = 6/3 = 2$ A
out, and $3 = 1 + 2$. Each non-ground junction costs one equation, just as each loop costs one in
mesh. Count loops, count free junctions, pick the smaller.
:::

::: exercise q1
Node A connects to a 9 V source through $R_1 = 3$ Ω, and to ground through $R_2 = 9$ Ω. What is
the voltage at A?

::: answer
6.75 V. Apply the current law at A and solve.
:::

::: solution
Currents leaving A sum to zero:

$$ \frac{V_A - 9}{3} + \frac{V_A}{9} = 0 $$

Multiply through by 9:

$$ 3V_A - 27 + V_A = 0 \;\Rightarrow\; 4V_A = 27 \;\Rightarrow\; V_A = 6.75\ \text{V} $$

∎
:::
:::