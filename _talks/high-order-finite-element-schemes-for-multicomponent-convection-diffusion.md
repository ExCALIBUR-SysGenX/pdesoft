---
name: "High-order finite element schemes for multicomponent convection-diffusion"
speakers:
  - "Aaron Baier-Reinio"
  - "Patrick E. Farrell"
categories:
  - "Talk"
---

In this talk we consider the Stokes–Onsager–Stefan–Maxwell (SOSM) equations, which model the flow of concentrated mixtures of distinct chemical species in a common thermodynamic phase. The equations account for both the diffusive interactions between chemical species and the bulk convection. Our aim is to develop computationally efficient high-order finite element schemes that discretize these nonlinear equations in two and three spatial dimensions. Because the SOSM equations relate many unknown variables (e.g. the bulk and species velocities, pressure, concentrations, chemical potentials, etc.), this is a difficult task. In particular, there are many choices of which variables should be explicitly solved for in the formulation, and it is not clear which discrete finite element function spaces should be employed. To tackle this challenge, we derive a novel weak formulation of the SOSM problem in which the species mass fluxes are treated as unknowns. We show that this new formulation naturally leads to a large class of high-order finite element discretizations that are straightforward to implement and have desirable linear-algebraic properties. From a theoretical standpoint, we are able to prove that when applied to a linearized version of the SOSM problem, the proposed finite element schemes are convergent. We also present some preliminary simulations on the mixing of hydrocarbons.