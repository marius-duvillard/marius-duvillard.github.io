---
title: "Data Assimilation by Alignment for Lagrangian Simulation"
collection: publications
category: draft
permalink: /publication/2024-01-01-ensemble-data-assimilation
date: 2024-01-01
venue: "Draft"
citation: "Marius Duvillard, Loïc Giraldi, Olivier Le Maître. (2024). &quot;Data Assimilation by Alignment for Lagrangian Simulation.&quot; Draft."
paperurl: '/files/align-part-enkf.pdf'
---

This study presents a novel approach for integrating data assimilation techniques into particle-based simulations using the Ensemble Kalman Filter. If data assimilation methods have been applied to Eulerian simulations for a long, they have never been properly used in the context of a Lagrangian solution discretization. Two specific methodologies are introduced to complete the analysis. The first one is based on the use of an intermediary Eulerian transformation combining a projection and a remeshing process. The second is a purely Lagrangian scheme that is applicable when remeshing is not adapted. These methods are evaluated using a one-dimensional advection-diffusion model with periodic boundaries. Subsequently, assimilation schemes are applied to a non-linear two-dimensional incompressible flow problem, solved via the Vortex-In-Cell method. In the one-dimensional scenario, the performance of these filters is benchmarked against a grid-based assimilation filter. In the two-dimensional case, the study demonstrates the feasibility of applying these methods in more intricate scenarios.

![](/images/three_vortex.gif)
*Three vortex simulation*