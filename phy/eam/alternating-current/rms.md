---
title: The honest average, RMS
---

::: card
What single number do you put on an AC voltage? Not the peak, touched for only an instant, and
not the plain average, which is zero: over a full cycle the positive and negative halves cancel
exactly. Yet AC clearly does work, so we need a number that captures it.
:::

::: card
The number that matters gets the power right. A resistor dissipates $P = v^2/R$ at every instant,
and what we care about is its average over a cycle.

$$ P_\text{avg} = \frac{\overline{v^2}}{R} $$
:::

::: card
One rule of order: square first, then average.[RMS](reference:rms) Squaring at each instant makes
the negative half of the cycle count instead of cancelling. Take the square root of the averaged
square to return to volts, and you have the **root mean square**: root of the mean of the square.
:::

::: card
This is the equivalent DC voltage: the steady voltage that would deliver the same average power
to a resistor. For a sine the average of $\sin^2$ is $1/2$, so the result is clean.

$$ V_\text{rms} = \frac{V_p}{\sqrt{2}} \approx 0.707\,V_p $$
:::

::: card
The 230 V at a European outlet is this RMS value; its peak is $230\sqrt{2} \approx 325$ V. With
RMS values every DC power formula returns unchanged: $P = V_\text{rms} I_\text{rms} = I_\text{rms}^2 R$.
When an AC voltage or current is quoted without saying "peak," it is RMS.
:::

::: exercise q1
A European outlet is quoted as 230 V. What is the peak voltage of the sine?

::: answer
About 325 V. The quoted value is RMS, so the peak is $V_p = V_\text{rms}\sqrt{2} = 230\sqrt{2} \approx 325$ V.
:::
:::

::: reference rms
# RMS of a sine

The root-mean-square value of an alternating quantity is the equivalent DC value: the steady
level that delivers the same average power. For a sine it is the peak over root two.

::: equation
V_\text{rms} = \frac{V_p}{\sqrt{2}} \approx 0.707\,V_p
:::

::: legend
$V_\text{rms}$: root-mean-square voltage, in volts
$V_p$: peak voltage, in volts
:::

::: derivation
Average power in a resistor is the instantaneous $v^2/R$ averaged over a cycle:
$P_\text{avg} = \overline{v^2}/R$.
Define $V_\text{rms} = \sqrt{\overline{v^2}}$, so $P_\text{avg} = V_\text{rms}^2/R$, the DC form.[Electrical power](reference:power)
For $v = V_p\sin(\omega t)$, the average of $\sin^2$ over a cycle is $1/2$, so
$\overline{v^2} = V_p^2/2$.
Therefore $V_\text{rms} = V_p/\sqrt{2}$. ∎
:::
:::
