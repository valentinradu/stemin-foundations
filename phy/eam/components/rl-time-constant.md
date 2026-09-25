---
title: The RL time constant
---

::: card
The inductor's time constant follows the same logic as the RC circuit, with current in the role
voltage played.[RL current](reference:rl-current)

$$ I(t) = \frac{V_s}{R}\left(1 - e^{-t/\tau}\right) \qquad \tau = \frac{L}{R} $$

```plot
x: { var: t, label: "$t$ in units of $\\tau$", from: 0, to: 5, ticks: 1, grid: true }
y: { label: "$I / I_\\text{final}$", from: 0, to: 1.1 }

inputs:
  - { name: tau, min: 0.5, max: 2, default: 1, step: 0.1, label: "the time constant" }

draw:
  - hline: { at: 0.632, dash: true, label: "63%" }
  - vline: { at: tau, dash: true }
  - curve: { is: 1 - exp(-t / tau), accent: true }
  - point: { at: [tau, 0.632], label: "one $\\tau$" }
```
:::

::: card
At switch-on the inductor opposes the full supply and current starts at zero. As it builds, the
rate of change slows, the opposing voltage drops, and current climbs toward its final value
$V_s/R$ along the same exponential. After $5\tau$, done.
:::

::: card
A larger $L$ resists change more strongly, giving a slower rise. A larger $R$ means a lower final
current and dissipates energy faster, giving a shorter time constant.
:::

::: exercise q1
An RL circuit has $L = 50$ mH and $R = 25$ Ω, switched onto a 10 V supply. What is the time
constant and the final current?

::: answer
$\tau = 2$ ms and $I = 0.4$ A. The time constant is $L/R$; the final current is $V_s/R$.
:::

::: solution
The time constant:

$$ \tau = \frac{L}{R} = \frac{0.05}{25} = 0.002\ \text{s} = 2\ \text{ms} $$

The final current, once the inductor is just a wire:

$$ I = \frac{V_s}{R} = \frac{10}{25} = 0.4\ \text{A} $$

reached in practice after $5\tau = 10$ ms. ∎
:::
:::

::: reference rl-current
# RL current rise

The current in an inductor switched onto a supply rises toward $V_s/R$ along an exponential, with
time constant $\tau = L/R$.

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

::: derivation
Around the loop the supply equals the resistor drop[Ohm's law](reference:ohms-law) plus the
inductor's opposition:[Inductor voltage](reference:inductor-voltage)
$V_s = I R + L\,dI/dt$.
Rearrange: $L\dfrac{dI}{dt} = V_s - I R$, the rate of change proportional to the remaining gap to
$V_s/R$.
That integrates to an exponential approach. With $I(0) = 0$:
$I(t) = \dfrac{V_s}{R}\left(1 - e^{-t/(L/R)}\right)$, so $\tau = L/R$. ∎
:::
:::
