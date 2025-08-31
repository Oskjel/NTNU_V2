Si du har et området avgrenset av $\begin{matrix}1\leq x^{2}-y^{2}\leq 2, & 3\leq xy \leq 4\end{matrix}$

og skal beregne

$$
  \iint_{\Omega }x^{4}-y^{4}\, dA   
$$

Kan et man transformere om dette området ved å sette

$$
\begin{cases}
u = xy \\
v = x^{2}-y^{2}
\end{cases}
$$
deretter må man regne ut [[jacobimatrisen]]

I dette tilfellet blir det veldig vanskelig å regne ut uttrykk $x(u,v) \quad \text{and} \quad y(u , v)$ så derfor sjekker vi heller om kanselleringsmetoden funker bedre.

$$
J = {\frac{1}{\frac{ \partial (x, y) }{ \partial (u,v) } } } = \frac{1}{2(x^{2}+y^{2})}
$$

ved innsetning får vi da

$$
\int_{3}^{4}\int_{1}^{2} \frac{(x^{2}-y^{2})(x^{2}+y^{2})}{2(x^{2}+y^{2})}dudv = \int_{3}^{4}\int_{1}^{2} \frac{1}{2}u \,du \,dv
$$




