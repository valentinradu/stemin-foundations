---
title: Thévenin and Norton
---

::: card
You have a circuit and want to try different loads on it: a motor, a sensor, a lamp. Each swap
means re-solving the whole circuit. Thévenin's theorem says you never have to.
:::

::: card
Any circuit of sources and resistors, however complex, looks from the outside like exactly one
battery in series with one resistor, $V_\text{th}$ and $R_\text{th}$, as seen from the two
terminals where the load connects. A different choice of terminals gives different values: they
belong to the circuit *as seen from those points*.

![A Thévenin equivalent: one source and one resistor, driving the load](assets/thevenin.svg)
:::

::: card
**$V_\text{th}$** is the open-circuit voltage: what you measure across the terminals with nothing
bridging them. The network is still alive inside, driving current through its own loops, and
$V_\text{th}$ is what it offers at those terminals with no load drawing current.
:::

::: card
**$R_\text{th}$** is the resistance the network presents at the terminals. To find it, kill all
sources first (a voltage source becomes a wire, a current source an open gap), then look in and
calculate what the remaining resistors form. Replacing a source with a wire does not short the
terminals: the resistors are still between them.
:::

::: card
With a load $R_L$ across the terminals, the Thévenin circuit is just a voltage
divider.[Thévenin equivalent](reference:thevenin)

$$ V_L = V_\text{th} \cdot \frac{R_L}{R_\text{th} + R_L} $$

Maximum power reaches the load when $R_L = R_\text{th}$: too small and most of $V_\text{th}$ drops
across $R_\text{th}$; too large and the current falls to near zero.
:::

::: card
Norton's theorem describes the same network the other way up: a current source $I_N$ in parallel
with the same $R_\text{th}$. Open the terminals and all of $I_N$ flows through $R_\text{th}$,
putting $I_N R_\text{th} = V_\text{th}$ across them; short them and the current is $I_N$. They
convert directly.

$$ I_N = \frac{V_\text{th}}{R_\text{th}} $$
:::

::: exercise q1
A Thévenin equivalent has $V_\text{th} = 6$ V and $R_\text{th} = 2$ Ω. What load draws maximum
power, and what is that power?

::: answer
$R_L = 2$ Ω draws maximum power, 4.5 W. Maximum transfer is at $R_L = R_\text{th}$; then
$I = 6/(2+2) = 1.5$ A and $P = I^2 R_L = 4.5$ W.
:::
:::

::: exercise q2
A 24 V source has $R_1 = 6$ Ω in series, and $R_2 = 12$ Ω from the junction to the negative
terminal. A load $R_L = 4$ Ω connects across $R_2$. Find the Thévenin equivalent the load sees
and the voltage across it.

::: answer
$V_\text{th} = 16$ V, $R_\text{th} = 4$ Ω, and $V_L = 8$ V. Open the load for $V_\text{th}$, kill
the source for $R_\text{th}$, then treat it as a divider.
:::

::: solution
Remove $R_L$. With the terminals open, the source still drives current through $R_1$ and $R_2$ in
series; the drop across $R_2$ is the open-circuit voltage:

$$ I = \frac{24}{6 + 12} = 1.33\ \text{A}, \qquad V_\text{th} = I R_2 = 16\ \text{V} $$

Kill the source (a wire). From the terminals, $R_1$ and $R_2$ are in parallel:

$$ R_\text{th} = \frac{R_1 R_2}{R_1 + R_2} = \frac{6 \times 12}{18} = 4\ \Omega $$

Connect the load. The equivalent is 16 V in series with 4 Ω:

$$ I_L = \frac{16}{4 + 4} = 2\ \text{A}, \qquad V_L = I_L R_L = 8\ \text{V} $$

∎
:::
:::