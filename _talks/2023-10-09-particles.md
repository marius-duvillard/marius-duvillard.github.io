---
title: "PARTICLES 2023 - Ensemble Kalman Filter Adapted to Particle Simulations"
collection: talks
type: "Talk"
permalink: /talks/2023-10-09-particles-2023-enkf-particle-simulations
venue: "PARTICLES 2023"
date: 2023-10-09
location: "Milan, Italy"
slidesurl: "/files/particles2023_duvillard.pdf
---

**Presentation of adaptations of the EnKF algorithm for particle-based simulation by intensity correction.**  

Data assimilation methods refer to a sequential estimation of the state of a system based on the incorporation of online observations. The complete way determines the state’s posterior distribution given the observations until now.
In the case of linear Gaussian models and observations, one can update the mean and covariance of the system’s state analytically using the Kalman Filter formula [^1].
However, in general, one must estimate the state’s distribution. A popular filter is the Ensemble Kalman Filter (EnKF), a Monte-Carlo version of the Kalman Filter suitable for non-linear and high-dimensional problems [^2]. The EnKF method uses a set of realizations (in our case, simulations) to estimate the empirical distribution of the system’s state. Then, it updates the members of the realizations’ set, applying corrections consisting of linear combinations of the members’ states.
This method has been extensively applied to problems discretized on fixed Eulerian grids (for instance, in Geociences [^3]). The EnKF filter requires adaptations for more specific Eulerian discretization methods, such as for problems using members having different mesh resolutions [^4] or moving mesh simulations [^5]. In this work, we adapt the EnKF method to particle-based simulations. Specifically, we focus on defining the members’ correction from states’ linear combinations when the members have different particle discretizations (number of particles, positions, and weights).
We propose and test different filters involving hybrid particle-mesh or purely Lagrangian approaches, with a criterion to adapt the particle discretization of the updated members. These developments are illustrated with 2D vortex simulations. The proposed schemes can be applied to other methods, such as the SPH or MPM.

REFERENCES

[^1]: R.E. Kalman. «A New Approach to Linear Filtering and Prediction Problems.» Journal of Basic Engineering 82, no 1 (1960): 35 45.
[^2]: G. Burgers, P.J. van Leeuwen, et G. Evensen. «Analysis Scheme in the Ensemble Kalman Filter.» Monthly Weather Review 126, no 6 (1998): 1719 24. 
[^3]: M. Bocquet. «Introduction to the Principles and Methods of Data Assimilation in the Geosciences,» (2014), 89.
[^4]: A. Siripatana, L. Giraldi, O. P. Le Maître, O. M. Knio, et I. Hoteit. «Combining Ensemble Kalman Filter and Multiresolution Analysis for Efficient Assimilation into Adaptive Mesh Models.» Computational Geosciences 23, no 6 (2019): 1259 76.
[^5]: J. Du, J. Zhu, F. Fang, C. C. Pain, et I. M. Navon. «Ensemble Data Assimilation Applied to an Adaptive Mesh Ocean Model.» International Journal for Numerical Methods in Fluids 82, no 12 (2016): 997 1009.

[More info](https://particles2023.cimne.com/event/contribution/de1204ac-dacd-11ed-9a1c-000c29ddfc0c).