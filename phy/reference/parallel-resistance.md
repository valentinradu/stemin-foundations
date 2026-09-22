---
title: Resistances in parallel
uses: [ohms-law]
---

::: equation
\frac{1}{R_\text{parallel}} = \frac{1}{R_1} + \frac{1}{R_2}
:::

Components side by side between the same two points see the same voltage. The reciprocals of
their resistances add.

$$ R_\text{parallel} = \frac{R_1 R_2}{R_1 + R_2} $$

::: derivation
Both branches sit across the same voltage $V$.
Each draws its own current by Ohm's law: $I_1 = V / R_1$ and $I_2 = V / R_2$.
The branch currents sum to the total: $I = I_1 + I_2 = V \left( \dfrac{1}{R_1} + \dfrac{1}{R_2} \right)$.
Dividing by $V$ gives $\dfrac{1}{R_\text{parallel}} = \dfrac{1}{R_1} + \dfrac{1}{R_2}$.
Combining the fractions gives $R_\text{parallel} = \dfrac{R_1 R_2}{R_1 + R_2}$. ∎
:::