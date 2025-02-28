# Hybrid Gaussian RAdial Basis Neural Networks (GRAB-NN): Development, Training, and Application to Process Modeling

Python (Jupyter) Notebooks for developing model architectures and novel training algorithms for standalone RBF networks and hybrid GRAB-NN structures for modeling nonlinear dynamic noisy chemical processes

Author: Angan Mukherjee (amukherjee43@wisc.edu)

Last Page Update: Feb 26, 2025

# Announcement

We are very welcome to your contribution. Please feel free to reach out to us with your feedback and suggestions on how to improve the current models.

# Publication

This public repository contains Python (Jupyter) notebooks for developing different architectures and corresponding training algorithms for standalone constrained and unconstrained RBF as well as hybrid GRAB-NN structures for nonlinear 
chemical systems operating under uncertainties. The corresponding publication for this work is currently under review:

**Mukherjee, A.**, Gupta, D. & Bhattacharyya, D, "*Mass-Constrained Hybrid Gaussian Radial Basis Neural Networks: Development, Training, and Applications to Modeling Nonlinear Dynamic Noisy Chemical Processes*", 
Computers & Chemical Engineering, 109080, 2025. DOI: https://doi.org/10.1016/j.compchemeng.2025.109080

These codes will be updated in subsequent versions to enhance robustness of the proposed algorithms and user friendliness.

# Brief Description

## Sample Data

Test case steady-state and dynamic data have been provided in Excel spreadsheets with respect to the operation of a continuous stirred tank reactor (CSTR)
system. Note that the codes uploaded in this repository are generic and can be applied to create data-driven models for any steady-state and dynamic
system (data). The rows of the input and output data matrices refer to the observation indices and time steps for steady-state and dynamic modeling respectively,
while the corresponding columns signify the different input / output variables.

## Pre-Requisites for Python / PYOMO Codes

The equality constrained optimization problems in several training approaches proposed in this work for development of parsimonious models have been solved using the 
Python-based open-source optimization modeling language, Pyomo v6.7.1 through the IDAES framework.
Note that using the IDAES framework is not mandatory for running the codes uploaded in this repository. One may simply use the interior point optimization solver (IPOPT) in
PYOMO to solve the constrained optimization problems proposed in this work. 

More details about Pyomo can be found at: https://github.com/Pyomo/pyomo

More details about IDAES can be found at: https://github.com/IDAES/idaes-pse

One may follow the following installation instructions for downloading Python / Pyomo / IDAES:
  * Install Anaconda: https://www.anaconda.com/download
  * Run 'Anaconda Prompt'
  * Create a new environment by: conda create -n my-new-env
  * Activate the new environment by: conda activate my-new-env
  * Install IDAES by: pip install idaes-pse
  * Get IDAES extensions by: idaes get-extensions
  * If a user wants to dodge using IDAES framework, the easiest way to install a version of Ipopt is: conda install -c conda-forge ipopt. More information can be found in
    PYOMO documentation (available online at: https://pyomo.readthedocs.io/en/stable/contributed_packages/parmest/index.html).  

However, for latest updates on IDAES and installation commands, please look up the IDAES GitHub page (https://github.com/IDAES/idaes-pse). 

Other libraries may be installed before running the Python notebooks, as necessary.

In addition, to access the training / simulation codes for development of Artificial Neural Network (ANN) models which exactly conserve linear / nonlinear mass conservation 
constraints in chemical process systems, please refer to the following link: https://github.com/mukherjeeangan26/Steady_Dynamic_MCNN.

Additional details about the MCNN model architectures and training / simulation algorithms have been discussed in the following publication:

**Mukherjee, A.** & Bhattacharyya, D. "*On the Development of Steady-State and Dynamic Mass-Constrained Neural Networks Using Noisy Transient Data*", 
Comput. Chem. Eng. 187, 108722 (2024). Avaiable online at: https://doi.org/10.1016/j.compchemeng.2024.108722

