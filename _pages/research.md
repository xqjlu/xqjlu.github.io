---
permalink: /research/
title: "Research"
excerpt: "Efficient electronic-structure methods for mesoscale and large-scale condensed-matter simulations."
author_profile: true
redirect_from:
  - /rs/
  - /research.html
---

I develop fast and accurate theoretical and computational methods for mesoscale condensed-matter systems. My work spans real-time electron dynamics, orbital-free and Kohn–Sham density functional theory, and theoretical models of emergent material properties.

## 1. Velocity-Gauge Real-Time DFTB

<figure class="align-right" style="max-width: 240px; margin-top: 0;">
  <img src="/images/dftb.jpg" alt="Journal of Chemical Theory and Computation cover featuring the VG-rtTDDFTB method">
  <figcaption>VG-rtTDDFTB featured on the JCTC cover.</figcaption>
</figure>

We derived and implemented a velocity-gauge real-time time-dependent density functional tight-binding (VG-rtTDDFTB) method in the open-source DFTB+ package. The method enables real-time electron-dynamics simulations of large periodic systems containing thousands of atoms, including defects, surfaces, nanowires, and amorphous materials.

* Theoretical development: [Q. Xu et al., JCTC (2023)](https://doi.org/10.1021/acs.jctc.3c00689)
* Ehrenfest dynamics: [Q. Xu et al., JACS (2024)](https://doi.org/10.1021/jacs.4c12952)

## 2. Orbital-Free DFT

Orbital-free density functional theory (OFDFT) scales linearly with the number of atoms and is therefore well suited to large material simulations spanning nanometers to hundreds of nanometers. Our work improves the accuracy and scope of OFDFT through advanced kinetic-energy, pseudopotential-energy, and finite-temperature functionals. An overview is available in our [recent review](https://doi.org/10.1002/wcms.1724).

* **Kinetic-energy density functionals (KEDFs)**
  * XWM functional for periodic systems: [Q. Xu et al., PRB (2019)](https://doi.org/10.1103/PhysRevB.100.205132)
  * LDAK-X functionals for isolated systems: [Q. Xu et al., PRB (2020)](https://doi.org/10.1103/PhysRevB.101.045110)
* **Nonlocal pseudopotential energy density functionals (NLPPFs)**
  * Metals: [Q. Xu et al., Nature Communications (2022)](https://doi.org/10.1038/s41467-022-29002-3)
  * Semiconductors: [C. Ma et al., PRB (2024)](https://doi.org/10.1103/PhysRevB.109.075144)
* **Free-energy density functionals**
  * XWM-FEDF for warm dense matter: [C. Ma et al., PRB (2024)](https://doi.org/10.1103/PhysRevB.110.085113)

## 3. Kohn–Sham DFT

We developed ARES, a real-space Kohn–Sham DFT package based on finite differences, Chebyshev-filtered subspace iteration, flexible periodic and non-periodic boundary conditions, and highly parallel algorithms for large-scale systems.

* ARES development: [Q. Xu et al., JPCM (2019)](https://doi.org/10.1088/1361-648X/ab2a63)
* Real-space pseudopotential method for core-level binding energies: [Q. Xu et al., JCTC (2022)](https://doi.org/10.1021/acs.jctc.2c00474)

## 4. Theoretical Models

I also develop and apply theoretical models to understand emergent condensed-matter phenomena, including the microscopic mechanisms of superconductivity in molecular hydrides.

* Molecular-hydride superconductivity: [P. Liu et al., Science Advances (2025)](https://doi.org/10.1126/sciadv.adt9411)
