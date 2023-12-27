# Model description

This numerical model simulates Taylor-Couette flow using Large-Eddy Simulations. This solves the filtered continuity and Navier-Stokes equations which resolve the turbulent motion down to a point (defined by a top-hat filter $\Delta = V^{1/3}$ based on the cell volume, $V$). A wall adapting local eddy-viscosity (WALE) approach is implemented for the sub-grid-scale eddy-viscosity. 

This repository includes the complete OpenFOAM (v4) case file here for a validation test case we performed in our previously published work:

Stafford, J., et al. Real-time Monitoring and Hydrodynamic Scaling of Shear Exfoliated Graphene. _2D Materials._ 2021;8:025029 [doi:10.1088/2053-1583/abdf2f](https://doi.org/10.1088/2053-1583/abdf2f).



Dong, S. Direct numerical simulation of turbulent Taylor–Couette flow. _Journal of Fluid Mechanics._ 2007;587:373-393. [doi:10.1017/S0022112007007367](https://doi.org/10.1017/S0022112007007367)
