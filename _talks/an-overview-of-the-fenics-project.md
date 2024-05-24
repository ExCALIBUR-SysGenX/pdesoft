---
name: "An overview of the FEniCS project"
speakers:
  - "Jørgen Schartum Dokken"
categories:
  - "Talk"
---

The FEniCS project, with its foundation in 2003 has gone through many major transformations in the last two decades. Some key changes in the first decade of development was the introduction of code generation through the FEniCS form compiler, the Python interface, MPI support, and the unified form language.

In its second decade, the code-based matured with many additional extensions including multi-mesh, mixed dimensional finite element support and goal oriented mesh refinement. However, the introduction of all these features made code maintenance more laborious.

There were also several core design choices, which no longer were justified, due to the development of C++, Python as languages and the improvements in hardware.

A rewrite of the whole FEniCS project started in 2017, called DOLFINx, with a bottom-up redesign of the core structures and user interface. In this talk, I will give an overview of the user interface, as well as highlighting new functionality.