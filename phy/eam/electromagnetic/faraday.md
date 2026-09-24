---
title: Faraday's law
---

::: card
Flux is the amount of field passing through a surface: field strength times area times the
cosine of the angle between the field and the surface normal. Straight through gives maximum
flux; parallel to the surface gives zero.
:::

::: card
Faraday's law: a changing magnetic flux through a loop induces a voltage around that
loop.[Faraday's law](reference:faraday) Not the field itself, the rate of change. A steady field,
however strong, does nothing; start changing it and a voltage appears.

$$ V = -\frac{d\Phi_B}{dt} $$
:::

::: card
The minus sign is Lenz's law: the induced voltage always opposes the change that caused it.
Increase the flux and the induced current fights the increase. This is the inductor's defining
behaviour; the coil is Faraday's law made physical.
:::

::: card
It is also how transformers work: alternating current in one coil makes a changing magnetic
field, that field threads through the second coil, and the changing flux induces a voltage there.
No electrical connection between the two coils is needed.
:::

::: exercise q1
Faraday's law says a changing magnetic flux induces a voltage. What happens if the flux through a
coil is large but constant?

::: answer
No voltage is induced. The law depends on the rate of change of flux, not the flux itself. A
steady field, however strong, induces nothing.
:::
:::

::: reference faraday
# Faraday's law of induction

A changing magnetic flux through a loop induces a voltage around it, equal to the rate of change
of flux. The minus sign is Lenz's law: the induced voltage opposes the change that caused it.

A steady flux induces nothing; only its rate of change drives a voltage.

::: equation
V = -\frac{d\Phi_B}{dt}
:::

::: legend
$V$: induced voltage, in volts
$\Phi_B$: magnetic flux, in webers
$\frac{d\Phi_B}{dt}$: rate of change of flux
:::
:::
