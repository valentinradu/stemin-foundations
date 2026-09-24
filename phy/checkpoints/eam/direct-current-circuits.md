---
title: Power and real circuits
---

::: exercise power-q1
A 4 Ω resistor carries 3 A. What power does it dissipate?

::: answer
$P = I^2 R = 3^2 \times 4 = 36\ \text{W}$. Use the $I^2 R$ form, since you know the current and
the resistance.
:::
:::

::: exercise power-q2
A lamp draws 0.26 A from a 230 V supply. What is its power rating?

::: answer
$P = V I = 230 \times 0.26 \approx 60\ \text{W}$. Multiply the voltage by the current.
:::
:::

::: exercise power-q3
A 2 kW heater runs for 3 hours a day. How much energy does it use per day, and what does that
cost at €0.22 per kWh?

::: answer
6 kWh, costing €1.32. Energy is power times time; cost is energy times the tariff.
:::

::: solution
Energy used in a day:

$$ W = P\,t = 2\ \text{kW} \times 3\ \text{h} = 6\ \text{kWh} $$

Cost at the tariff:

$$ 6\ \text{kWh} \times 0.22 = 1.32 $$

So €1.32 a day. ∎
:::
:::

::: exercise internal-resistance-q1
A real 12 V source has internal resistance 1 Ω and delivers 3 A. What is its terminal voltage?

::: answer
$U = \mathcal{E} - I r = 12 - 3 \times 1 = 9\ \text{V}$. Subtract the internal drop $I r$ from
the EMF.
:::
:::

::: exercise internal-resistance-q2
A 12 V battery with internal resistance $r = 0.5$ Ω feeds a 5.5 Ω heating element for 2 hours.
Find the current, the terminal voltage, the power delivered to the element, and the energy used.

::: answer
$I = 2\ \text{A}$, $U = 11\ \text{V}$, $P = 22\ \text{W}$, $W = 44\ \text{Wh}$. The internal
resistance and the element are in series.
:::

::: solution
The internal resistance and the element sit in series, so the EMF drives current through their
combined resistance:

$$ I = \frac{\mathcal{E}}{R + r} = \frac{12}{5.5 + 0.5} = 2\ \text{A} $$

The terminal voltage is the EMF minus the drop lost inside the battery:

$$ U = \mathcal{E} - I r = 12 - (2 \times 0.5) = 11\ \text{V} $$

Power delivered to the element, from the current and its resistance:

$$ P = I^2 R = 2^2 \times 5.5 = 22\ \text{W} $$

Energy is power times time:

$$ W = P\,t = 22 \times 2 = 44\ \text{Wh} = 0.044\ \text{kWh} $$

∎
:::
:::

::: exercise series-parallel-q1
Two 100 Ω resistors are connected in parallel. What is the equivalent resistance?

::: answer
50 Ω, half of one. A parallel combination is always smaller than the smallest resistor in it.
:::

::: solution
$$ \frac{1}{R_\text{eq}} = \frac{1}{100} + \frac{1}{100} = \frac{2}{100} $$

$$ R_\text{eq} = \frac{100}{2} = 50\ \Omega $$

∎
:::
:::

::: exercise series-parallel-q2
A 20 Ω and a 30 Ω resistor are in series across a 10 V supply. What current flows, and what is
the voltage across the 30 Ω resistor?

::: answer
$I = 0.2$ A, and 6 V across the 30 Ω resistor. Add the resistances, then use Ohm's law.
:::

::: solution
The resistances add in series:

$$ R_\text{eq} = 20 + 30 = 50\ \Omega $$

The current from Ohm's law:

$$ I = \frac{V}{R_\text{eq}} = \frac{10}{50} = 0.2\ \text{A} $$

The drop across the 30 Ω resistor:

$$ V_{30} = I R = 0.2 \times 30 = 6\ \text{V} $$

The remaining 4 V sits across the 20 Ω resistor, and the two drops add back to 10 V. ∎
:::
:::

::: exercise dc-vs-ac-q1
Why does alternating current cause far less electrolytic corrosion than direct current?

::: answer
Because the current reverses each half cycle. Ions migrate one way, then back, so the net
migration over a full cycle is nearly zero and the corrosion cancels.
:::
:::
