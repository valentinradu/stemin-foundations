---
title: Superposition
---

::: card
When a circuit has more than one source, superposition lets you handle them one at a time. Kill
all but one (a voltage source becomes a wire, a current source an open gap), find what that
single source contributes, repeat for each, then add the contributions, respecting direction.
The sum is the real answer.
:::

::: card
It works because a resistive circuit is linear: double a source and its effect exactly doubles.
Ohm's law and Kirchhoff's laws contain no squared terms or products, so sources never interfere;
each contributes independently.
:::

::: card
One limit: superposition works for voltage and current, not power. Power is $I^2 R$, which is
nonlinear, so you cannot find the power in each sub-circuit and add them. It is especially useful
when sources run at different frequencies, which no single combined calculation can handle.
:::

::: card
Take a series loop with a 12 V source, a 6 V source opposing it, and a 2 Ω resistor. Kill the
6 V source: $I' = 12/2 = 6$ A. Kill the 12 V source: $I'' = 6/2 = 3$ A, opposing. The actual
current is $I = I' - I'' = 3$ A, matching the net EMF $12 - 6 = 6$ V across 2 Ω.
:::

::: exercise q1
A series loop has a 10 V source and a 4 V source opposing it, with a 3 Ω resistor. Use
superposition to find the current.

::: answer
2 A. Each source acting alone gives $10/3$ A and $4/3$ A in opposition; the difference is 2 A,
matching $(10-4)/3$.
:::

::: solution
Kill the 4 V source (short it). Only 10 V drives the loop:

$$ I' = \frac{10}{3}\ \text{A} $$

Kill the 10 V source. Only 4 V drives the loop, in the opposing direction:

$$ I'' = \frac{4}{3}\ \text{A} $$

The actual current is the difference:

$$ I = I' - I'' = \frac{10}{3} - \frac{4}{3} = 2\ \text{A} $$

matching the direct check $(10 - 4)/3 = 2$ A. ∎
:::
:::