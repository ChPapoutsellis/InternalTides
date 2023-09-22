# Internal Tides CMS

Calculation of Internal Tides (IT) using a Coupled-Mode System (CMS) obtained
by the body-forcing formulation of the hydrodynamic problem.

The function ITCMS calculates the IT generated by a Gaussian ridge.
It returns the energy conversion rate and visualises several flow fields.

Details on the mathematical formulation and the numerical scheme are given in the paper:

Papoutsellis, C., Mercier, M., & Grisouard, N. (2023). Internal tide generation from non-uniform barotropic body forcing. Journal of Fluid Mechanics, 964, A20. doi:10.1017/jfm.2023.358 (https://arxiv.org/abs/2107.00632)

Any comments and questions are welcome!


# Working Example
Running the [https://github.com/chpapoutsellis/InternalTidesCMS/blob/main/ITCMS.m](ITCMS.m) function in the Matlab Command Window (type ITCMS and press Enter) produces the IT corresponding to the $M_2$ tidal constituent with constant stratification $N=0.0015$ (1/s), Coriolis frequency $f = 0.0001$ (1/s). The amplitude of the horizontal barotropic current at infinity is $U_0 = 0.04$ (m/s). The depth at infinity is $3000$ m and the ridge has a criticality $0.8$ and relative height $0.5$. The calculated energy conversion rate is $1577.26$ (W/m) per unit ridge length. We give below typical plots (baroclinic stream function and horizontal velocity) and a video produced by the code:
![alt text](https://github.com/ChPapoutsellis/InternalTidesCMSv1.0/blob/main/OUTPUT/psi.png?raw=true)
![alt text](https://github.com/ChPapoutsellis/InternalTidesCMSv1.0/blob/main/OUTPUT/u.png?raw=true)
![alt text](https://github.com/ChPapoutsellis/InternalTidesCMSv1.0/blob/main/OUTPUT/VIDEO.gif?raw=true)

# Acknowledgements
For the colormaps we use the function cmocean.m (also provided here) written by Chad A. Greene of the Institute for Geophysics at the 
University of Texas at Austin (UTIG), June 2016, using colormaps created by Kristen
Thyng of Texas A&M University, Department of Oceanography.

Thyng, K.M., C.A. Greene, R.D. Hetland, H.M. Zimmerle, and S.F. DiMarco. 2016. True 
colors of oceanography: Guidelines for effective and accurate colormap selection. 
Oceanography 29(3):9-13, http://dx.doi.org/10.5670/oceanog.2016.66.

