# Maxwell's Equations

| **Equation**                                       | **Formula**                                                                 |
|----------------------------------------------------|-----------------------------------------------------------------------------|
| **1. Gauss's Law for Electricity**                 | $$ \nabla \cdot \mathbf{E} = \frac{\rho}{\epsilon_0} $$                    |
| **2. Gauss's Law for Magnetism**                   | $$ \nabla \cdot \mathbf{B} = 0 $$                                           |
| **3. Faraday's Law of Induction**                  | $$ \nabla \times \mathbf{E} = -\frac{\partial \mathbf{B}}{\partial t} $$    |
| **4. Ampère's Law with Maxwell's Correction**      | $$ \nabla \times \mathbf{B} = \mu_0 \mathbf{J} + \mu_0 \epsilon_0 \frac{\partial \mathbf{E}}{\partial t} $$ |

| **Symbol**   | **Description**            |
| ------------ | -------------------------- |
| $\mathbf{E}$ | Electric field             |
| $\mathbf{B}$ | Magnetic field             |
| $\rho$       | Electric charge density    |
| $\epsilon_0$ | Permittivity of free space |
| $\mu_0$      | Permeability of free space |
| $\mathbf{J}$ | Current density            |
| $t$          | Time                       |
# Maxwell's Equations (4-4-MAXWELLS LOVER)

## Introduction to Maxwell's Equations
- Historical context of Maxwell's work (1860s).
- Heaviside's reformulation into four differential equations.

## Mathematical Preliminaries
- Notation for time derivatives: \( \frac{d}{dt}, \frac{\partial}{\partial t} \).
- Role of the gradient operator \( \nabla \) in spatial coordinates.

## Integral Forms of Maxwell's Equations
- Derived using vector calculus theorems:
  - **Divergence theorem:**  
    $$
    \int_V (\nabla \cdot \mathbf{F}) dV = \oint_S \mathbf{F} \cdot d\mathbf{S}
    $$
  - **Stokes' theorem:**  
    $$
    \oint_C \mathbf{F} \cdot d\mathbf{l} = \int_S (\nabla \times \mathbf{F}) \cdot d\mathbf{S}
    $$
- Links between differential and integral forms.

## Simplified Scenarios
### Static Fields in a Vacuum
$\dot{E}=\dot{B}=0$
#### Empty space
$J=\rho=0$

### Electrostatics
- The electric field is conservative:  
  $$
  \nabla \times \mathbf{E} = 0
  $$
- Exists a scalar potential \( \phi \) such that:  
  $$
  \mathbf{E} = -\nabla \phi
  $$
- Satisfies Poisson’s equation:  
  $$
  \nabla^2 \phi = -\frac{\rho}{\epsilon_0}
  $$

### Magnetostatics
- No magnetic monopoles:  
  $$
  \nabla \cdot \mathbf{B} = 0
  $$
- Magnetic field has a vector potential \( \mathbf{A} \) such that:  
  $$
  \mathbf{B} = \nabla \times \mathbf{A}
  $$
- The components of \( \mathbf{A} \) satisfy Poisson’s equation:  
  $$
  \nabla^2 \mathbf{A} = -\mu_0 \mathbf{J}
  $$
Dette stemmer når vi velger at $div(A) =0$. 

