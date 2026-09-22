---
title: Current divider
uses: [ohms-law, parallel-resistance, kcl]
---

::: equation
I_1 = I_\text{total} \cdot \frac{R_2}{R_1 + R_2}
:::

::: legend
$I_1$: current in the first branch, in amperes
$I_\text{total}$: total current into the junction, in amperes
$R_1$: first branch resistance, in ohms
$R_2$: other branch resistance, in ohms
:::

A current arriving at two parallel branches splits between them. The share through one branch is
set by the *other* branch's resistance.

::: derivation
Both branches span the same two nodes, so both see the same voltage $V$: $I_1 = V/R_1$ and
$I_2 = V/R_2$.
The total is $I_\text{total} = V\left(\dfrac{1}{R_1} + \dfrac{1}{R_2}\right) = V\,\dfrac{R_1 + R_2}{R_1 R_2}$.
Solve for $V$ and substitute into $I_1 = V/R_1$:
$I_1 = I_\text{total} \cdot \dfrac{R_2}{R_1 + R_2}$. ∎
:::