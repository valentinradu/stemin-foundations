---
title: Phasors, freezing the spin
---

::: card
Working with sines as $\sin(\omega t + \varphi)$ means dragging trig through every calculation.
Phasors make it algebra. In a single circuit every voltage and current oscillates at the same
frequency, the one the source sets, so the frequency tells you nothing about how they differ.
:::

::: card
Only two things distinguish one sinusoid from another: its size and its phase. Drop the frequency
and keep just those two as an arrow, a **phasor**: its length is the size (peak or RMS), its
angle is the phase.
:::

::: card
This is the rotating point from the generator, frozen. Every sinusoid is a point going around a
circle at $\omega$; since they all turn together at the same rate, you lose nothing by stopping
the rotation and looking at the snapshot. A quarter-cycle lead in time becomes an arrow 90°
around from another.
:::

::: card
The payoff: adding or comparing sinusoids becomes adding or comparing arrows, plain vectors, with
no trig. Two voltages in a loop add tip-to-tail; a current lagging its voltage by 90° is an arrow
a quarter-turn behind. This is the tool that makes reactance and impedance tractable.
:::

::: exercise q1
A phasor diagram drops the frequency. What must the sinusoids share for that to be valid, and
what two things does each phasor keep?

::: answer
They must share the same frequency. Each phasor keeps the two things that still differ: its
length (the size) and its angle (the phase).
:::
:::