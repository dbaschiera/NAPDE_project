## Inverse Homogenization Topology Optimization of Vascular Stents Under Geometric Design Constraints

This repository contains the code and results for the project developed within the course *Numerical Analysis of Partial Differential Equations* (Academic Year 2024/2025) at Politecnico di Milano.

## Authors

- **Damiano Baschiera** — damiano.baschiera@mail.polimi.it  
- **Alice Cortinovis** — alice.cortinovis@mail.polimi.it

## Project Description

This project implements a numerical framework for the optimization of vascular stent unit cells via inverse homogenization coupled with anisotropic mesh adaptation. The core methodology is based on the density-based SIMP formulation and is applied to retrieve microstructures with prescribed mechanical properties at the macroscale, as discussed in the accompanying report.

## Repository Structure

- **`main.edp`**  
  This is the FreeFem++ code implementing the full optimization loop for unit cell design, including:
  - Computation of the homogenized stiffness tensor via periodic problems;
  - Evaluation of the cost function
  - Adaptive anisotropic mesh refinement following the microSIMPATY algorithm.

- **`results/`**  
  This folder contains `.vtk` files with the optimized density fields and constraint contribution of each part of them.

- **`Report_Baschiera_Cortinovis.pdf`**  
  The detailed report describing the formulation, numerical implementation, and results.  

## References

Please refer to the report [`Report_Baschiera_Cortinovis.pdf`](./Report_Baschiera_Cortinovis.pdf) for:
- Full mathematical formulation;
- Discussion of methods;
- Discussion of all numerical experiments.


## License

This code is intended for educational and academic use within the scope of the "Numerical Analysis of PDEs" course at Politecnico di Milano.
