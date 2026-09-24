---
title: A linear system in matrix form
---

::: card
Two linear equations in $x$ and $y$ collapse into one matrix equation $A \vec{x} = \vec{b}$:

$$ \begin{pmatrix} a & b \\ c & d \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} p \\ q \end{pmatrix} $$
:::

::: card
When the determinant is nonzero, Cramer's rule solves the system directly.[Cramer's rule](reference:cramer)
:::

::: exercise q2
Solve the system for $x$ and $y$:

$$ \begin{cases} 2x + y = 5 \\ x - 3y = -1 \end{cases} $$

::: answer
$(x, y) = (2, 1)$. The lines are not parallel, so they meet at one point.
:::

::: solution
Multiply the second equation by 2 and subtract it from the first:

$$ 7y = 7 \implies y = 1, \quad 2x + 1 = 5 \implies x = 2 $$

The determinant $2 \cdot (-3) - 1 \cdot 1 = -7$ is nonzero, so the solution is unique. ∎
:::
:::

::: exercise q3
Solve the same system three ways and confirm they agree.

::: answer
$(x, y) = (2, 1)$, by substitution, elimination, and Cramer's rule alike.
:::

::: solution
**Substitution.** The first equation gives $y = 5 - 2x$, so

$$ x - 3(5 - 2x) = -1 \implies 7x = 14 $$
$$ x = 2, \quad y = 1. $$

**Cramer's rule.** With $\det A = -7$,

$$ x = \frac{\begin{vmatrix} 5 & 1 \\ -1 & -3 \end{vmatrix}}{-7} = 2 $$
$$ y = \frac{\begin{vmatrix} 2 & 5 \\ 1 & -1 \end{vmatrix}}{-7} = 1 $$

All three agree. ∎
:::
:::

::: reference cramer
# Cramer's rule

For a system $A \vec{x} = \vec{b}$ with $\det A \ne 0$, the solution is

::: equation
x = \frac{\begin{vmatrix} p & b \\ q & d \end{vmatrix}}{\det A}, \quad
   y = \frac{\begin{vmatrix} a & p \\ c & q \end{vmatrix}}{\det A}.
:::

::: legend
$x$: first unknown
$y$: second unknown
$p$: the first equation's constant
$q$: the second equation's constant
$\det A$: determinant of the coefficient matrix
:::

::: derivation
Write $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$. Replacing each column of $A$ by
$\vec{b}$ in turn and dividing by $\det A$ gives the two quotients. The denominator is
$\det A$, nonzero by assumption, so each is well defined. ∎
:::
:::
