# BEAM 📡
**B**roadside **E**lectromagnetic **A**rray **M**odeler

A comprehensive Python-based simulation tool for analyzing and visualizing dipole antenna arrays. Developed as a Jupyter Notebook, this project models the electromagnetic behavior of half-wave dipoles, calculates combined array factors, and demonstrates the principles of phased arrays through electronic beam steering.

## 🚀 Features
* **Single Dipole Analysis:** Evaluates a standalone half-wave dipole at 1 GHz, calculating the input impedance match (S11 parameter), performing frequency sweeps, and rendering the baseline omnidirectional and figure-eight radiation patterns.
* **Linear Array Modeling:** Computes the Element Factor (EF) and Array Factor (AF) for an $N$-element linear array (configured for 10 elements with $\lambda/2$ spacing) to demonstrate enhanced directivity, main lobe narrowing, and side lobe generation.
* **Electronic Beam Steering:** Implements progressive phase shifting to dynamically steer the main beam across multiple angles (in 45° increments). It utilizes the standard steering equation $\alpha = -kd \cos(\theta_0)$ to achieve directional control without mechanical movement.
* **Rich 2D & 3D Visualizations:** Generates high-quality spatial representations, including 3D geometric models of the antennas, 3D surface radiation patterns, and 2D polar plots for both Azimuth (H-plane) and Elevation (E-plane) cuts.

## 🛠️ Technology Stack
This project is built using **Python 3** within a **Jupyter Notebook** environment. It relies on the following core libraries:
* **NumPy:** For handling complex array operations, trigonometric calculations, grid meshing, and signal processing math.
* **Matplotlib:** Used extensively for all data visualization. Specifically leverages `pyplot`, `cm` (colormaps like 'plasma'), and `mpl_toolkits.mplot3d` for the 3D surface and line plots.

## ⚙️ Installation & Usage
To run this notebook locally, you will need Python installed along with Jupyter and the required scientific libraries.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/BFG508/BEAM
2. **Install the required dependencies:**
It is recommended to use a virtual environment. Install the packages via pip:
    ```bash
        pip install numpy matplotlib jupyter
3. **Launch the simulation:**
Navigate to the repository folder and start the Jupyter Notebook server:
    ```bash
    jupyter notebook BEAM.ipynb
4. **Run the cells:** Execute the notebook sequentially to compute the S11 parameters, build the array arrays, and generate the final 3D visualizations and beam steering patterns.