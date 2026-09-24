---
title: Ampère's law and Maxwell's addition
---

::: card
Ampère's law in its original form: the magnetic field around a closed loop equals the total
current passing through the surface that loop encloses.

$$ \oint \mathbf{B} \cdot d\mathbf{l} = \mu_0 \, I_\text{through} $$
:::

::: card
For a straight wire this gives the field at distance $r$ directly: $B = \mu_0 I / (2\pi r)$.
Closer to the wire, stronger field; more current, stronger field.
:::

::: card
Maxwell found a contradiction at a capacitor. Current flows in the wire toward the plate, so
Ampère's law gives a field around it. But draw the surface through the gap between the plates
instead: no current crosses it. The same loop and boundary should give the same field, yet the
original law gives zero.
:::

::: card
As the capacitor charges, the electric field in the gap is growing. Maxwell showed a changing
electric flux acts identically to a real current for creating a magnetic field. He called it
displacement current and added it.[Ampère–Maxwell law](reference:ampere-maxwell)

$$ \oint \mathbf{B} \cdot d\mathbf{l} = \mu_0\left( I_\text{through} + \varepsilon_0 \frac{d\Phi_E}{dt} \right) $$
:::

::: card
Through the wire, the first term answers and the second is zero. Through the gap, the first is
zero and the second gives the same answer, because the rate of change of electric flux in the gap
exactly equals the wire current. Both surfaces, same loop, same result.
:::

::: exercise q1
A capacitor is being charged. No current crosses the gap between the plates, yet the magnetic
field around the gap is nonzero. What creates it?

::: answer
The growing electric field in the gap: Maxwell's displacement current. A changing electric flux
acts identically to a real current in Ampère's law, producing the same field as if current
crossed the gap.
:::
:::

::: reference ampere-maxwell
# The Ampère–Maxwell law

The magnetic field around a closed loop is set by the current through the enclosed surface plus
Maxwell's displacement current, the rate of change of electric flux.

The displacement term makes the law consistent for any surface bounded by the loop, including one
through a charging capacitor's gap.

::: equation
\oint \mathbf{B} \cdot d\mathbf{l} = \mu_0\left( I_\text{through} + \varepsilon_0 \frac{d\Phi_E}{dt} \right)
:::
:::
