---
title: Ohm's law
---

::: card
Three quantities, one relationship. Ohm's law says the current through a conductor equals the
voltage across it divided by its resistance.[Ohm's law](reference:ohms-law)

$$ I = \frac{V}{R} $$

More voltage drives more current; more resistance allows less.
:::

::: card
You will most often use it rearranged as $V = I R$, which gives the voltage drop across a
component from the current through it and its resistance. The third form, $R = V / I$, finds a
resistance from a measurement.
:::

::: card
Voltage is measured **across** a component: one probe on each terminal, from outside. A
voltmeter has very high internal resistance, so it draws almost no current and leaves the
voltage it is reading undisturbed.
:::

::: card
Current is measured **through** a component: the meter sits in the current path. Break the
circuit at one side and insert the ammeter in the gap. Its internal resistance is very low, so
it adds almost none to the circuit. A clamp meter reads the magnetic field around the wire
instead, so you never break the circuit at all.
:::

::: card
Drag the levers. The line is $I = V / R$ for the resistance you choose. Raise $R$ and the line
tilts flatter, so the same voltage produces less current.

```plot
x: { var: V, label: "$V$ in volts", from: 0, to: 12, ticks: 2, grid: true }
y: { label: "$I$ in amperes", from: 0, to: 6 }

inputs:
  - { name: R, min: 2, max: 12, default: 4, step: 1, label: resistance R }

draw:
  - curve: { is: V / R, accent: true }
```
:::

::: exercise q1
A 9 V supply is connected across a 3 Ω resistor. What current flows?

::: answer
$I = V / R = 9 / 3 = 3\ \text{A}$. Divide the voltage by the resistance.
:::
:::

::: exercise q2
A component carries 0.5 A when 6 V sits across it. What is its resistance?

::: answer
$R = V / I = 6 / 0.5 = 12\ \Omega$. Divide the voltage by the current.
:::
:::