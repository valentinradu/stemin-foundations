---
title: Cramer's rule
---

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

For a system $A \vec{x} = \vec{b}$ with $\det A \ne 0$, the solution is

::: derivation
Write $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$. Replacing each column of $A$ by
$\vec{b}$ in turn and dividing by $\det A$ gives the two quotients. The denominator is
$\det A$, nonzero by assumption, so each is well defined. ∎
:::