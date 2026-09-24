---
title: Reactance
---

::: card
A resistor opposes current by turning energy into heat, and its opposition $R$ is the same at any
frequency. Capacitors and inductors also oppose AC current, but they store the energy and give it
back, and their opposition depends on frequency. That frequency-dependent opposition is
**reactance**, $X$, measured in ohms, so it slots into Ohm's law as $V = I X$.
:::

::: card
The capacitor passes fast, blocks slow.[capacitive reactance](reference:capacitive-reactance)

$$ X_C = \frac{1}{\omega C} $$

High frequency gives a small $X_C$ and easy current; at DC ($\omega = 0$) it is infinite and
blocks completely.
:::

::: card
Nothing crosses the gap; electrons rush onto and off the plate, and that rushing in the wires is
the current. The faster the reversal, the less charge accumulates before it is yanked back, so
the plate's counter-field never builds and a large current flows. Slow it down and the plate
fills, its counter-field chokes the current, and at DC it stops.
:::

::: card
The inductor passes slow, blocks fast.[inductive reactance](reference:inductive-reactance)

$$ X_L = \omega L $$

High frequency gives a large $X_L$ and chokes the current; at DC it is zero, a plain wire.
:::

::: card
A changing current means a changing field, which induces a back-voltage opposing the change,
Lenz's law. On DC the steady field induces nothing. On AC the current never holds still, so the
field is always building and collapsing, always opposing, and the faster it changes the larger
that opposition.
:::

::: card
Both store rather than burn: over a full cycle an ideal one dissipates no heat. A capacitor
blocks DC and passes AC; an inductor passes DC and blocks AC. Pairing a resistor with one of them
is the basis of every filter, picking which frequencies get through.
:::

::: exercise q1
As the frequency rises, which passes more current, a capacitor or an inductor, and which passes
less?

::: answer
The capacitor passes more: $X_C = 1/\omega C$ falls as frequency climbs. The inductor passes
less: $X_L = \omega L$ rises. A capacitor favours high frequencies, an inductor low ones.
:::
:::

::: reference capacitive-reactance
# Capacitive reactance

A capacitor's opposition to alternating current falls as the frequency rises: it passes fast,
blocks slow. The reactance has units of ohms and enters Ohm's law as $V = I X_C$.

At high frequency $X_C$ is small and current flows easily; at DC ($\omega = 0$) it is infinite
and the capacitor blocks completely. The energy is stored and returned, not burned.

::: equation
X_C = \frac{1}{\omega C}
:::

::: legend
$X_C$: capacitive reactance, in ohms
$\omega$: angular frequency, in radians per second
$C$: capacitance, in farads
:::
:::

::: reference inductive-reactance
# Inductive reactance

An inductor's opposition to alternating current rises with the frequency: it passes slow, blocks
fast. The reactance has units of ohms and enters Ohm's law as $V = I X_L$.

At high frequency $X_L$ is large and chokes the current; at DC it is zero, a plain wire. The
energy is stored in the magnetic field and returned, not burned.

::: equation
X_L = \omega L
:::

::: legend
$X_L$: inductive reactance, in ohms
$\omega$: angular frequency, in radians per second
$L$: inductance, in henries
:::
:::
