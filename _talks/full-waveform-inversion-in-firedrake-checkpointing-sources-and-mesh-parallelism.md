---
name: "Full waveform inversion in Firedrake: checkpointing, sources and mesh parallelism"
speakers:
  - "Daiane Dolci"
  - "David A. Ham"
categories:
  - "Talk"
---

Full Waveform Inversion (FWI) is a technique for estimating subsurface properties in geophysics. It uses the full wavefield information recorded during seismic surveys to iteratively refine an Earth model until the simulated seismic response closely matches the observed data. This work presents an implementation of FWI within the Firedrake framework, leveraging parallel computing for faster and more efficient simulations. The core of our approach lies in the Ensemble Reduced functional, a Firedrake object that enables the simultaneous computation of the misfit (data difference) and its gradients for multiple seismic sources in parallel. This capability reduces computational time compared to single-source processing. Furthermore, the Ensemble Reduced functional allows mesh distribution across computing nodes. While source parallelisation offers faster simulations, it can also lead to increased memory demands due to the need to store wavefield data from multiple sources. To address this challenge, we employ checkpointing algorithms, which store only the state required to restart the forward calculation from a limited set of steps. This combined strategy enables us to perform FWI calculations on realistic, large-scale models while mitigating memory constraints.
