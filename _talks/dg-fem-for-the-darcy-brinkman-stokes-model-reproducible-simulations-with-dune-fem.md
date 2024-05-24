---
name: "DG-FEM for the Darcy-Brinkman-Stokes model: reproducible simulations with DUNE-FEM"
speakers:
  - "Benjamin Terschanski"
  - "Mohammad Ghanem"
  - "Julia Kowalski"
categories:
  - "Talk"
---

Computational scientists are frequently tasked with building application oriented simulation setups on top of ever-evolving modern numerical software. Contemporary open-source frameworks, such as FEniCS and DUNE-FEM [2,3], are powerful model building tools. With their inherent flexibility, they also pass the responsibility to develop sustainable application-specific research codes on to the user.

In this contribution, we present our DUNE-FEM-based solver framework for the Darcy-Brinkman-Stokes (DBS) model [3]. Originating from homogenization theory, this common model describes flows on domains where flow transitions from free incompressible flow to porous media flow and avoids explicit interface-tracking techniques. Our solver is based on stabilized mixed Discontinuous Galerkin Finite Elements (DG-FEM) and handles setups with spatially and temporally varying porosity as well as porosity jumps on the domain. We show convergence on test problems and discuss potential use-cases.

Based on the DBS model solver, we discuss our application-driven development efforts towards reproducible simulations built on open-source solver frameworks. To that end, we show our own Python-based simulation driver on top of the DUNE-FEM Python API, which automates the enrichment of simulation outputs with the respective setup used to obtain them. 

References: 

[1] Baratta et al. (2023), 10.5281/zenodo.10447666 

[2] Dedner et al. (2020), 10.5281/zenodo.3706994 

[3] Le Bars et al. (2006), 10.1017/S0022112005007998
