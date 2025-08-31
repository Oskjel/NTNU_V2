



# Curl in Cylindrical and Spherical Coordinates

## Curl in Cylindrical Coordinates (\(r, \theta, z\))

The vector field in cylindrical coordinates is given as:

$$\mathbf{F} = F_r \hat{e}_r + F_\theta \hat{e}_\theta + F_z \hat{e}_z$$

$$\nabla \times \mathbf{F} =
\begin{vmatrix}
\hat{e}_r & \hat{e}_\theta & \hat{e}_z \\
\frac{\partial}{\partial r} & \frac{1}{r} \frac{\partial}{\partial \theta} & \frac{\partial}{\partial z} \\
F_r & F_\theta & F_z
\end{vmatrix}
\
$$

Expanding the determinant, we get:
$$

\nabla \times \mathbf{F} =
\left( \frac{1}{r} \frac{\partial F_z}{\partial \theta} - \frac{\partial F_\theta}{\partial z} \right) \hat{e}_r
+ \left( \frac{\partial F_r}{\partial z} - \frac{\partial F_z}{\partial r} \right) \hat{e}_\theta
+ \frac{1}{r} \left( \frac{\partial}{\partial r} (r F_\theta) - \frac{\partial F_r}{\partial \theta} \right) \hat{e}_z

$$


---

## Curl in Spherical Coordinates (\(r, $\theta$, $\phi$\))

The vector field in spherical coordinates is:

$$
\mathbf{F} = F_r \hat{e}_r + F_\theta \hat{e}_\theta + F_\phi \hat{e}_\phi
$$

The curl in spherical coordinates is:

$$
\nabla \times \mathbf{F} =
\frac{1}{r \sin\theta}
\begin{vmatrix}
\hat{e}_r & r\hat{e}_\theta & r \sin\theta \hat{e}_\phi \\
\frac{\partial}{\partial r} & \frac{\partial}{\partial \theta} & \frac{\partial}{\partial \phi} \\
F_r & r F_\theta & r \sin\theta F_\phi
\end{vmatrix}
$$

Expanding the determinant, we get:

$$
\nabla \times \mathbf{F} =
\frac{1}{r \sin\theta}
\begin{bmatrix}
\frac{\partial}{\partial \theta} (F_\phi \sin\theta) - \frac{\partial F_\theta}{\partial \phi} \\
\frac{1}{\sin\theta} \frac{\partial F_r}{\partial \phi} - \frac{\partial}{\partial r} (r F_\phi) \\
\frac{1}{r} \frac{\partial}{\partial \theta} (r F_\theta) - \frac{1}{r} \frac{\partial F_r}{\partial \theta}
\end{bmatrix}
$$


