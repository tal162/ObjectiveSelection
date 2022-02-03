This dataset contains the synthetic patient and treatment data for prostate cancer radiation therapy planning used in the article entitled "Objective Selection for Cancer Treatment: An Inverse Optimization Approach" by Ajayi, Lee, and Schaefer (2021). The data include the dose influence matrices (i.e., the $D$ matrices) and a treatment plan used as input data for the objective selection problem (i.e., $\hat{x}$). Each patient data was generated via the `IMRTP` module of [CERR](https://github.com/cerr/CERR/wiki/IMRT-optimization-interfacing-with-an-external-solver) (Computational Environment for Radiotherapy Research) and an auxiliary optimization problem to generate the D matrices.

## Data Description

This dataset contains the dose influence matrices for prostate cancer radiation therapy treatment planning as well as a treatment plan used as input for the objective selection problem.

* `D_CTV.mat`: Dose influence matrix for the clinical target volume

* `D_PTV.mat`: Dose influence matrix for the planning target volume

* `D_Blad.mat`: Dose influence matrix for the bladder

* `D_Rect.mat`: Dose influence matrix for the rectum

* `D_LFem.mat`: Dose influence matrix for the left femoral head 

* `D_RFem.mat`: Dose influence matrix for the right femoral head

* `D_Norm.mat`: Dose influence matrix for other normal tissues surrounding the planning target volume

* `w_ach.out`: synthetic treatment plan used as input for the objective selection problem

Each `D_*` matrix is a 2-dimensional array: each row represents a voxel in patient anatomy and each column represents a beamlet. Each entry of the matrix then represents the amount of radiation dose delivered by each beamlet to each voxel in Gy. 

Other parameters used for the treatment plan optimization problem can be found in Ajayi, Lee, and Shaefer (2021).

## Citing the Data

Suggested citation for data use: T. Ajayi, T. Lee, and A. J. Schaefer (2021) "Objective Selection for Cancer Treatment: An Inverse Optimization Approach." _Operations Research_.