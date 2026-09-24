---
title: The capacitor
---

::: card
A capacitor is two metal plates facing each other with an insulating gap between them: air,
plastic, or ceramic. No electrons cross the gap.
:::

::: card
Connect a battery. It pushes electrons onto the negative plate; their combined field reaches
across the gap and pushes electrons off the positive plate, which flow out through the circuit
and back to the battery. Current flows in the whole circuit even though nothing crosses the gap:
the field couples the two halves.
:::

::: card
Both terminals are essential. The second is the escape route for the electrons pushed off the
positive plate. Without it they pile up at once and block any further charging, like a clogged
pipe: pressure builds but nothing flows.
:::

::: card
As the capacitor charges, its own voltage grows and opposes the battery. Less voltage across the
resistor means less current, so slower charging. The fuller it gets, the slower it fills.
Eventually its voltage matches the battery: zero across the resistor, zero current, charging
stops.
:::

::: card
At full charge it holds its voltage but passes no current, the opposite of a wire. A wire passes
current and drops no voltage; a charged capacitor drops the full voltage and passes none. In
series in a DC circuit it charges up, then the circuit is effectively broken.
:::

::: card
For alternating current the picture reverses. The voltage keeps changing direction, so the
capacitor never fully charges before the voltage reverses and discharges it. To AC it looks like
it conducts, current flowing in and out of the plates, though nothing ever crosses the gap.
:::

::: card
**Capacitance**, in farads, is how much charge is needed to reach a given voltage.[capacitance](reference:capacitance)
Large plates close together: strong coupling, large capacitance. Small plates far apart: weak
coupling, small.

$$ Q = C V $$
:::

::: card
The capacitors an electrician meets most are motor start and run capacitors. A single-phase
motor cannot start alone: its field does not rotate. A start capacitor shifts the phase of a
second winding to get it spinning, then disconnects; a run capacitor stays in, improving torque.
A failed run capacitor leaves the motor humming but not starting.
:::

::: exercise q1
A capacitor is fully charged and the battery is disconnected. Is there voltage across the
terminals? Does current flow?

::: answer
Voltage yes, current no. The charge imbalance holds the voltage indefinitely, but with no path
to discharge, nothing flows. A charged, isolated capacitor is the opposite of a wire.
:::
:::

::: exercise q2
An air-conditioning compressor starts sluggishly, drawing high current but barely turning. Why
would a failed run capacitor cause this?

::: answer
The run capacitor shifts the phase of the second winding to keep the field rotating. Without it
the rotating field weakens, so the motor cannot develop torque: it draws high current trying to
accelerate but cannot.
:::
:::

::: reference capacitance
# Capacitance

Capacitance is how much charge a capacitor holds per volt across it. The charge stored is the
capacitance times the voltage.

A farad is one coulomb per volt. Large plates close together give a large capacitance; small
plates far apart give a small one.

::: equation
Q = C V
:::

::: legend
$Q$: stored charge, in coulombs
$C$: capacitance, in farads
$V$: voltage across the plates, in volts
:::
:::
