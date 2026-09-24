---
title: The three methods
---

::: exercise mesh-analysis-q1
Two meshes share a 4 Ω resistor. Mesh 1 also has a 12 V source and a 2 Ω resistor; mesh 2 also
has a 2 Ω resistor and no source. Find both mesh currents.

::: answer
$I_1 = 3.6$ A and $I_2 = 2.4$ A. Write the voltage law round each loop, the shared resistor
carrying the difference of the loop currents.
:::

::: solution
Mesh 1, clockwise:

$$ 12 = 2 I_1 + 4(I_1 - I_2) \;\Rightarrow\; 6I_1 - 4I_2 = 12 $$

Mesh 2, no source:

$$ 0 = 2 I_2 + 4(I_2 - I_1) \;\Rightarrow\; 6I_2 - 4I_1 = 0 \;\Rightarrow\; I_1 = 1.5 I_2 $$

Substitute:

$$ 6(1.5 I_2) - 4I_2 = 12 \;\Rightarrow\; 5I_2 = 12 \;\Rightarrow\; I_2 = 2.4\ \text{A}, \quad I_1 = 3.6\ \text{A} $$

∎
:::
:::

::: exercise nodal-analysis-q1
Node A connects to a 9 V source through $R_1 = 3$ Ω, and to ground through $R_2 = 9$ Ω. What is
the voltage at A?

::: answer
6.75 V. Apply the current law at A and solve.
:::

::: solution
Currents leaving A sum to zero:

$$ \frac{V_A - 9}{3} + \frac{V_A}{9} = 0 $$

Multiply through by 9:

$$ 3V_A - 27 + V_A = 0 \;\Rightarrow\; 4V_A = 27 \;\Rightarrow\; V_A = 6.75\ \text{V} $$

∎
:::
:::

::: exercise sources-q1
To find a network's equivalent resistance you first kill its sources. What replaces a voltage
source, and what replaces a current source?

::: answer
A voltage source becomes a wire (zero volts is a short); a current source becomes an open gap
(zero amps passes nothing). Same logic, opposite result.
:::
:::

::: exercise superposition-q1
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
