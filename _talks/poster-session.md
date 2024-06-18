---
name: "Poster session"
speakers: ""
categories:
  - Social
session: "from 17:00"
---

{% include hidden_abstract_js.html %}

{%include poster_abstract.html
    id="scroggs"
    title="DefElement: an encyclopedia of finite element definitions"
    author="Matthew Scroggs"
    affiliation="University College London"
    website="https://defelement.com"
    github="mscroggs"
    abstract="<a href='https://defelement.com/'>DefElement</a> is an online encyclopedia that aims to include details of the definitions of all finite elment spaces. This poster will tell people about DefElement and how they con contribute."
%}

{%include poster_abstract.html
    id="ward"
    title="An execution abstraction for compact computational kernels on unstructured meshes"
    author="Connor Ward"
    affiliation="Imperial College London"
    github="connorjward"
    email="c.ward20@imperial.ac.uk"
    coauthors="David Ham (Imperial College London), Jack Betteridge (Imperial College London)"
    abstract="The execution of compact computational kernels is ubiquitous in continuum mechanics simulations. These \"local\" kernels, often hand-written, are executed repeatedly as part of an outer loop over (usually) the cells or facets of the mesh, with the relevant parts of the global data structures loaded into local temporaries as required.

Whilst initially appearing to be a simple task, this pack/unpack execution model is surprisingly complicated. Performance portability considerations often require intrusive changes (e.g. data layout transformations, different programming languages, manual vectorisation) that would require either rewriting the outer loop time and time again or sacrificing performance.

In this work we present pyop3, a new framework for handling mesh iteration problems. pyop3 uses code generation to produce the different loops automatically from a high-level representation. Core to its design is a novel data layout abstraction that bridges the gap between unstructured mesh data and traditional N-dimensional arrays. Work is currently under way to integrate pyop3 into the finite element package Firedrake, with the hope that it facilitates the development of new numerical methods and performance optimisations."
%}

{%include poster_abstract.html
    id="eardley-brunt"
    title="Developing computational liquid-metal MHD capabilities for fusion applications"
    author="Rupert Eardley-Brunt"
    affiliation="UKAEA (United Kingdom Atomic Energy Authority)"
    coauthors="Aleksander J Dubas (UKAEA), Andrew Davis (UKAEA)"
    abstract="Fusion power is being targeted as a major energy source for the future, promising clean, sustainable power, however many challenges remain in the design of magnetic confinement fusion devices as they scale from experimental tokamaks to power plants. A key part of tackling these challenges is developing the computational capability to simulate integrated components using multiphysics approaches. Building high fidelity simulations with multiple physics domains coupled together will enhance predictive modelling and in silico design, but incorporating highly scalable open-source solvers across many disciplines of physics into multiphysics packages remains a major practical challenge. A particular area of interest is liquid-metal magnetohydrodynamics (MHD), dominating the behaviour of conducting flows in liquid metal breeder designs due to the proximity to the strong magnetic fields of the tokamak. This work outlines ongoing investigations into suitable existing codes for liquid metal MHD, as well as the development of potential alternatives, with the ultimate goal of targeting efficient exascale computations and coupling to other physics such as electromagnetism in neighbouring domains, heat transfer, and tritium breeding and transport."
%}

{%include poster_abstract.html
    id="derlatka"
    title="Tackling parameterised PDEs with proper orthogonal decomposition and deep learning: benchmark in FEniCSx"
    author="Jan Jakub Derlatka"
    email="jjd61@cam.ac.uk"
    github="jjderlatka"
    affiliation="University of Cambridge"
    abstract="Solving parameterised PDEs with finite elements method (FEM) requires recalculation of the solution upon every change of parameters values. This poster explores the POD-ANN approach to that problem, initially proposed by J.S. Hesthaven and S. Ubbiali. In that method, in offline phase, solutions to a range of parameters are calculated using FEM. Proper Orthogonal Decomposition (POD) is applied to these solutions, to identify a reduced basis for the problem. Finally, an artificial neural network (ANN) is trained to map parameters to reduced basis coefficients. Then, in online phase, finding a solution to previously unseen values of parameters amounts to running the ANN, and reconstructing the solution from reduced basis, with a hope that it’s quicker than solving the full FEM problem.

The poster discusses the method through the \"lid-driven cavity problem\", used in the original paper, but implemented with parallelised offline phase, using a range of open-source libraries in development, including FEniCSx. Additionally, the poster addresses the challenges of geometric parameterization in a different way. Time permitting, a demonstration of the method's performance on a time-dependent version of the problem may also be included."
%}

{%include poster_abstract.html
    id="hope-collins"
    title="Parallel-in-time finite element models using ParaDiag"
    author="Josh Hope-Collins"
    affiliation="Imperial College London"
    email="joshua.hope-collins13@imperial.ac.uk"
    website="https://profiles.imperial.ac.uk/joshua.hope-collins13"
    github="JHopeCollins"
    coauthors="Colin Cotter (Imperial College London)"
    abstract="Spatial parallelism has been an effective strategy for PDE solvers for many decades. However, for time dependent problems the wallclock time is linear in the number of timesteps N once spatial parallelism saturates. Parallel-in-time algorithms overcome this by solving multiple timesteps simultaneously, allowing the number of processors to increase with N. ParaDiag solves the all-at-once system for multiple timesteps by preconditioning with a matrix that is block diagonalisable with the FFT. Solving the block diagonal matrix can be trivially parallelised across multiple processors.

We present asQ, a library for solving arbitrary finite element models using Paradiag written with Firedrake and PETSc. Firedrake enables users to specify their problem in the high level Unified Form Language (UFL) and automates kernel code generation. Given the UFL for a single timestep, asQ will construct the all-at-once system and ParaDiag preconditioners. PETSc then provides a wide range of linear and nonlinear methods for solving the system. We describe the library design and present scaling results up to 512 nodes of Archer2 for a set of atmospheric flow test cases." 
%}
