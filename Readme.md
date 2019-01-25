# SMU - MATLAB Package for Structural Model Updating

This package provides example MATLAB code and data for finite element model updating of structures. The code offers selection of different updating formulations and optimization algorithms. 

## Introduction

Field dynamic testing on an as-built structure usually provides modal properties that are different from these generated by a finite element (FE) model. To update the FE model parameters, optimization problems can be formulated to minimize the difference between experimental and simulated modal properties. Various FE model parameters can be selected as optimization variables for model updating, such as the elastic moduli of structural members, as well as stiffness values of support springs.

This software package for FE model updating offers two modal property difference formulations, one using MAC values and the other using direct differences between eigenvectors. For each updating formulation, analytical Jacobian derivative of the objective function is implemented. To find the optimal solution of the formulated optimization problem, the package supports two optimization algorithms implemented in MATLAB lsqnonlin optimization toolbox, namely the Levenberg-Marquardt and the trust-region-reflective algorithms. Randomly generated starting values of the optimization variables can be adopted to increase the chance of finding global minimum of the optimization problem. Finally, the MATLAB code contains two structural examples to evaluate the model updating formulations and optimization algorithms. 


## Contents

 “\_Shared”
The folder contains shared MATLAB routines for finite element model updating. This folder should be added into MATLAB path prior to running the example model updating code of the two example structures.

“\ConcreteBuildingFrame”
The folder contains example code and data for the updating of a concrete building frame model.

“\SteelPedestrianBridge”
The folder contains example code and data for the updating of a steel pedestrian bridge model.

## Companion Monograph
X. Dong and Y. Wang (2018). ["Formulation and optimization algorithm comparison for the FE model updating of large-scale structures."](http://wang.ce.gatech.edu/sites/default/files/docs/Formulation%20and%20Optimization%20Algorithm%20Comparison%20for%20the%20FE%20Model%20Updating%20of%20Large-Scale%20Structures.pdf)

## Citing SMU
Y. Wang, X. Dong, D. Li, and Y. Otsuki. SMU - MATLAB Package for Structural Model Updating. https://github.com/ywang-structures/Structural-Model-Updating, January 2019.

## Contact

Yang Wang, Ph.D.\
Associate Professor\
School of Civil and Environmental Engineering &\
School of Electrical and Computer Engineering\
Georgia Institute of Technology\
790 Atlantic Dr NW, Atlanta, GA 30332-0355\
E-mail: yang.wang@ce.gatech.edu\
Webpage: http://wang.ce.gatech.edu
