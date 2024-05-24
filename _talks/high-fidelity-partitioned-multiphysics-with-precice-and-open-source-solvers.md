---
name: "High-fidelity partitioned multiphysics with preCICE and open-source solvers"
speakers:
  - "Benjamin Rodenberg"
  - "Benjamin Uekermann"
  - "Hans-Joachim Bungartz"
categories:
  - "Talks"
session: "09:15 - 10:45"
---

The open-source library preCICE allows connecting open-source solvers to solve multiphysics problems collaboratively. A minimally invasive partitioned coupling approach allows this without modifying the source code of the solvers. For fluid-structure interaction, for example, we couple the CFD toolbox OpenFOAM with the FEM library FEniCS. Behind a minimally invasive API, preCICE offers functionality for mesh mapping, efficient communication, quasi-Newton coupling acceleration, and time interpolation to simplify this process.

I present a short live demo of the preCICE ecosystem in my talk. It includes the C++ coupling library, language bindings, the adapter glue code between preCICE and the solvers, and a suite of tutorials. I also highlight the time interpolation feature I developed during my PhD. While following our partitioned coupling approach, this new feature allows the high-fidelity coupling of solvers with higher-order time-stepping and supports multirate time-stepping.
