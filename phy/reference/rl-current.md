---
title: RL current rise
uses: [ohms-law, inductor-voltage]
---

::: equation
I(t) = \frac{V_s}{R}\left(1 - e^{-t/\tau}\right) \qquad \tau = \frac{L}{R}
:::

::: legend
$I$: current, in amperes
$V_s$: supply voltage, in volts
$R$: resistance, in ohms
$L$: inductance, in henries
$\tau$: time constant, in seconds
:::

The current in an inductor switched onto a supply rises toward $V_s/R$ along an exponential, with
time constant $\tau = L/R$.

::: derivation
Around the loop the supply equals the resistor drop plus the inductor's opposition:
$V_s = I R + L\,dI/dt$.
Rearrange: $L\dfrac{dI}{dt} = V_s - I R$, the rate of change proportional to the remaining gap to
$V_s/R$.
That integrates to an exponential approach. With $I(0) = 0$:
$I(t) = \dfrac{V_s}{R}\left(1 - e^{-t/(L/R)}\right)$, so $\tau = L/R$. ∎
:::