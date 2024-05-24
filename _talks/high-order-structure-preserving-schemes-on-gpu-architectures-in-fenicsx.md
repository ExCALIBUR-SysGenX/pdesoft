---
name: "High-order, structure-preserving schemes on GPU architectures in FEniCSx"
speakers:
  - "Joseph P. Dean"
  - "Garth N. Wells"
categories:
  - "Talk"
session: "13:30 - 15:00"
---

Many established codes rely on traditional, low-order discretisations. These low-order methods have low arithmetic intensity, which is not well suited to current and future generations of high-performance computing architectures. Simulation of complex, whole-system problems will require accurate and stable methods with high arithmetic intensity, especially to exploit the coming generation of exascale computers.

We investigate the application of high-order, structure-preserving methods on GPU architectures. These discretisations are stable, arbitrarily high-order accurate, and have excellent conservation properties, but they present some challenges on GPU architectures due to the reliance on high-order H(div)- and H(curl)-conforming finite elements. High-order geometry is also required, which can result in both mathematical and computational difficulties. 

We make use of recent developments in the FEniCSx finite element library that allow state-of-the-art hardware, including modern GPUs, to be experimented with. We focus on the magnetohydrodynamics equations, using liquid metal breeder blankets (used in some nuclear fusion reactor designs) as an example application.
