![](Pasted%20image%2020250218142433.png)## **Why Are All Three Components Necessary?**

1. $V_{a}$(Voltage Source):** Provides the power to drive the motor.
2. $R_{a}$​ (Resistance):** Models **realistic losses** in the winding.
3. $L_{a}$ (Inductance):** Models the effect of **current lag and transient response**.

****
**Relevant formulas**

$$
\begin{matrix}
\omega =n\cdot \frac{\pi}{30} \\
P=T\omega  \\
P_{el}=T_{dev}\omega _{dev}=E_{a}I_{a} \hspace{1 cm} \text{where $E_{a}$ is the armature voltage}\\
E_{a} = k\phi \omega_{m}\\

T_{dev} = k \phi I_{a}\\
T_{dev} - T_{load} = J \frac{d\omega }{dt}
\end{matrix}

$$


## Difference in Shunt Excited and Separately Excited DC machine
***
- How you control the magnetic field used for creating rotation in the motor

**Shunt excited:**
The potensiometer with resistance and inductor, where the magnitude of the potensiometer decides the strength of the magnetic field.

**Separately Excited:**
Circiuts for motor and magnetic field are separat, and 
