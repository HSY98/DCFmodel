# DCFmodel
Supporting Information for DCF model applied in Titanium hydrogen storage tank simulation. DCF model is combined with Descrete Element Method (DEM), Computational Fluid Dynamics (CFD), Finite Element Method (FEM), and Bayesian Optimization (BO). It serves as a comprehensive toolkit for researchers and engineers working on the numerical analysis, optimization, and performance prediction of alloy-based hydrogen storage systems.
## Repository Contents

The repository is organized into three core modules, each addressing a key aspect of the titanium-based hydrogen storage device simulation workflow:

### 1. Discrete Element Method (DEM) Code



* **Purpose**: Implements open-source software YADE for simulating the mechanical behavior, particle-particle interactions, and stacking state of the Titanium-based storage bulks during accumulation process.

* **Key Features**: Includes pre-defined material properties for storage bulks, customizable bulk size, and randomly distributed bulk positions.

* **Usage**: Suitable for simulating stacking state of the titanium storage bed under gravity.

### 2. Block Packing STL Models


* **Purpose**: Provides ready-to-use STL (Standard Tessellation Language) models representing the **packed structure of titanium-based storage bulks**—a critical component for accurate CFD and multiphysics simulation setup.

* **Model Details**: The STL files are generated based on DEM simulation result of Titanium blocks, ensuring consistency with industrial-scale hydrogen storage device designs.

* **Compatibility**: Can be directly imported into FEM multiphysics platforms (e.g., COMSOL Multiphysics) for mesh generation and further simulation.

### 3. Bayesian Optimization Code for COMSOL Multiphysics Coupling


* **Purpose**: Enables **Bayesian optimization-driven parameter tuning** for multiphysics simulations of titanium-based hydrogen storage devices, with seamless integration with COMSOL Multiphysics.

* **Core Functionality**:
  * Automates the coupling between BO parameters and COMSOL’s multiphysics models (two equivalent heat transfer coefficients).

  * Uses Bayesian optimization to minimize errors between simulation result and experiment data.

* **Dependencies**:
* COMSOL Multiphysics (v6.2 recommended). 
* Python libraries. 'bayesian-optimization'for Bayesian optimization and 'mph' for communicating with COMSOL.

## Getting Started

1. Clone this repository to your local machine using:

   `git clone https://github.com/HSY98/DCFmodel.git`

2. Refer to the `README.md` for detailed parameter configuration tutorials and COMSOL coupling workflows.

3. For DEM simulations: Navigate to the `dem_code/` directory and follow the `README.md` inside to set up input parameters and run simulations.

4. For Bayesian optimization: Check the `bayesian_optimization/` folder for example scripts and COMSOL API integration steps.

## Contributing

Contributions to improve the codebase, add new simulation features, or expand documentation are welcome.

## License

This repository is licensed under the MIT License. See the `LICENSE` file for full terms and conditions.

## Contact

For questions, bug reports, or collaboration inquiries, please contact:

Shouyi Hu - blueblood@sjtu.edu.cn

Project Link: https://github.com/HSY98/DCFmodel
