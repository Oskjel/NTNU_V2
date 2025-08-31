

## Stokes' Theorem

Stokes' theorem relates the surface integral of the curl of a vector field to a line integral over its boundary:
$$
\oint_{\partial S} \mathbf{F} \cdot d\mathbf{r} = \iint_S (\nabla \times \mathbf{F}) \cdot d\mathbf{S}
$$


where:

- is an oriented surface with boundary ,
    
- is the surface element normal to ,
    
- is a continuously differentiable vector field.




---

## Oppgave 12
La $\Omega \in \mathbb{R}^3$ være begrenset av paraboloidene:

$$
x_3 = x_1^2 + (x_2 + 1)^2, \quad x_3 = 10 - x_1^2 - (x_2 - 1)^2.
$$

La \( \Gamma \) betegne skjæringskurven mellom dem, og la:

$$
f(x) = (x_1 + x_2, x_2 - x_1, x_1^2 + x_2^2)^T.
$$

Regn ut:

$$
\oint_{\Gamma} f \cdot ds
$$

der $\Gamma$ er orientert mot klokken sett ovenfra.

> [!tip]
Finn $curl(f)$ og bruke, og deretter sette kurvene like hverandre for da blir differansen $x_{1}^2+x_{2}^{2}=4$ så $\hat{n}=\begin{pmatrix}0 \\ 0 \\ 1\end{pmatrix}$
 


$$
\iint_{\Sigma}(\nabla \times f)\cdot d\mathbf{S} = A_{sirkel}\cdot(-2)
$$

## Beregning av flater integral med Stokes' teorem

For å beregne flater integralet $$\iint_{\Sigma} (\nabla \times \mathbf{f}) \cdot d\mathbf{S}$$ over delen av ellipsoideskallet gitt ved $$ x_1^2 + x_2^2 + 8(x_3 - 1)^2 = 9, \space \space x_{3}\geq{0} $$


Vektorfeltet er gitt ved:

$$
\mathbf{f}(x) = (x_1 x_3 - 5 x_2 \cos x_3, 5 x_1 e^{x_3}, 6 x_1 x_2 e^{x_1^2 + x_2^2 + x_3^2})
$$

$$
\iint_{\Sigma} (\nabla \times \mathbf{f}) \cdot d\mathbf{S} = \oint_{\partial \Sigma} \mathbf{f} \cdot d\mathbf{r}
$$
> [!tip]
> Trikset er å sette $x_{3}=0$ siden man kan velge hvilken som helst rand langs $\Sigma$. Da bler vektorfeltet mye penere og kan beregne arbeidet rundt pen sirkel.


