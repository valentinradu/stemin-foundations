---
title: Describing the wave
---

::: card
Knowing the voltage is a sine, we need a vocabulary to pin down *which* sine. Any sinusoid is
fixed by three numbers: how tall it is, how fast it repeats, and where it starts.
:::

::: card
The **peak** $V_p$ is the height from the centre line to the crest, the most the voltage ever
reaches in either direction. The full swing from trough to crest is the **peak-to-peak**,
$V_{pp} = 2 V_p$.
:::

::: card
The **period** $T$ is the time for one cycle; the **frequency** $f$ is how many cycles fit in a
second, in hertz. They are reciprocals.

$$ f = \frac{1}{T} $$

For 50 Hz mains, $T = 20$ ms, and the whole pattern repeats every 20 ms.
:::

::: card
A sine is the height of a point going around a circle, so its progress can be measured as an
angle. One cycle is $2\pi$ radians, and radians per second is the **angular frequency**.

$$ \omega = 2\pi f $$

For 50 Hz, $\omega \approx 314$ rad/s, large because the point whips around fifty times a second.
:::

::: card
Angular frequency converts elapsed seconds into swept angle, $\text{angle} = \omega t$, so the
wave as a function of time is

$$ v(t) = V_p \sin(\omega t) $$

That equation *is* the AC voltage.
:::

::: card
The last number, the **phase** $\varphi$, says where the wave sits when the clock starts:
$v(t) = V_p\sin(\omega t + \varphi)$. A single wave's phase is arbitrary. What is physical is the
phase difference between two waves of the same frequency: whichever reaches a point in the cycle
first **leads**, the other **lags**. A quarter-cycle is 90°.
:::

::: exercise q1
European mains runs at 50 Hz. What is its angular frequency $\omega$?

::: answer
About 314 rad/s. $\omega = 2\pi f = 2\pi \times 50 \approx 314$ rad/s.
:::
:::