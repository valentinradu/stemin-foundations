---
title: Terminal voltage
uses: [ohms-law]
---

::: equation
U = \mathcal{E} - I r
:::

::: legend
$U$: terminal voltage, in volts
$\mathcal{E}$: electromotive force, in volts
$I$: current drawn, in amperes
$r$: internal resistance, in ohms
:::

A real source carries a small internal resistance $r$ in series with the circuit. The voltage at
its terminals is its EMF less the drop lost across $r$.

::: derivation
The internal resistance $r$ carries the same current $I$ the source delivers.
By Ohm's law it drops a voltage $I r$ inside the source.
The EMF $\mathcal{E}$ is the source's voltage with no current flowing.
What reaches the terminals is the EMF less that internal drop: $U = \mathcal{E} - I r$. ∎
:::