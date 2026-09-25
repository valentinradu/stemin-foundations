---
title: The RC time constant
---

::: card
The current at any moment is set by the voltage still available to drive it.

$$ I = \frac{V_s - V_\text{cap}}{R} $$
:::

::: card
That current adds charge to the capacitor, raising $V_\text{cap}$, which reduces the current,
which slows the charging further. A rate of change proportional to the remaining gap always
produces an exponential curve.
:::

::: card
After one $\tau$ the capacitor reaches 63% of the supply voltage, always, whatever the values.
After $5\tau$ it is at 99.3%, close enough to call done.[RC charging](reference:rc-charge)

$$ V_\text{cap}(t) = V_s\left(1 - e^{-t/\tau}\right) \qquad \tau = RC $$

```plot
x: { var: t, label: "$t$ in units of $\\tau$", from: 0, to: 5, ticks: 1, grid: true }
y: { label: "$V_\\text{cap} / V_s$", from: 0, to: 1.1 }

inputs:
  - { name: tau, min: 0.5, max: 2, default: 1, step: 0.1, label: "the time constant" }

draw:
  - hline: { at: 0.632, dash: true, label: "63%" }
  - vline: { at: tau, dash: true }
  - curve: { is: 1 - exp(-t / tau), accent: true }
  - point: { at: [tau, 0.632], label: "one $\\tau$" }
```
:::

::: card
Both $R$ and $C$ stretch $\tau$ the same way. A larger $R$ limits the current; a larger $C$ needs
more charge for the same voltage. Their product is the timescale in seconds: ohms times farads
are seconds.
:::

::: card
On discharge through a resistor the curve runs in reverse, falling with the same $\tau$. The
capacitor now acts as the source, driving current from its positive plate through the circuit
back to its negative.
:::

::: exercise q1
A 470 Ω resistor charges a 100 μF capacitor from a 12 V supply. What is the time constant, and
what voltage is across the capacitor after one time constant?

::: answer
$\tau = 47$ ms and $V \approx 7.58$ V. The time constant is $RC$; after one $\tau$ the capacitor
is at 63% of the supply.
:::

::: solution
The time constant:

$$ \tau = RC = 470 \times 100 \times 10^{-6} = 0.047\ \text{s} = 47\ \text{ms} $$

After one time constant the capacitor is at 63.2% of the supply:

$$ V = V_s\left(1 - e^{-1}\right) = 12 \times 0.632 = 7.58\ \text{V} $$

∎
:::
:::

::: reference rc-charge
# RC charging

A capacitor charging through a resistor approaches the supply voltage along an exponential, with
time constant $\tau = RC$.

::: equation
V_\text{cap}(t) = V_s\left(1 - e^{-t/\tau}\right) \qquad \tau = RC
:::

::: legend
$V_\text{cap}$: capacitor voltage, in volts
$V_s$: supply voltage, in volts
$t$: time, in seconds
$\tau$: time constant, in seconds
$R$: resistance, in ohms
$C$: capacitance, in farads
:::

::: derivation
The same current flows through the resistor and into the capacitor: $I = (V_s - V_\text{cap})/R$[Ohm's law](reference:ohms-law)
and $I = C\,dV_\text{cap}/dt$.[Capacitance](reference:capacitance)
Equate them: $C\dfrac{dV_\text{cap}}{dt} = \dfrac{V_s - V_\text{cap}}{R}$.
The rate of change is proportional to the remaining gap $V_s - V_\text{cap}$, which integrates
to an exponential approach.
With $V_\text{cap}(0) = 0$: $V_\text{cap}(t) = V_s\left(1 - e^{-t/RC}\right)$, so $\tau = RC$. ∎
:::
:::
