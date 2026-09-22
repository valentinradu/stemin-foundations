---
title: Solving a linear equation
---

::: card
A *linear equation* in one unknown has the form $a x + b = 0$. Solve it by isolating the
unknown, undoing each operation in turn.
:::

::: card
$$ 2x + 4 = 10 \implies 2x = 6 \implies x = 3 $$
:::

::: card
The graph of $y = a x + b$ is a straight line. The slope $a$ tilts it; it meets the vertical axis
at $b$.[the intercept](reference:intercept) Drag the sliders and watch the line move.

```plot
x: { var: x, label: "$x$", from: 0, to: 8, ticks: 2, grid: true }
y: { label: "$y$", from: 0, to: 8 }

inputs:
  - { name: a, min: 0, max: 2, default: 0.5, step: 0.1, label: slope a }
  - { name: b, min: 0, max: 6, default: 1, step: 0.5, label: intercept b }

draw:
  - point: { at: [0, b], label: "the intercept" }
  - curve: { is: a * x + b, accent: true }
```
:::

::: exercise q1
Solve $3x - 6 = 9$ for $x$.

::: answer
$x = 5$. Add 6 to both sides, then divide by 3.
:::

::: solution
$$ 3x - 6 = 9 \implies 3x = 15 \implies x = 5 $$

Check: $3(5) - 6 = 9$. ∎
:::
:::