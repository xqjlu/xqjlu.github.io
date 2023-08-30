---
permalink: /research/
title: "Research"
author_profile: true
redirect_from: 
  - /rs/
  - /research.html
---

In short, I am committed to developing fast and accurate computational theories and methods, which can be used to accurately describe the properties of mesoscale systems. Currently, I am working on three directions:

**1. Velocity-Gauge Real-Time DFTB**

We first derived and implemented a new velocity-gauge real-time, time-dependent density functional tight-binding (VG-RT-TDDFTB) method in the open-source DFTB+ software package for probing electronic excitations in large, condensed matter systems. Our VG-RT-TDDFTB approach enables real-time electron dynamics simulations of large, periodic, condensed matter systems containing thousands of atoms with a favorable computational scaling as a function of system size. Taken together, our VG-RT-TDDFTB approach enables new electron dynamics simulations of complex systems that require large periodic supercells, such as crystal defects, complex surfaces, nanowires, and amorphous materials.
* Theoretical Development. See Ref.[Q. Xu et al., JCTC (2023)](https://doi.org/10.48550/arXiv.2308.09782)  
JCTC Cover<br/><img src='/images/dftb.png' width="300" height="300" >

**2. Orbital-Free DFT**

Orbital-free density functional theory (OF-DFT) is an electronic structure method with a low computational cost that scales linearly with the number of simulated atoms, making it suitable for large-scale material simulations (1-100 million atoms, 1-100 nm). However, the accuracy of OF-DFT simulations depends strongly on the quality of the non-interacting kinetic energy and the electron-ion (or electron-pseudocore) interaction energy employed in the simulations. In the past few years, we derived the advanced kinetic energy density functionals for OF-DFT calculations. Furthermore, we first proposed the nonlocal pseudopotential method in this field, which defies the belief that nonlocal pseudopotentials are not applicable to OF-DFT, leading to the creation for an alternate theoretical framework of OF-DFT that works superior to the traditional approach.
* Kinetic Energy Density Funtional (KEDF)
  * Xu-Wang-Ma (XWM) functional for periodic systems. See Ref.[Q. Xu et al., PRB (2019)](https://doi.org/10.1103/PhysRevB.100.205132). 
  * LDAK-X functionals for isolated systems. See Ref.[Q. Xu et al., PRB (2020)](https://doi.org/10.1103/PhysRevB.101.045110).
* Nonlocal Pesudopotential Energy Density Functional (NLPPF). See Ref.[Q. Xu et al., NC (2022)](https://doi.org/10.1038/s41467-022-29002-3).

**3. Kohn-Sham DFT**

We presented a Kohn-Sham DFT based calculation package (ARES), utilizing real-space finite-difference method, advanced Chebyshev subspace filtering iteration solver, versatile non-periodic/periodic boundary conditions, and highly parallelizable features making the simulation of large-scale systems possible.
* ARES Development. See Ref.[Q. Xu et al., JPCM (2019)](https://doi.org/10.1088/1361-648X/ab2a63)
  * Massively parallel is on going
* Real-Space Pesudopotential Core-Level Binding Energies Calculation Method (CEBE). See Ref.[Q. Xu et al., JCTC](https://doi.org/10.1021/acs.jctc.2c00474).
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

