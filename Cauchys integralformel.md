# Cauchy's Integral Formula

Cauchy's Integral Formula is a fundamental result in complex analysis that gives the value of a contour integral of a holomorphic (complex differentiable) function over a closed curve. It is especially useful for evaluating integrals and finding values of functions inside a contour.

## **Cauchy's Integral Formula (General Form)**

Let $f(z)$ be a function that is analytic (holomorphic) inside and on a simple closed contour $C$ that encloses a point $z_0$. Then for any point $z$ inside $C$, the value of $f(z)$ is given by the following integral:

$$
2 \pi i\cdot f(a) =\oint_C \frac{f(z)}{z - a} \, dz
$$

Where:
- $f(z)$ is the value of the function on the contour.
- $z$ is the variable of integration.
- $a$ is any point inside the contour $C$.
Og a er eneste singualritet innenfor $C$

Verdt å nevne er at på grunn av [Cauchys integralteorem](Notater/Matematikk%204/Cauchys%20integralteorem.md) vil singulariteter være de eneste elementene som har bidrag på linjeintegralet, og dermed er et linjeintegral over singulariteten det samme som å plusse sammen individuelle linjeintegral rundt hver av singulariteter

