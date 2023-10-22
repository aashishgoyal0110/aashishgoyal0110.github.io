---
layout: archive
title: " "
permalink: /more_projects/
author_profile: true
---

<p style="text-align:left; color:DimGray; font-size:30px; font-weight:bold;"> 
ACADEMIC PROJECTS 
</p>

This section continues the work shown on the <a href="https://aashishgoyal0110.github.io/" target="_blank">Home</a> page.

<p style="text-align:left; color:DimGray; font-size:25px; font-weight:bold;">
- Point cloud generation
</p>

Hydrodynamic force calculations on complex structures or non-spherical rigid bodies are an important part of the computational modeling of particle-laden flows. A numerical surface integration of the discretized surface provides the total force experienced by the rigid bodies due to the fluid. Following are a few images showing the generated point cloud.

Cube | Tetrahedron | Octahedron | Dodecahedron | Icosahedron | Cylinder | Sphere
:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|
![](../files/cube.png) | ![](../files/tetra.png) | ![](../files/octa.png) | ![](../files/dodeca.png) | ![](../files/icosa.png) | ![](../files/cylinder.png) | ![](../files/sphere.png)

<p style="text-align:left; color:DimGray; font-size:25px; font-weight:bold;">
- Hydrodynamic force on a randomly distributed Platonic polyhedrons
</p>

Here we increase the computational complexity by performing PR-DNS on randomly generated Platonic polyhedrons. We aim to study the impact of particle shape on the hydrodynamic forces. Stay tuned for more details.

Tetrahedron | Cube | Octahedron | Dodecahedron | Icosahedron
:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|
![](../files/ManyTetra.png) | ![](../files/ManyCubes.png) | ![](../files/ManyOcta.png) | ![](../files/ManyDodeca.png) | ![](../files/ManyIcosa.png)

<hr>

<p style="text-align:left; color:DimGray; font-size:30px; font-weight:bold;"> 
INDUSTRIAL PROJECTS
</p>

<p style="text-align:justify; font-size=22px;"> 
The data below are examples of my previous work as a Project Engineer at <a href="https://tridiagonal.com/" target="_blank">Tridiagonal Solutions</a>. I provided technical consulting to the partners in the food, pharmaceutical, and oil industries in order to optimize their process operations. The consultation involved the creation of smart and creative computational models to compensate for the high computing costs and enormous equipment size. I was successful in completing many projects in a short period of time, and my contributions were favorably recognized by industry partners.
</p>

<p style="text-align:left; color:DimGray; font-size:25px; font-weight:bold;">
- Liquid coating on particles 
</p>

<p style="text-align:justify; font-size=22px;"> 
The physical properties of particles change as they are coated with liquid. I wrote an interface in the open-source Discrete Element Method platform <a href="https://www.cfdem.com/liggghtsr-open-source-discrete-element-method-particle-simulation-code" target="_blank">LIGGGHTS</a> to:
</p>

* Detect the particle being coated under the spray using a ray-tracing approach.
* Change the particle properties during the simulation to reflect the actual scenario.

<p style="text-align:justify; font-size=22px;"> 
The following animation shows the particle rotating in a drum (not shown due to a confidentiality agreement), and the color shows the count when a particle comes under the spray.
</p>

![](../files/coating.gif)

<p style="text-align:justify; font-size=22px;"> 
I further added more details to the model to capture the liquid transfer when two particles with different liquid contents come into contact. The animation below shows an example of coating under spray in conjunction with the liquid transfer model. The color represent the amount of liquid carried by each rigid particle.
</p>

![](../files/coating2.gif)

<p style="text-align:left; color:DimGray; font-size:25px; font-weight:bold;">
- Sand transport in turbulent flow
</p>

<p style="text-align:justify; font-size=22px;"> 
Sand transport in pipes is very common in the oil industry. In this project, I developed a model to mimic the sand behavior of stable suspension or deposition in fluid flow. The sand particles are modeled using the open-source DEM framework <a href="https://www.cfdem.com/liggghtsr-open-source-discrete-element-method-particle-simulation-code" target="_blank">LIGGGHTS</a>, and the hydrodynamic forces from the turbulence are captured using a combination of <a href="https://www.openfoam.com/" target="_blank">OpenFOAM</a> and a stochastic model. This model was successful in predicting the minimum flow rate required to keep the sand particles suspended. The animation below shows the energy provided by the flow is not sufficient to keep the sand suspended, and hence the suspension height decreases.
</p>

![](../files/suspension.gif)

<p style="text-align:left; color:DimGray; font-size:25px; font-weight:bold;">
- Equipment design for optimum particle mixing
</p>

<p style="text-align:justify; font-size=22px;"> 
Another example where I provided an optimized impeller design for the efficient mixing of particles to the industry partners. The best design of the impeller include the optimization of the particle residence time in the mixer. The system shown below is designed using Ansys SpaceClaim and simulated in <a href="https://www.cfdem.com/liggghtsr-open-source-discrete-element-method-particle-simulation-code" target="_blank">LIGGGHTS</a>.
</p>

![](../files/tumbling.gif)