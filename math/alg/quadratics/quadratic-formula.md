---
title: The quadratic formula
---

::: card
A *quadratic equation* in one unknown has the form $a x^2 + b x + c = 0$, with $a \ne 0$.
:::

::: card
Every quadratic is solved by one formula.[the quadratic formula](reference:quadratic-formula)

$$ x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a} $$
:::

::: card
The sign of $b^2 - 4ac$ decides how many real roots there are: two, one, or none.[the discriminant](reference:discriminant)
:::

::: exercise q1
Solve $x^2 - 5x + 6 = 0$.

::: answer
$x = 2$ or $x = 3$.
:::

::: solution
$$ x = \frac{5 \pm \sqrt{25 - 24}}{2} = \frac{5 \pm 1}{2} $$

So $x = 3$ or $x = 2$. Check: $(x-2)(x-3) = x^2 - 5x + 6$. ∎
:::
:::

::: reference discriminant
# The discriminant

The discriminant of a quadratic $a x^2 + b x + c$ tells how many real roots it has: positive
gives two, zero gives one, negative gives none.

::: equation
\Delta = b^2 - 4ac
:::

::: legend
$\Delta$: the discriminant
$a$: coefficient of the square term
$b$: coefficient of the linear term
$c$: constant term
:::
:::

::: reference quadratic-formula
# The quadratic formula

For $a x^2 + b x + c = 0$ with $a \ne 0$, the solutions are

::: equation
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}.
:::

::: legend
$x$: the solutions (roots)
$a$: coefficient of the square term
$b$: coefficient of the linear term
$c$: constant term
:::

::: derivation
Divide by $a$ and complete the square:

$$ x^2 + \frac{b}{a}\,x = -\frac{c}{a}, \qquad \left(x + \frac{b}{2a}\right)^2 = \frac{b^2 - 4ac}{4a^2}. $$

Take the square root of both sides and isolate $x$ to get the formula. ∎

It rests on [The discriminant](reference:discriminant).
:::
:::
