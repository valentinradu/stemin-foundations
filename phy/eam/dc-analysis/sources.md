---
title: Two kinds of source
---

::: card
A **voltage source** fixes the voltage across its terminals and lets the current be whatever the
circuit demands. A battery is the common example: connect any load and the voltage stays
constant while the current adjusts. An ideal voltage source has zero internal resistance; a real
one sags slightly under heavy load.
:::

::: card
A **current source** is the mirror: it fixes the current through the circuit and lets the voltage
settle where it needs to. Connect any load and the current stays constant while the voltage
adjusts. Transistors in their active region and solar cells behave this way. An ideal current
source has infinite internal resistance.
:::

::: card
The distinction matters most when killing sources to find an equivalent. A voltage source set to
zero volts is a plain wire, so you replace it with one. A current source set to zero amps passes
nothing, so you replace it with a break: an open gap. Same logic, opposite result.
:::

::: exercise q1
To find a network's equivalent resistance you first kill its sources. What replaces a voltage
source, and what replaces a current source?

::: answer
A voltage source becomes a wire (zero volts is a short); a current source becomes an open gap
(zero amps passes nothing). Same logic, opposite result.
:::
:::