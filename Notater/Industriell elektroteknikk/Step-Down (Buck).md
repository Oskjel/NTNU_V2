![[Pasted image 20250324133228.png]]

**Under $t_\text{on}:$**

$$
v_{l, t_{on}} = V_{D}-V_{o}

$$
$$
\implies i_{L, t_{on}} = \frac{1}{L}\int_{0}^{t} V_{D}-V_{0} \, d\tau =(V_{D}-V_{o})t
$$
**Under $t_\text{off}:$**
$$
v_{l, t_{off}} = -V_{o}

$$
$$
\implies i_{L, t_{off}} = \frac{1}{L}\int_{t_{on}}^{t} -V_{0} \, d\tau =(-V_{o})(t-t_{on})
$$
***
##### Over a period $T = t_{on} + t_{off}$
![[Pasted image 20250324135050.png]]
The integral over the voltage over a period $T$ is $0$ since the waveform is a periodic wave

$$
\implies \int_{0}^{t_{on}} V_{D}-V_{0} \, d\tau + \int_{t_{on}}^{T} -V_{0} \,d\tau = 0
$$
$$
\implies (V_{D}-V_{o})t_{on} + (-V_{0})t_{off} = 0
$$
Del på $T$ og bruk at $\frac{t_{on}}{T}=D$
$$
V_{D}D
=V_{o}
$$
