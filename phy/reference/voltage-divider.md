---
title: Voltage divider
uses: [ohms-law, series-resistance, kvl]
---

::: equation
V_\text{out} = V_\text{in} \cdot \frac{R_2}{R_1 + R_2}
:::

::: legend
$V_\text{out}$: output voltage, in volts
$V_\text{in}$: input voltage, in volts
$R_1$: first resistor, in ohms
$R_2$: second (output) resistor, in ohms
:::

Two resistors in series across a supply tap a fraction of it at their junction. The output is the
supply scaled by the bottom resistor's share.

::: derivation
The two resistors form one series path, so the same current flows: $I = V_\text{in}/(R_1 + R_2)$.
The output sits directly across $R_2$, so it is the drop there: $V_\text{out} = I R_2$.
Substituting $I$: $V_\text{out} = V_\text{in} \cdot \dfrac{R_2}{R_1 + R_2}$. ∎
:::