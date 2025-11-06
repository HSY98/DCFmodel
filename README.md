# DCFmodel
Scripts for DCF model applied in Titanium hydrogen storage tank simulation. DCF model is combined with Descrete Element Method (DEM), Computational Fluid Dynamics (CFD), Finite Element Method (FEM), and Bayesian Optimization (BO). It serves as a comprehensive toolkit for researchers and engineers working on the numerical analysis, optimization, and performance prediction of alloy-based hydrogen storage systems.
## Repository Contents

The repository is organized into three core modules, each addressing a key aspect of the titanium-based hydrogen storage device simulation workflow:

### 1. Discrete Element Method (DEM) Code



* **Purpose**: Implements the DEM algorithm tailored for simulating the mechanical behavior, particle-particle interactions, and dynamic contact forces (DCF) of the titanium-based storage medium during hydrogen absorption/desorption cycles.

* **Key Features**: Includes pre-defined material properties for titanium alloys, customizable particle size distributions, and contact force models optimized for hydrogen storage applications.

* **Usage**: Suitable for simulating granular flow, stress distribution, and structural deformation of the titanium storage bed under different operating conditions (e.g., temperature, pressure).

### 2. Block Packing STL Models



* **Purpose**: Provides ready-to-use STL (Standard Tessellation Language) models representing the **packed structure of titanium-based storage blocks**—a critical component for accurate DEM and multiphysics simulation setup.

* **Model Details**: The STL files are generated based on realistic packing densities and geometric configurations of titanium blocks, ensuring consistency with industrial-scale hydrogen storage device designs.

* **Compatibility**: Can be directly imported into DEM simulation software (e.g., LIGGGHTS, EDEM) or multiphysics platforms (e.g., COMSOL Multiphysics) for mesh generation and simulation initialization.

### 3. Bayesian Optimization Code for COMSOL Multiphysics Coupling



* **Purpose**: Enables **Bayesian optimization-driven parameter tuning** for multiphysics simulations of titanium-based hydrogen storage devices, with seamless integration with COMSOL Multiphysics.

* **Core Functionality**:


  * Automates the coupling between DEM-derived data (e.g., stress, porosity) and COMSOL’s multiphysics models (e.g., hydrogen diffusion, heat transfer).

  * Uses Bayesian optimization to minimize computational cost while maximizing the accuracy of key performance indicators (e.g., hydrogen storage capacity, charging/discharging rate).

* **Dependencies**: Requires COMSOL Multiphysics (v5.6+ recommended) and Python libraries for Bayesian optimization (e.g., `GPyOpt`, `scikit-learn`).

## Getting Started

1. Clone this repository to your local machine using:

   `git clone ``https://github.com/HSY98/DCFmodel.git`

2. Refer to the `README.md` for detailed parameter configuration tutorials and COMSOL coupling workflows.

3. For DEM simulations: Navigate to the `dem_code/` directory and follow the `README.md` inside to set up input parameters and run simulations.

4. For Bayesian optimization: Check the `bayesian_optimization/` folder for example scripts and COMSOL API integration steps.

## Contributing

Contributions to improve the codebase, add new simulation features, or expand documentation are welcome.

## License

This repository is licensed under the MIT License. See the `LICENSE` file for full terms and conditions.

## Contact

For questions, bug reports, or collaboration inquiries, please contact:

\Shouyi Hu - \blueblood@sjtu.edu.cn

Project Link: https://github.com/HSY98/DCFmodel
