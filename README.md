## Courseware on Finite Element Methods

[![View Courseware on Finite Element Methods on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://www.mathworks.com/matlabcentral/fileexchange/125135-courseware-on-finite-element-methods) or [![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=MathWorks-Teaching-Resources/Courseware-on-Finite-Element-Methods&project=CoursewareonFiniteElementMethods.prj)

**Curriculum Module**  
_Created with R2022b. Compatible with R2022b and later releases._  

## Description ##

This courseware on Finite Element Methods addresses standard and advanced Finite Element formulations for shear-deformable lightweight structures of the Timoshenko beam and Reissner-Mindlin plate types.\
\
Moreover, the interactive courseware uses extensively the [MATLAB&reg;](https://www.mathworks.com/products/matlab.html) Live Editor and the [Symbolic Math Toolbox&trade;](https://www.mathworks.com/products/symbolic.html) for the development and the presentation.\
\
Additionally, a comprehensive (but not exhaustive) set of [MATLAB Grader](https://grader.mathworks.com/) assignments for this material exist. These assignments touch upon the topics mentioned in each of the chapters in the courseware syllabus. Please reach out to Andreas Apostolatos ([aapostol@mathworks.com](mailto:aapostol@mathworks.com)) to request access to the underlying MATLAB Grader assignments.\
\
Please refer to the recording **``Introduction-to-the-Courseware-on-Finite-Element-Methods.mp4``** under folder **``Introduction/``** for a short introduction on how to use the courseware along with its main highlights

## Owner/s
Andreas Apostolatos, PhD ([aapostol@mathworks.com](mailto:aapostol@mathworks.com))

## Contents
The repository contains the following Live Scripts and folders:

- **``CoursewareonFiniteElementMethods.prj``**\
This is the MATLAB project file which sets up all necessary dependencies

- **``main.mlx``**\
This is the main document that can be used to navigate to the rest of the Live Scripts in the repository

- **``main_unitTests.mlx``**\
This is the Live Script that executes the unit tests

- **``1_BasisFunctions/``**\
This folder contains the Live Script addressing the construction of the Finite Element basis functions
  - **``main_Chapter1_BasisFunctions.mlx``**

![basis_functions](https://user-images.githubusercontent.com/93076320/220189039-4c6cf9da-065c-4274-8f32-808254e34b6a.gif)\
(This animation can be generated using script ``main_Chapter3_AShearDeformablePlateElement.mlx`` in Chapter 3)

- **``2_TimoshenkoBeam/``**\
This folder contains the Live Script addressing the variational formulation and Finite Element approximation of the Timoshenko beam problem
  - **``main_Chapter2_ALinearStraightTimoshenkoBeamElement.mlx``**

<img src="https://user-images.githubusercontent.com/93076320/220361943-ae52101a-8bb4-4de6-a00a-9e8feb2cd3bd.png" width="50%">

- **``3_ReissnerMindlinPlate/``**\
This folder contains the Live Scripts addressing the variational formulation and Finite Element approximation of the Reissner-Mindlin plate problem
  - **``main_Chapter3_AShearDeformablePlateElement.mlx``**

<img src="https://user-images.githubusercontent.com/93076320/220361987-0e310c93-f57d-4ca3-bea9-c3ce2c922543.png" width="50%">

- **``4_TransverseShearLocking/``**\
This folder contains the Live Scripts highlighting and addressing the transverse-shear locking:
  - **``main_Chapter4_TransverseShearLocking_TimoshenkoBeam.mlx``**
  - **``main_Chapter4_Locking_ReissnerMindlinCantileverPlate.mlx``**
  - **``main_Chapter4_Locking_ReissnerMindlinSquarePlate.mlx``**

<img src="https://user-images.githubusercontent.com/93076320/220362061-f5e029b3-4302-474d-8b8d-12bc04d1c859.png" width="50%">

- **``5_WeakDirichletBoundaryConditions/``**\
This folder contains the Live Script addressing the weak application of Dirichlet boundary conditions for the Timoshenko beam problem
  - **``main_Chapter5_WeakBoundaryConditions_TimoshenkoBeam.mlx``**

<p float="left">
  <img src="https://user-images.githubusercontent.com/93076320/220362151-fe73acd1-d2c0-4d60-ac30-e645965bcfc2.png" width="45%">
  <img src="https://user-images.githubusercontent.com/93076320/220367398-9ed95db7-bca1-4e49-9851-7eef4acad5c6.png" width="45.8%"> 
</p>

- **``6_HellingerReissnerFormulation/``**\
This folder contains the Live Scripts addressing the variational formulation of the Timoshenko beam problem by means of the Hellinger-Reissner principle
  - **``main_Chapter6_HellingerReissnerFormulation_TimoshenkoBeam.mlx``**
  - **``main_Chapter6_HellingerReissnerFormulation_TimoshenkoBeam_Study.mlx``**

<img src="https://user-images.githubusercontent.com/93076320/220362740-104ea5a5-9b12-4c1f-92b5-a52805b1f966.png" width="85%">
<img src="https://user-images.githubusercontent.com/93076320/220363390-79ca64ed-746b-4e46-8907-7a32b768c161.png" width="45%">

- **``AppexA_EfficiencyConsiderations/``**\
This folder contains the Live Scripts demonstrating the runtime performance speedup by using page-wise computation of the element stiffness matrices and sparse assembly
  - **``main_AppexA_EfficiencyCondiderationsReissnerMindlinPlate.mlx``**
  - **``main_AppexA_EfficiencyCondiderationsTimoshenkoBeam.mlx``**

<img src="https://user-images.githubusercontent.com/93076320/220362807-240cc55a-d464-4482-9da7-168b4b2d4bf8.png" width="55%">

- **``TimoshenkoBeam/``**\
This folder contains all functions needed for the Finite Element discretization of the Timoshenko beam problem

- **``EulerBernoulliBeam/``**\
This folder contains all functions needed for the Finite Element discretization of the Bernoulli beam problem

- **``ReissnerMindlinPlate/``**\
This folder contains all functions needed for the Finite Element discretization of the Reissner-Mindlin plate problem

- **``utilityFunctions/``**\
This folder contains all auxiliary functions, such the computation of the basis functions, functions related to visualization and functions for the numerical integration among others

- **``unitTest/``**\
This folder contains all classes and functions needed for the unit testing performed by means of the Live Script ``main_unitTests.mlx``

## Concepts
Finite Element Methods, lightweight structures, Timoshenko beam, Reissner-Mindlin plate, transverse-shear locking, high-order basis functions, assumed natural strain, Hellinger-Reissner principle, slenderness study, convergence study, analytical solutions, [Live Functions](https://www.mathworks.com/help/matlab/matlab_prog/create-live-functions.html), [Local Functions](https://www.mathworks.com/help/matlab/matlab_prog/local-functions.html), [Symbolic Math Toolbox&trade;](https://www.mathworks.com/products/symbolic.html), plotting, [unit-testing](https://www.mathworks.com/help/matlab/matlab_prog/ways-to-write-unit-tests.html), [MATLAB Projects](https://www.mathworks.com/help/matlab/projects.html), [Git-integration](https://www.mathworks.com/help/matlab/matlab_prog/set-up-git-source-control.html)

## Suggested Audience
All engineering disciplines, such as, civil engineers, mechanical engineers, etc.

## Workflow
Firstly, open the project file CoursewareonFiniteElementMethods.prj to have all the folder dependencies resolved. Then, open Live Script **main.mlx**, go to Section **Quick guide**, select any of the desirable Live Scripts from the list, and hit Run!

## Unit-testing framework
To run the unit tests for this courseware, just type the following commands in the Command Window of MATLAB\
``>> suite = matlab.unittest.TestSuite.fromProject("CoursewareonFiniteElementMethods.prj");``\
``>> run(suite)``\
Alternatively, start the project and then run the file ``main_unitTests.mlx``

## Release last tested
R2022b

## TODO
- Add the Finite Element discretization of the Euler-Bernoulli beam using the third order Hermitian basis functions
- Add structural dynamics

## Revision History

