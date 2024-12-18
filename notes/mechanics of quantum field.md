# Quantum Field

[TOC]



## Principles

### Wave-Particle Duality

Quantum objects (like electrons or photons) exhibit both wave-like and particle-like properties. They can behave as particles in some experiments and as waves in others.

### Measurement and Collapse

The Copenhagen Interpretation asserts that until a quantum system is measured, it exists in a superposition of all possible states. Upon measurement, the wave function "collapses" to a single state, which is observed. The act of observation is crucial in determining the outcome.

## Wave Function


玻恩规则
$$
\mathbb P = |\psi(x)|^2\\
\int|\psi(x)|^2 d^3 r= 1
$$


算符对易关系
$$
[\hat x, \hat y] = x y - yx = i \hbar
$$
测量中的期望值
$$
\langle\hat{A}\rangle=\int \psi^{*}(\mathbf{r}, t) \hat{A} \psi(\mathbf{r}, t) d^{3} r
$$

### Wave equation: Schrödinger equation

$$
i\hbar \frac{\partial}{\partial t} \psi(\mathbf{r}, t) = \hat{H} \psi(\mathbf{r}, t)
$$
The time-dependent Schrödinger equation, describes how the quantum state evolves over time for a given Hamiltonian. The wave function $\psi(\mathbf{r}, t)$ contains all the information about the system, and the Hamiltonian operator governs the dynamics of the system.

- $\psi(\mathbf{r}, t)$ is the wave function, which encodes the quantum state of a particle or system.
- $\hbar$ is the reduced Planck's constant
- $\hat{H}$ is the Hamiltonian operator, which represents the total energy (kinetic + potential) of the system.

#### Time-independent Schrödinger equation

$$
\hat{H} \psi(\mathbf{r}) = E \psi(\mathbf{r})
$$
$$
\nabla^{2} \psi-\frac{8 \pi^{2}}{h^{2}} V \psi \mp \frac{4 \pi i}{h} \frac{\partial \psi}{\partial t}=0
$$

$$
\nabla^2 \psi + \frac{8 \pi^2}{h^2} (E-V) \psi = 0
$$

### Uncertainty Principle

描述了两个共轭可观测量（如位置和动量，或能量和时间）之间的不确定性关系。一般形式的海森堡不确定性原理可以表示为：
$$
\Delta A \Delta B \geq \frac{1}{2} \left| \langle [\hat{A}, \hat{B}] \rangle \right|
$$

- $\Delta A$: The standard deviation (or uncertainty) of the observable $A$. 
- $\hat{A}$ 和 $\hat{B}$ 是对应的量子算符。
- $\langle [\hat{A}, \hat{B}] \rangle$ 是对易算符的期望值。

具体到位置和动量的情况，不确定性原理可以表示为：

$$
\Delta x \Delta p \geq \frac{\hbar}{2}
$$

### Dirac equation

狄拉克方程是一个关于四分量自旋量子的方程，可以写作：

$$
(i \gamma^\mu \partial_\mu - m) \psi = 0
$$

其中：
- $\psi$ 是狄拉克自旋量子，具有四个分量，表示粒子的波函数。
- $\gamma^\mu$ 是狄拉克矩阵，满足反对易关系 $\{ \gamma^\mu, \gamma^\nu \} = 2g^{\mu\nu}$，其中 $g^{\mu\nu}$ 是闵可夫斯基度规。
- $m$ 是粒子的质量。
- $\partial_\mu$ 是对时空坐标的偏导数。

狄拉克矩阵 $\gamma^\mu$ 是 4×4 矩阵，满足以下反对易关系：

$$
\{ \gamma^\mu, \gamma^\nu \} = \gamma^\mu \gamma^\nu + \gamma^\nu \gamma^\mu = 2g^{\mu\nu}I
$$

这些矩阵的一个常见表示是标准的狄拉克表示（Dirac-Pauli 表示）：

