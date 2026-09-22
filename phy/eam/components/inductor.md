---
title: The inductor
---

::: card
An inductor is a coil of wire. A single electron in a straight wire makes a weak field in rings
around it. Bend the wire into a loop and the rings through the inside all point the same way;
stack many loops and every turn adds its field through the centre. The coil is a magnet whose
strength is set by its current.
:::

::: card
Switch the current on from zero. The field grows, and a growing magnetic field induces a voltage
in any conductor around it: Faraday's law. The coil is that conductor, so the growing field
induces a voltage in the very coil that created it, pointing opposite to the battery.
:::

::: card
The result: current cannot jump. It climbs gradually, each step opposed by the field it just
produced. As it nears its final value the rate of change slows, the opposition shrinks, and the
current settles. Once steady, no change and no opposition: the coil is just a wire.
:::

::: card
Voltage across the inductor equals inductance times the rate of change of current.[inductor voltage](reference:inductor-voltage)
Steady current: zero voltage, invisible. Changing current: an opposing voltage proportional to
how fast it changes.

$$ V = L \frac{di}{dt} $$
:::

::: card
This is the mirror of the capacitor. A capacitor resists a change in voltage, blocks steady DC,
and holds its voltage when interrupted. An inductor resists a change in current, passes steady DC
like a wire, and throws a voltage spike when interrupted.
:::

::: card
**Inductance**, in henries, measures how strongly the coil opposes change. One henry: a current
changing at 1 A/s generates 1 V of opposition. More turns, larger loops, or an iron core all
raise it by strengthening the field per ampere.
:::

::: card
Every motor winding is an inductor; the rotating field that drives the rotor is built from them.
Transformer windings are inductors coupled through a shared iron core. The spike when an
inductor's current is cut is the arc you see breaking a circuit under load, and the reason
suppression diodes and capacitors sit across contactors and relay coils.
:::

::: exercise q1
Why does breaking a circuit under load produce an arc at the contacts, and what does it have to
do with inductors?

::: answer
An inductive load stores energy in its magnetic field. When the circuit breaks, the inductor
throws a high voltage spike trying to maintain its current; that voltage ionises the air across
the opening gap and sustains a brief arc. Suppression components give the energy somewhere else
to go.
:::
:::