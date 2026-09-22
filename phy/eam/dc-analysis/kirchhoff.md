---
title: Kirchhoff's laws
---

::: card
Once a circuit splits into several loops that share components, Ohm's law alone stalls. Two laws
written by Gustav Kirchhoff in 1845 are enough between them to analyse any circuit. Both are
bookkeeping, one for charge and one for energy, each insisting nothing goes missing.
:::

::: card
**Kirchhoff's current law** is the bookkeeping for charge. At any junction, the current flowing
in equals the current flowing out.[current law](reference:kcl) Nothing piles up and nothing
vanishes. Picture water at a pipe junction: every litre a second in must leave by some branch.

$$ \sum I_\text{in} = \sum I_\text{out} $$
:::

::: card
**Kirchhoff's voltage law** is the bookkeeping for energy. Go round any closed loop, adding rises
and subtracting drops, and the total is zero.[voltage law](reference:kvl) The source lifts every
coulomb by exactly as much as the resistors drop it, so the sum is zero: not because nothing
happened, but because the source covered every drop exactly.

$$ \sum V = 0 $$
:::

::: card
The sign is simple: walk the loop in any direction; crossing a component from − to + is a rise,
from + to − is a drop. Two sources opposing each other count with opposite signs, and only the
net drives current.
:::

::: card
KCL and KVL look simple but they are powerful. Every method that follows, from mesh analysis to
Thévenin equivalents, is just one or both of them applied.
:::

::: exercise q1
A node has three wires. $I_1 = 6$ A flows in and $I_2 = 2$ A flows in. What does the third wire
carry, and in which direction?

::: answer
8 A, flowing out. By the current law, $6 + 2 = 8$ A in must leave the node.
:::
:::

::: exercise q2
A 9 V source, a 3 Ω resistor, and a 6 Ω resistor are in series. What is the drop across each, and
does the voltage law hold?

::: answer
$V_3 = 3$ V and $V_6 = 6$ V. The current is $9/(3+6) = 1$ A, the drops sum to 9 V, and
$9 - 3 - 6 = 0$, so the voltage law holds.
:::
:::