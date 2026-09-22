---
title: RC charging
uses: [ohms-law, capacitance]
---

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

A capacitor charging through a resistor approaches the supply voltage along an exponential, with
time constant $\tau = RC$.

::: derivation
The same current flows through the resistor and into the capacitor: $I = (V_s - V_\text{cap})/R$
and $I = C\,dV_\text{cap}/dt$.
Equate them: $C\dfrac{dV_\text{cap}}{dt} = \dfrac{V_s - V_\text{cap}}{R}$.
The rate of change is proportional to the remaining gap $V_s - V_\text{cap}$, which integrates
to an exponential approach.
With $V_\text{cap}(0) = 0$: $V_\text{cap}(t) = V_s\left(1 - e^{-t/RC}\right)$, so $\tau = RC$. ∎
:::