## Inverse Homogenization Topology Optimization of Vascular Stents Under Geometric Design Constraints

This repository contains the code and results for the project developed within the course *Numerical Analysis of Partial Differential Equations* (Academic Year 2024/2025) at Politecnico di Milano.

## Authors

- **Damiano Baschiera** — damiano.baschiera@mail.polimi.it  
- **Alice Cortinovis** — alice.cortinovis@mail.polimi.it

## Project Description

This project implements a numerical framework for the inverse homogenization-based topology optimization of vascular stent unit cells, coupled with anisotropic mesh adaptation. The goal is to design stent unit cells that minimize foreshortening during crimping, while satisfying mechanical and geometric constraints. The core methodology is based on the density-based SIMP formulation and is applied to retrieve microstructures with prescribed mechanical properties at the macroscale, as discussed in the accompanying report.

## Repository Structure

- **`main.edp`**  
  This is the FreeFem++ code implementing the full optimization pipeline. It performs the following steps:
  - Solution of the periodic cell problems to compute the homogenized stiffness tensor;
  - Evaluation of the objective functional (foreshortening) and enforcement of mechanical and geometric constraints;
  - Application of Helmholtz filtering and anisotropic mesh adaptation;
  - Constrained optimization via the *Ipopt* solver.

- **`results/`**  
  Contains `.vtk` files with:
  - Optimized density fields;
  - Contributions to the vertical constraint functional.

- **`Report_Baschiera_Cortinovis.pdf`**  
  The detailed report describing the mathematical formulation, numerical implementation, and results.  

## References

Please refer to the report [`Report_Baschiera_Cortinovis.pdf`](./Report_Baschiera_Cortinovis.pdf) for:
- Full mathematical formulation;
- Discussion of methods;
- Discussion of all numerical experiments.


## License

This code is intended for educational and academic use within the scope of the "Numerical Analysis of PDEs" course at Politecnico di Milano.
