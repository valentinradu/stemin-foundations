---
title: Why alternating current won
---

::: card
The grid runs on AC for one main reason: the **transformer**, which responds only to changing
current and so needs AC. It lets voltage be traded against current while the power is held fixed,
since $P = V I$.
:::

::: card
A fixed power can ship as a low voltage with a large current, or a high voltage with a small one.
The reason to pick high voltage is the loss in the transmission line itself.

$$ P_\text{loss} = I^2 R $$

The loss depends on the current squared, and on nothing about the voltage directly.
:::

::: card
Cut the current to a tenth, by stepping the voltage up tenfold, and the loss falls to a
hundredth. That squaring is the entire case for high-voltage transmission: step the voltage up
for the long haul, then back down for use. DC could not be transformed easily when the grid was
built, so AC won the wiring of the world.
:::

::: card
One intuition to retire: high voltage does not mean fast electrons. Current counts the charge
passing a point each second, not the speed of one electron, and a wire is so full that an
ordinary current creeps them along at under a millimetre a second. In AC they do not even
progress: they rock a tiny distance back and forth fifty times a second, while the energy rides
the field past them at near light speed.
:::

::: exercise q1
Transmission loss is $I^2 R$. You step the line voltage up tenfold, cutting the current to a
tenth for the same power. By what factor does the line loss fall?

::: answer
A hundredth. Loss goes as the current squared, so a tenth of the current means
$(1/10)^2 = 1/100$ of the loss.
:::
:::