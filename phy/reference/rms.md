---
title: RMS of a sine
uses: [power]
---

::: equation
V_\text{rms} = \frac{V_p}{\sqrt{2}} \approx 0.707\,V_p
:::

::: legend
$V_\text{rms}$: root-mean-square voltage, in volts
$V_p$: peak voltage, in volts
:::

The root-mean-square value of an alternating quantity is the equivalent DC value: the steady
level that delivers the same average power. For a sine it is the peak over root two.

::: derivation
Average power in a resistor is the instantaneous $v^2/R$ averaged over a cycle:
$P_\text{avg} = \overline{v^2}/R$.
Define $V_\text{rms} = \sqrt{\overline{v^2}}$, so $P_\text{avg} = V_\text{rms}^2/R$, the DC form.
For $v = V_p\sin(\omega t)$, the average of $\sin^2$ over a cycle is $1/2$, so
$\overline{v^2} = V_p^2/2$.
Therefore $V_\text{rms} = V_p/\sqrt{2}$. ∎
:::