---
permalink: /research/
title: "Research"
author_profile: true
redirect_from: 
  - /rs/
  - /research.html
---

In short, I am committed to developing fast and accurate computational theories and methods, which can be used to accurately describe the properties of nanoscale systems.

Velocity-Gauge Real-Time DFTB
======
I first derived and implemented a new velocity-gauge real-time, time-dependent density functional tight-binding (VG-RT-TDDFTB) method in the open-source [DFTB+ software package](https://dftbplus.org) for probing electronic excitations in large, condensed matter systems. Our VG-RT-TDDFTB approach enables real-time electron dynamics simulations of large, periodic, condensed matter systems containing thousands of atoms with a favorable computational scaling as a function of system size. Taken together, our VG-rtTDDFTB approach enables new electron dynamics simulations of complex systems that require large periodic supercells, such as crystal defects, complex surfaces, nanowires, and amorphous materials.

Orbital-Free DFT
======
The accuracy of OF-DFT simulations depends strongly on the quality of the non-interacting kinetic energy and the electron-ion (or electron-pseudocore) interaction energy employed in the simulations. In the past few years, we derived the advanced kinetic energy density functionals for OF-DFT calculations. Furthermore, I first proposed the nonlocal pseudopotential method in this field, which defies the belief that nonlocal pseudopotentials are not applicable to OF-DFT, leading to the creation for an alternate theoretical framework of OF-DFT that works superior to the traditional approach.
* Kinetic Energy Density Funtional (KEDF)
  * Xu-Wang-Ma (XWM) functional for periodic systems. See Ref.[XWM](https://doi.org/10.1103/PhysRevB.100.205132). 
  * LDAK-X functionals for isolated systems. See Ref.[LDAK-X](https://doi.org/10.1103/PhysRevB.101.045110).
* Nonlocal Pesudopotential Energy Density Functional (NLPPF). See Ref.[NLPPF](https://doi.org/10.1038/s41467-022-29002-3).

Kohn-Sham DFT
======
We presented a Kohn-Sham DFT based calculation package (ARES), utilizing real-space finite-difference method, advanced Chebyshev subspace filtering iteration solver, versatile non-periodic/periodic boundary conditions, and highly parallelizable features making the simulation of large-scale systems possible.
