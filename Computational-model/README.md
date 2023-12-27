# Model description

This numerical model simulates the Taylor-Couette flow using Large-Eddy Simulations. This solves the filtered continuity and Navier-Stokes equations which resolve the turbulent motion down to a point (defined by a top-hat filter $\Delta = V^{1/3}$ based on the cell volume, $V$).    This repository includes OpenFOAM (v4) case file here for the validation test case:

Dong, S. Direct numerical simulation of turbulent Taylor–Couette flow. _Journal of Fluid Mechanics._ 2007;587:373-393. [doi:10.1017/S0022112007007367](https://doi.org/10.1017/S0022112007007367)
