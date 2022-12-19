# ATS-workflow
## Important materials you must read before proceeding
ATS Manuscript --> https://www.sciencedirect.com/science/article/pii/S1364815215301316

ATS surface-subsurface coupling manuscript--> https://www.sciencedirect.com/science/article/pii/S0309170820301536

ATS documentation --> https://amanzi.github.io/ats/input_spec/ATSNativeSpec_1_4.html

## ATS demos and  short course
Rerun the demos and short course to understand how it works
https://github.com/amanzi/ats-demos

https://github.com/amanzi/ats-short-course

## Pin Shuai has a similar workflow that is very informative and helpful (there may be more!!!)
https://pinshuai.github.io/ats-workflow/intro.html

It contains details on Model setup and execution (both for local PC and HPC)

## For Mos_Test 
This is a case of Richard’s flow (case of infiltration at the top, base flow at the bottom)

Basic Input paramers are:

Domain mesh only (1,1,20)
Cycle = 1 year
PK solved = Richards flow
Boundary conditions =  @ top – mass flux, 
outward mass flux=  -0.004
Initial condition –-> hydrostatic head = “-19” and density = 1000
Independent variable –porosity = 0.45, permeability = 4.5 e-12

* See results and demonstartion in attached powerpoint

## For TR00 -- Coupled Surface and Subsurface flow (Richards flow + overland flow)
This demo is a 3D domain with coarse mesh to demonstrate how water moves from surface to subsurface

Input parameters

Domain mesh and surface (40,50,20)
Cycle = 2 day (172,800s)
Boundary conditions @ surface = critical depth

Initial condition –surface domain– 101325 (atm pressure) Function_linear = 101325(atm pressure); [0,0,0,3]; [0,0,0, -9806.23]

surface – “initialise surface head from subsurface”

surface-mass_source =Function-tabular – {0,43200},{3e-02,0}

source-Molar_density = 55347.378, surface-manning_coefficient = 0.01986, surface-temperature = 274.65, base_porosity = 0.35, surface-Relative_permeability = 1, mass_density=997, viscosity – 0.00089, permeability = 1.052888e-12, van Genuchten; alpha = 0.00010224, n=2, residual saturation = 0.2, saturation smoothing interval= 0

* See results and demonstartion in attached powerpoint

## How to generate custom mesh


## For case of infiltration with growing mesh --  

