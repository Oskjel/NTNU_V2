Greens teorem: Arbeid og curl

$$
 \iint \frac{ \partial f_{2} }{ \partial x_{1}} - \frac{ \partial f_{1} }{ \partial x_2 } = \oint_{\partial\Gamma}^{}  \,f^TT dx 
$$


$$
curl(f) = \frac{ \partial f_{2} }{ \partial x_{1} } - \frac{ \partial f_{1} }{ \partial x_{2} }  
$$

Her ser man at summen av $curl(f)$ over området $\Gamma$ er det samme som [[Arbeid]] over randen $\partial \Gamma$.


Dersom $f$ er gradientfeltet til funksjon $\phi$, vil $div(f)=0$

Dette kan bevises ved,

$$
div(f)=\frac{ \partial f_{1} }{ \partial x_{1} } + \frac{ \partial f_{2} }{ \partial x_{2} }=0
$$
$$\implies \frac{ \partial^2 \phi }{ \partial^2 x_{1} } +\frac{ \partial^2 \phi }{ \partial^2 x_{2} } = 0 $$
Dette er [[laplaceoperator]], og når denne er null har vi at $\phi$ er en harmonisk funksjon.


I likhet har man Greens teorem for divergens og fluks der:

$$
\int \int \frac{ \partial f_{1} }{ \partial x_{1} } + \frac{ \partial f_{2} }{ \partial x_{2} }   = \oint f^TNds

$$
$$
div(f) = \frac{ \partial f_{1} }{ \partial x_{1} } + \frac{ \partial f_{2} }{ \partial x_{2} }  
$$

Her ser man at summen av $div(f)$ over området $\Gamma$ er det samme som [[Fluks]] over randen $\partial \Gamma$.


Dersom en et vektorfelt $g(x)$ er konservativt vil $curl(g)=0$. 
Dette kan bevises ved definisjonen av et konservativt vektorfelt altså,

$$
curl(g) =  \frac{ \partial g_{2} }{ \partial x_{1} } - \frac{ \partial g_{1} }{ \partial x_{2} }  = \frac{ \partial^2\phi }{ \partial x_{1} \partial x_{2}}- \frac{ \partial^2\phi }{ \partial x_{2} \partial x_{1}} =0
$$
