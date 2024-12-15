# Basic principles of mechanics

[TOC]

## The Principle of Least Action

### Action & Lagrangian

$$
S = \int L \mathrm{d} t
$$

The action is defined as the integral of the Lagrangian $L$ over time. It provides a unifying principle that describes the dynamics of a system in terms of its energy distribution.

The Lagrangian $L$ is a function that encapsulates the state and dynamics of a system.

### The Principle of Least Action

$$
\delta S = 0
$$



Nature chooses the path between two points in configuration spacetime that makes $S$ stationary.

### Euler-Lagrange equations

$$
\frac{d}{dt} \left( \frac{\partial \mathcal{L}}{\partial \dot{q}} \right) - \frac{\partial \mathcal{L}}{\partial q} = 0,
$$

where $q$ represents generalized coordinates of the system, and $\dot{q}$ is the time derivative (velocity).

## 相空间

相空间：由 s 个广义坐标和 s 个广义动量构成的 2s 维空间。
$$
(q, p)
$$

### Hamiltonian function

Hamiltonian function, Hamiltonian equations

哈密顿方法的好处是, 在特定限制下, 使 Lagrange 方程降阶，能找到 2s 个一阶微分方程, 方便计算. 
$$
H(p,q,t) = \sum_i p_i \dot q_i - L\\
\dot q_i = \frac{\partial H}{\partial p_i}\\
\dot p_i = \frac{\partial H}{\partial q_i}\\
$$

### Poisson bracket

$$
\{f, g\}=\sum_{k}\left(\frac{\partial f}{\partial p_{k}} \frac{\partial g}{\partial q_{k}}-\frac{\partial f}{\partial q_{k}} \frac{\partial g}{\partial p_{k}}\right)\\
\frac{\mathrm{d}f}{\mathrm{d}t} = \frac{\partial f}{\partial t} + \{H, f\}
$$

### 莫培督原理

假设拉格朗日量不显含时间，因而哈密顿量不显含时间，因此系统的能量守恒, 最小作用量原理有更简单的形式
$$
H(p, q) = E = const.
$$

### 刘维尔定理

在相空间内, 具有相体积不变性
$$
\int \mathrm{d} \Gamma = const.
$$


## Symmetry: Noether's theorem

### Symmetry & quantity: Noether's theorem

For every differentiable symmetry of the action of a physical system, there exists a corresponding conserved quantity.

- Time translation symmetry → Conservation of energy: If the Lagrangian does not explicitly depend on time $\partial \mathcal{L} / \partial t = 0$, energy is conserved.
- Spatial translation symmetry → Conservation of linear momentum: If the Lagrangian is invariant under shifts in position, linear momentum is conserved.
- Rotational symmetry → Conservation of angular momentum: If the Lagrangian is invariant under rotations, angular momentum is conserved.