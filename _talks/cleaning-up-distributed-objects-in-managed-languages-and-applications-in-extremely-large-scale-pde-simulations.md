---
name: "Cleaning up distributed objects in managed languages and applications in extremely large scale PDE simulations"
speakers:
  - "Jack Betteridge"
categories:
  - "Talk"
---

Memory managed languages such as Python and Julia are being used increasingly often on high performance computers (HPC) to drive extremely large, pre-exascale simulations of PDEs.

Advantages of working in a managed language include the flexibility to easily change discretisations and solvers for better hardware utilisation, as well as being more productive for scientists and engineers.

However, one drawback is that the memory management of such a language can create havoc when attempting to clean up distributed objects.

When running simulation code in a managed language in parallel, it is possible for Python's garbage collector to cause a deadlock when attempting to clean up distributed data structures that require collective destruction.

Turning off Python's garbage collection is a poor workaround at best and a catastrophic memory leak at worst.

We outline an algorithm for the safe parallel destruction of distributed objects that can be used in any managed language and fixes deadlocks when running in parallel.

Furthermore, we discuss the impact for very large scale PDE simulations that are written using Firedrake -- a Python based code generation framework for solving PDEs.