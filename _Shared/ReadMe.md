# ReadMe.md

**Table of Contents**
<img src="http://latex.codecogs.com/gif.latex?n_{modes}&space;\times&space;1" title="n_modes \times 1" />

# StructModelUpdating.m
This function performs one run of the finite element model updating usingmfrequency domain modal properties. The starting point for this run can be provided as optimzOpts.x0.
## Syntax
function updtResults = StructModelUpdating (structModel, expModes)
function updtResults = StructModelUpdating (structModel, expModes, updatingOpts)
function updtResults = StructModelUpdating (structModel, expModes, [], optimzOpts)
function updtResults = StructModelUpdating (structModel, expModes, updatingOpts, optimzOpts)
## Description
### Input Arguments
#### structModel - a MATLAB structure array with following fields of structural model information:
|Field Name |Dimension       |Description                    |
|:----------|:---------------|:------------------------------|
|M0         |N x N           |mass matrix (assumed accurate enough and no need to update in current revision). Here N refers to the number of degrees of freedom of the finite element model |
|K0         |N x N           |nominal stiffness matrix constructed with nominal parameter values |
|K_j        |N x N x n_alpha |influence matrix corresponding to updating variables (Note: the third dimension of K_j should be equal to the number of updating variables). Here n_alpha refers the number of stiffness updating variables |
#### expModes - a MATLAB structure array with experimental modal properties for model updating:
|Field Name    |Dimension        |Description                    |
|:-------------|:----------------|:------------------------------|
|lambdaExp     |n_modes x 1      |experimental eigenvalue. Here n_modes refers to the number of experimental modes available |
|psiExp        |n_meas x n_modes |experimental mode shape vector at measured DOFs. Here n_meas refers to the number of measured DOFs |
|measDOFs      |n_meas x 1       |measured DOFs |
|lambdaWeights |n_modes x 1      |weighting factor for eigenvalue |
|psiWeights    |n_modes x 1      |weighting factor for eigenvector |

<table>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>
