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
Input
Domain mesh only (1,1,20)
Cycle = 1 year
PK solved = Richards flow
Boundary conditions =  @ top – mass flux, outward mass flux–  -0.004
Initial condition – hydrostatic head = “-19” and density of 1000
Independent variable –porosity = 0.45, permeability = 4.5 e-12

##
