---
title: Real sources
---

::: card
So far the battery has been a perfect push that never weakens. A perfect source has no internal
resistance, so its terminal voltage equals its EMF however much current you draw. Real sources
are less generous.
:::

::: card
A real battery has a small resistance inside it, in the materials and connections of the cell.
We call it **internal resistance**, written $r$. It sits in series with the rest of the circuit,
so every ampere drawn must push through it first.
:::

::: card
The battery's voltage with nothing connected and no current flowing is the **electromotive
force**, or **EMF**, written $\mathcal{E}$. Draw current $I$ and a drop of $I r$ is lost inside
the battery. What remains at the terminals is the **terminal voltage** $U$.[terminal voltage](reference:terminal-voltage)

$$ U = \mathcal{E} - I r $$
:::

::: card
A healthy car battery has $r$ around 0.02 Ω. When the starter pulls 150 A, the internal drop is
$150 \times 0.02 = 3$ V, pulling the terminal voltage from 12 V to 9 V. Every branch, including
the headlights, now sees 9 V instead of 12 V, so they dim. The dimming is the signature of $r$.
:::

::: card
An old battery with $r = 0.4$ Ω cannot deliver 100 A at all: the formula gives a negative
terminal voltage, which tells you the model has broken down and the battery collapses before
reaching that current. High internal resistance is why a weak battery fails on a cold morning.
:::

::: exercise q1
A real 12 V source has internal resistance 1 Ω and delivers 3 A. What is its terminal voltage?

::: answer
$U = \mathcal{E} - I r = 12 - 3 \times 1 = 9\ \text{V}$. Subtract the internal drop $I r$ from
the EMF.
:::
:::

::: exercise q2
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