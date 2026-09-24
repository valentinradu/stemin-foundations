---
title: Series and parallel
---

::: card
There are only two basic ways to connect components, and anything more complex is a mix of the
two.
:::

::: card
**Series** means end to end on a single path. The current has nowhere else to go, so it passes
through every component in turn. The same current flows everywhere. Each takes a share of the
voltage in proportion to its resistance, so resistances add.[series](reference:series-resistance)

$$ R_\text{series} = R_1 + R_2 $$
:::

::: card
A series string: one path, the same current through both resistors.

![A series string: one loop, one current through both resistors](assets/series.svg)
:::

::: card
**Parallel** means side by side, both ends joined to the same two points. The current has a
choice of routes and divides. Both components see the same voltage. Each branch draws its own
current, $I_1 = V / R_1$ and $I_2 = V / R_2$, and the totals add.[parallel](reference:parallel-resistance)

$$ \frac{1}{R_\text{parallel}} = \frac{1}{R_1} + \frac{1}{R_2} $$
:::

::: card
Two branches across the same two points: one voltage, the current splits.

![Two resistors in parallel across the same two points](assets/parallel.svg)
:::

::: card
A parallel combination is always lower than the smallest resistor in it. Every extra branch adds
another route for current, and more routes means more total current for the same voltage, so
lower resistance. Two 100 Ω resistors in parallel give 50 Ω; add a third and it drops to 33 Ω.
:::

::: card
A real source with EMF $\mathcal{E}$ and internal resistance $r$ driving two resistors. In series
the same current runs through both; in parallel it splits at the node, with more flowing through
the smaller resistance.

![A real source: its EMF, its internal resistance, and two resistors](assets/emf-internal.svg)
:::

::: exercise q1
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

::: exercise q2
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

::: reference parallel-resistance
# Resistances in parallel

Components side by side between the same two points see the same voltage. The reciprocals of
their resistances add.

$$ R_\text{parallel} = \frac{R_1 R_2}{R_1 + R_2} $$

::: equation
\frac{1}{R_\text{parallel}} = \frac{1}{R_1} + \frac{1}{R_2}
:::

::: derivation
Both branches sit across the same voltage $V$.
Each draws its own current by Ohm's law: $I_1 = V / R_1$ and $I_2 = V / R_2$.
The branch currents sum to the total: $I = I_1 + I_2 = V \left( \dfrac{1}{R_1} + \dfrac{1}{R_2} \right)$.
Dividing by $V$ gives $\dfrac{1}{R_\text{parallel}} = \dfrac{1}{R_1} + \dfrac{1}{R_2}$.
Combining the fractions gives $R_\text{parallel} = \dfrac{R_1 R_2}{R_1 + R_2}$. ∎

It rests on [Ohm's law](reference:ohms-law).
:::
:::

::: reference series-resistance
# Resistances in series

Components end to end on a single path carry the same current. Their resistances add.

::: equation
R_\text{series} = R_1 + R_2
:::

::: legend
$R_\text{series}$: total resistance, in ohms
$R_1$: first resistor, in ohms
$R_2$: second resistor, in ohms
:::

::: derivation
The same current $I$ flows through both, since the path does not branch.
Each drops a voltage by Ohm's law: $V_1 = I R_1$ and $V_2 = I R_2$.
The drops add to the total across the pair: $V = V_1 + V_2 = I (R_1 + R_2)$.
Dividing by $I$ gives $R_\text{series} = R_1 + R_2$. ∎

It rests on [Ohm's law](reference:ohms-law).
:::
:::
