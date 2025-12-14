# Fluid-Sim-ABM
Inspired by boids-style ideas like separation and alignment, this system extends them with **physical constraints and density control**.

Agents behave as solid bodies that cannot overlap, using hard collision forces, while also applying soft, local interaction rules within a sensor radius that resemble separation and alignment. Movement is further shaped by density regulation, steering agents toward a target local crowding level rather than simple attraction or repulsion.

The result is a **hybrid swarm model** that sits between boids-style behavioral steering and fluid or active-particle physics.

**Key characteristics**
-   Agent-based: each particle acts on local information
-   Emergent behavior: global patterns arise without scripting
-   Physically grounded: collisions are enforced, not merely avoided


**Future improvements**
-   Add per-agent state and parameters (size, strength, perception) to support heterogeneous agents
-   Extend cohesion to full center-of-mass steering rather than single-axis support
-   Introduce agent states or goals (fear, attraction, task-driven motion) to expand behaviors

---
Built off and also inspired from [SebLague](https://github.com/SebLague)'s [fluid simulator](https://github.com/SebLague/Fluid-Sim) and development videos: [Simulation](https://youtu.be/rSKMYc1CQHE?si=KNw_i1sN2_CWEmzA) and [Rendering](https://youtu.be/kOkfC5fLfgE?si=1hXtw9nIiHllA6gn).

# Fluid-Sim

Development videos: [Simulation](https://youtu.be/rSKMYc1CQHE?si=KNw_i1sN2_CWEmzA) and [Rendering](https://youtu.be/kOkfC5fLfgE?si=1hXtw9nIiHllA6gn).
</br>Project created in Unity 2022.3

![Fluid Simulation](https://raw.githubusercontent.com/SebLague/Images/master/Fluid%20vid%20thumb.jpg)
![Fluid Rendering](https://raw.githubusercontent.com/SebLague/Images/refs/heads/master/FluidRendering.jpg)

With thanks to the following papers:
* Simulation:
* https://matthias-research.github.io/pages/publications/sca03.pdf
* https://web.archive.org/web/20250106201614/http://www.ligum.umontreal.ca/Clavet-2005-PVFS/pvfs.pdf
* https://sph-tutorial.physics-simulation.org/pdf/SPH_Tutorial.pdf
* https://web.archive.org/web/20140725014123/https://docs.nvidia.com/cuda/samples/5_Simulations/particles/doc/particles.pdf
* Rendering:
* https://developer.download.nvidia.com/presentations/2010/gdc/Direct3D_Effects.pdf
* https://cg.informatik.uni-freiburg.de/publications/2012_CGI_sprayFoamBubbles.pdf
