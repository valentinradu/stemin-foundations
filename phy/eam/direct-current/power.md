---
title: Power and energy
---

::: card
Each coulomb picks up energy from the source and spends it in the circuit. Power is the rate at
which that happens.[power](reference:power) Voltage is joules per coulomb, current is coulombs per
second; multiply them and the coulombs cancel, leaving joules per second, which is **power**,
$P$, in **watts**.

$$ P = V I \qquad 1\ \text{W} = 1\ \text{J/s} $$
:::

::: card
One watt is one joule per second. A 2 kW heater uses 2000 joules every second, about the output
of ten people cycling hard. Your body at rest gives off about 80 W of heat, which is why a
packed room gets warm.
:::

::: card
Because Ohm's law locks $V$, $I$, and $R$ together, you can write power two other ways when you
know only two of the three.

$$ P = V I = I^2 R = \frac{V^2}{R} $$
:::

::: card
The $I^2 R$ form matters most on the job. Power rises with the square of the current: double the
current and the power quadruples. More coulombs arrive each second, and each falls through a
larger drop $V = I R$, so the two effects multiply. This is why an overloaded cable heats
fiercely and why cable sizing is a safety matter.
:::

::: card
Power is the rate; energy is the running total. Run $P$ watts for time $t$ and the energy adds
up as $W = P t$. Joules are too small for the household, so the meter counts kilowatt-hours: one
kilowatt held for one hour.

$$ W_{\text{kWh}} = \frac{P_{\text{W}}}{1000} \times t_{\text{hours}} $$
:::

::: card
Choose a load and its hours per day to see the monthly cost at €0.22 per kWh, the rough European
residential tariff.

```plot
x: { var: h, label: "hours a day", from: 0, to: 24, ticks: 4, grid: true }
y: { label: "euro a month", from: 0, to: 200 }

inputs:
  - { name: P, min: 100, max: 2500, default: 1000, step: 100, label: load in watts }

draw:
  - curve: { is: P / 1000 * h * 30 * 0.22, accent: true }
```
:::

::: exercise q1
A 4 Ω resistor carries 3 A. What power does it dissipate?

::: answer
$P = I^2 R = 3^2 \times 4 = 36\ \text{W}$. Use the $I^2 R$ form, since you know the current and
the resistance.
:::
:::

::: exercise q2
A lamp draws 0.26 A from a 230 V supply. What is its power rating?

::: answer
$P = V I = 230 \times 0.26 \approx 60\ \text{W}$. Multiply the voltage by the current.
:::
:::

::: exercise q3
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