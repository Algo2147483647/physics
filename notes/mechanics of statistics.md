# Statistical Mechanics

[TOC]

## Thermodynamic Quantities

### Entropy


$$
S = k \ln(\Omega)
$$

Entropy is a measure of the number of available microstates.

- $S$: entropy of the system.
- $k$: Boltzmann constant, $1.380649 \times 10^{-23} \, \text{J/K}$.
- $\Omega$: the number of microstates (distinct ways the system can be arranged) corresponding to a particular macrostate (state defined by macroscopic variables such as energy, volume, etc.).


### Temperature

$$
\frac{\mathrm{d}S}{\mathrm{d}U} = \frac{1}{T}
$$

If two systems are each in thermal equilibrium with a third, they are also in thermal equilibrium with each other.
$$
\mathrm{d}U = \mathrm{d}Q - \mathrm{d}W
$$

### First law

In a process without transfer of matter, the change in internal energy, $\Delta U$, of a thermodynamic system is equal to the energy gained as heat, $Q$, less the thermodynamic work, $W$, done by the system on its surroundings.
$$
\Delta U = Q-W
$$

### Third law

As the temperature of a system approaches absolute zero, all processes cease and the entropy of the system approaches a minimum value.

## Ensemble

### Microcanonical ensemble

- Isolated System: The system does not exchange energy, particles, or volume with the environment. 
- Fixed Energy (E): All microstates in the ensemble have the same energy. 
- Fixed Volume (V): The volume of the system is constant. 
- Fixed Number of Particles (N): The number of particles in the system remains constant. 
- All Microstates are Equally Probable: In the microcanonical ensemble, all possible configurations of the system that satisfy the constraints of energy, volume, and number of particles are considered equally probable.

#### Entropy

$$
S = k \ln(\Omega)
$$

Entropy is a measure of the number of available microstates.

- $S$: entropy of the system.
- $k$: Boltzmann constant, $1.380649 \times 10^{-23} \, \text{J/K}$.
- $\Omega$: the number of microstates (distinct ways the system can be arranged) corresponding to a particular macrostate (state defined by macroscopic variables such as energy, volume, etc.).


Heat does not spontaneously flow from a colder body to a hotter body.
$$
\mathrm{d}S \ge \frac{\mathrm{d}Q}{T}
$$

### Canonical ensemble

- System in Thermal Contact: The system can exchange energy with a large external reservoir (heat bath), so the energy of the system is not fixed.
- Fixed Temperature (T): The system is maintained at a constant temperature by exchanging energy with the reservoir.
- Fixed Volume (V): The volume of the system is constant.
- Fixed Number of Particles (N): The number of particles in the system is constant.
- Energy Fluctuations: The system can have fluctuating energy, but on average, it is determined by the temperature of the reservoir.

#### partition function

### Grand canonical ensemble

- **System in Contact with a Reservoir**: The system can exchange both energy and particles with a large reservoir or bath. This implies that the system's energy and particle number can fluctuate, but the temperature $T$ and chemical potential $\mu$ of the system are fixed.
- **Fixed Temperature (T)**: The system is maintained at a constant temperature by exchanging heat with the reservoir.
- **Fixed Chemical Potential ($\mu$)**: The chemical potential, which controls the exchange of particles between the system and the reservoir, is fixed.
- **Energy and Particle Number Fluctuate**: Unlike the microcanonical and canonical ensembles, both the energy and the number of particles of the system are allowed to fluctuate.
- **System Size**: The number of particles in the system is not fixed and can change, which is different from the canonical ensemble, where the number of particles is constant.



## Ideal Gas

$$
PV=nRT
$$

- $P$: pressure
- $V$: volume
- $T$: temperature
- $n$: the amount of substance
- $R$: the ideal gas constant.