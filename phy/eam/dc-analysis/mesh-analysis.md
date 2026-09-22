---
title: Mesh analysis
---

::: card
Once a circuit has more than one loop sharing branches, you hit a chicken-and-egg problem: to use
the voltage law on a loop you need the current in every resistor, but those currents are what you
are trying to find. There is nowhere to start.
:::

::: card
**Mesh analysis** breaks the deadlock. Instead of the real branch currents, imagine one current
circulating around each loop, all clockwise: $I_1$, $I_2$, and so on. A branch in one loop
carries that loop's current; a branch shared by two loops has both running through it in opposite
directions, so its real current is the difference.
:::

::: card
Write the voltage law once around each loop, each drop being current times resistance. A shared
resistor drops its resistance times the difference of the two loop currents, since that is what
really flows through it. Each loop gives one equation; with as many equations as unknowns you
solve the lot.
:::

::: card
Take two meshes: an 18 V source and $R_1 = 3$ Ω in mesh 1, a shared $R_2 = 6$ Ω, and $R_3 = 2$ Ω
with $R_4 = 4$ Ω in mesh 2. The voltage law clockwise round mesh 1:

$$ 18 - 3I_1 - 6(I_1 - I_2) = 0 $$
$$ 9I_1 - 6I_2 = 18 $$

Mesh 2 has no source:

$$ 6(I_2 - I_1) + 2I_2 + 4I_2 = 0 $$
$$ 6I_1 = 12I_2 $$
:::

::: card
The second equation gives $I_1 = 2I_2$. Substituting into the first:

$$ 9(2I_2) - 6I_2 = 18 $$
$$ I_2 = 1.5\ \text{A}, \quad I_1 = 3\ \text{A} $$

The real current through the shared $R_2$ is $I_1 - I_2 = 1.5$ A. Each loop costs one equation, so
mesh analysis is quickest when a circuit has few loops.
:::

::: exercise q1
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