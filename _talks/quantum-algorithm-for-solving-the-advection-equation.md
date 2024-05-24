---
name: "Quantum algorithm for solving the advection equation"
speakers:
  - "Peter Brearley"
  - "Sylvain Laizet"
categories:
  - "Talk"
---

Quantum computing promises a paradigm shift in our computational capability, and among the most promising applications is efficiently solving partial differential equations. Quantum computers gain their advantage by storing and processing information in a space that grows exponentially with the size of the computer, but require the development of specialised algorithms for any advantage. In this talk, a new quantum algorithm for simulating advection is presented. The required circuit depth grows polynomially with the number of grid points N as O(N^{1/3}k/ε) for a three-dimensional problem, where k and ε are the order of spatial discretisation and the allowable error, respectively. This offers a significant polynomial speedup over classical algorithms with an approximate complexity of O(N^{4/3}).The results present a promising route for performing computational fluid dynamics on a quantum computer.