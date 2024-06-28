# Data Description

The excel spreadsheets provided here include steady-state and dynamic datasets for developing the RBF and GRABNN models for the 
isothermal continuous stirred tank reactor (CSTR) system using noisy measurement / experimental data.

## Dynamic CSTR Data

This spreadsheet contains dynamic time-series (total duration of around 1600 time steps) input-output datasets for 
the CSTR system. The model inputs are represented by the inlet feed space velocity (F/V), and the concentration of 
all four reaction species in the feed stream (CAf, CBf, CCf, CDf), whereas, the model outputs are denoted by the 
outlet concentration of all reaction species in the product stream, i.e., CA, CB, CC, CD.

The .xlsx file contains 2 tabs in total. The second tab contains a schematic of the CSTR system under consideration. 
The first tab contains dynamic noisy data for the model input and output variables which constitute the training and 
validation datasets for the proposed data-driven models.

## Steady-State CSTR Data

This spreadsheet contains 400 steady-state input-output datasets for the CSTR system. The model inputs are represented 
by the inlet feed space velocity (F/V), and the concentration of all four reaction species in the feed stream (CAf, CBf, 
CCf, CDf), whereas, the model outputs are denoted by the outlet concentration of all reaction species in the product 
stream, i.e., CA, CB, CC, CD.

The .xlsx file contains 3 tabs in total. The last tab contains a schematic of the CSTR system under consideration. 
The first two tabs contain steady-state data for the truth case (i.e., output estimates obtained by simulating a 
first-principles model) and for the case where data are corrupted with uncertainties, respectively. The steady-state 
CSTR data are only implemented during the development of Mass-Constrained RBF (i.e., McRBF) models in this work. The 
models are trained and validated with respect to the noisy steady-state data. However, the true data are only used to 
compare model performance and accuracy in capturing system truth due to imposition of mass balance constraints, even 
when trained against noisy measurements.

## Color Code

The input and output variables have been color-coded in both excel spreadsheets attached for clarity --
  * The columns representing the variation in model inputs shown in 'light orange'
  * The columns representing the variation in corresponding model outputs shown in 'light green'


