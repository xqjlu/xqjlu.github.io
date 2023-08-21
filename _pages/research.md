---
permalink: /research/
title: "Research"
author_profile: true
redirect_from: 
  - /rs/
  - /research.html
---

In short, I am committed to developing fast and accurate computational theories and methods, which can be used to accurately describe the properties of nanoscale systems. Currently, I am working on three directions:

**1. Velocity-Gauge Real-Time DFTB**

Real-time time-dependent density functional theory is a reliable framework to study the light-matter interaction. For large systems or some long time-scale electron dynamic simulations, it is necessary to adopt an approximate theoretical formalism at low computational cost. Therefore, the length-gauge real-time time-dependent density functional tight-binding (LG-RT-TDDFTB) method has previously been proposed that exhibits strong computational efficiency. However, the translation symmetry of the Hamiltonian is broken by the external electric field in the length-gauge implementation. Thus it is typically used for finite systems rather than the condensed matter systems modeled under widely used  periodic boundary conditions, such as crystal defects, complex surfaces, heterostructures, and amorphous systems, which require large supercells. To address the limitation, in this work, we first derived and implemented the velocity-gauge real-time time-dependent density functional tight-binding (VG-RT-TDDFTB) formalism for large, and long-time scale electron dynamics simulations under periodic boundary conditions. Numerical results show that the high computational efficiency and parallelizability provide remarkable advantages for electron dynamic simulations for large and complex systems.


**2. Orbital-Free DFT**

Orbital-free density functional theory (OF-DFT) is an electronic structure method with a low computational cost that scales linearly with the number of simulated atoms, making it suitable for large-scale material simulations (1-100 million atoms, 1-100 nm). However, the accuracy of OF-DFT simulations depends strongly on the quality of the non-interacting kinetic energy and the electron-ion (or electron-pseudocore) interaction energy employed in the simulations. In the past few years, we derived the advanced kinetic energy density functionals for OF-DFT calculations. Furthermore, we first proposed the nonlocal pseudopotential method in this field, which defies the belief that nonlocal pseudopotentials are not applicable to OF-DFT, leading to the creation for an alternate theoretical framework of OF-DFT that works superior to the traditional approach.
* Kinetic Energy Density Funtional (KEDF)
  * Xu-Wang-Ma (XWM) functional for periodic systems. See Ref.[XWM](https://doi.org/10.1103/PhysRevB.100.205132). 
  * LDAK-X functionals for isolated systems. See Ref.[LDAK-X](https://doi.org/10.1103/PhysRevB.101.045110).
* Nonlocal Pesudopotential Energy Density Functional (NLPPF). See Ref.[NLPPF](https://doi.org/10.1038/s41467-022-29002-3).

**3. Kohn-Sham DFT**

We presented a Kohn-Sham DFT based calculation package (ARES), utilizing real-space finite-difference method, advanced Chebyshev subspace filtering iteration solver, versatile non-periodic/periodic boundary conditions, and highly parallelizable features making the simulation of large-scale systems possible.
* ARES Development. See Ref.[ARES](https://doi.org/10.1088/1361-648X/ab2a63)
  * Massively parallel is on going
* Real-Space Pesudopotential Core-Level Binding Energies Calculation Method (CEBE). See Ref.[CEBE](https://doi.org/10.1021/acs.jctc.2c00474).
  * Traditional all-electron method
    * (o) High accuracy
    * (-) An additional algorithm is required to protect the core hole in the final-state calculations, which unexpectedly causes variational collapse.
    * (-) When the system contains multiple identical elements, it is difficult to select specific atom and core state.
    * (-) The expensive computation cost for large-scale systems
  * Real-space pseudopotential method
    * (o) High accuracy
    * (o) No need to introduce additional algorithms for final-state calculaton, good numerical stability
    * (o) Using non-self-consistent hybrid functional to refine the total energy at a low computational cost
    * (o) Core-hole atom and state can be specially and easily selected
    * (o) non-periodic boundary condtions for charged final-state calculation
    * (o) High computational efficiency for large-scale systems