$$
\gamma^0 = \begin{pmatrix}
I & 0 \\
0 & -I
\end{pmatrix}, \quad
\gamma^i = \begin{pmatrix}
0 & \sigma^i \\
-\sigma^i & 0
\end{pmatrix}
$$
其中 $I$ 是 2×2 单位矩阵，$\sigma^i$ 是泡利矩阵。

## Hydrogen Atom

### Hamiltonian of the hydrogen atom

$$
H = -\frac{\hbar^2}{2m} \nabla^2 - \frac{e^2}{4 \pi \epsilon_0 r}
$$

- $-\frac{\hbar^2}{2m} \nabla^2$: **Kinetic Energy**. This term accounts for the kinetic energy of the particle due to its motion through space.
- $-\frac{e^2}{4 \pi \epsilon_0 r}$: **Potential Energy**. This term represents the Coulomb potential energy between two charged particles, such as the attraction between the negatively charged electron and the positively charged proton in a hydrogen atom. The negative sign indicates that this is an attractive force.

### Wave function solution for the hydrogen atom

$$
\begin{align*}
\psi_{n,l,m_l}(r, \theta, \phi) &= R_{n,l}(r) \cdot \Theta(\theta) \cdot \Phi(\phi)  \\
R_{n,l}(r) &= \sqrt{\frac{2}{a_0}} \cdot \frac{1}{\sqrt{n^2}} \left( \frac{r}{a_0} \right)^l e^{-\frac{r}{n a_0}} L_{n-l-1}^{2l+1} \left( \frac{2r}{n a_0} \right)  \tag{Radial}\\
\Theta(\theta) &= P_l^{m_l}(\cos \theta)  \tag{Angular}  \\
\Phi(\phi) &= \frac{1}{\sqrt{2\pi}} e^{i m_l \phi}  \tag{Azimuthal angle}
\end{align*}
$$

- $n$: principal quantum number (for energy levels). $n = 1, 2, 3, \dots$.
- $l$: angular momentum quantum number (determines the orbital shape).
- $m_l$: magnetic quantum number (determines the orientation of the orbital in space).
- $\psi_{n,l,m_l}(r, \theta, \phi)$: the wavefunction of the system, which depends on three quantum numbers.
- $R_{n,l}(r)$: the radial part of the wavefunction, which describes how the wavefunction depends on the radial distance $r$ from the nucleus.
- $\Theta(\theta)$: the angular part of the wavefunction. $P_l^{m_l}(\cos \theta)$ is the associated Legendre polynomial.
- $\Phi(\phi)$: the angular dependence on the azimuthal angle $\phi$, which is periodic with period $2\pi$. The factor $e^{i m_l \phi}$ reflects the azimuthal dependence of the wavefunction. The quantum number $m_l$ determines how the wavefunction rotates in the $xy$-plane. The factor $\frac{1}{\sqrt{2\pi}}$ is a normalization factor to ensure that the wavefunction is properly normalized over the angular coordinate $\phi$, such that $\int_0^{2\pi} e^{i m_l \phi} e^{-i m_l' \phi} d\phi = 2\pi \delta_{m_l,m_l'}$.

$$
E_n = - \frac{13.6 \, \text{eV}}{n^2}
$$



## Spin


### Fermions: Fermi-Dirac Distribution

$$
f(E) = \frac{1}{e^{(E - \mu) / k_B T} + 1}
$$
其中，$E$是能量，$\mu$是化学势，$k_B$是玻尔兹曼常数，$T$是温度。

### Boson: Bose-Einstein Distribution

$$
n(\epsilon) = \frac{1}{e^{(\epsilon - \mu) / k_B T} - 1}
$$
其中，$\epsilon$是单粒子能量，$\mu$是化学势。


**路径积分表述（Path Integral Formulation）**（费曼路径积分）：
$$
\langle x_f, t_f | x_i, t_i \rangle = \int \mathcal{D}[x(t)] e^{\frac{i}{\hbar} S[x(t)]}
$$
其中，$S[x(t)]$是作用量。

### Yang-Mills theory
