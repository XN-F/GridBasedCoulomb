# Code for Grid-Based Simulation of Coulombic Dynamics

This repository contains the Python code supporting the manuscript: **[Improved Grid-Based Simulation of Coulombic Dynamics]**

### Repository Contents

- `Potential Correction.ipynb`: This script generates the corrected potentials for 2-electron quantum ring and 2D hydrogen systems. The number of correction grid points can be adjusted via the parameter `Ncorre`.

- `Main Simulation of 2D Hydrogen.ipynb`: This script generates the autocorrelation data for the 2D hydrogen system. Users may switch between corrected and uncorrected potentials and wavefunctions by commenting or uncommenting the corresponding lines.

  Note: The corrected wavefunction requires the value of `Edynamic`, which is obtained from an initial run using the uncorrected wavefunction.

- `Main Simulation of 2-Electron Ring.ipynb`: This script generates the autocorrelation data for the 2-electron quantum ring system. Users may switch between corrected and uncorrected potentials by activating the corresponding lines.

### Usage Notes
Please note that the most computationally demanding part is the seventh code block of Potential Correction.ipynb. On a standard laptop (Intel i5 processor, 16 GB RAM), this step took 30-40 minutes when executed with Ncorre = 800.

Please refer to the manuscript for details on methods, parameters, and interpretation of the results.

### Requirements

- Python 3.11.4
- Jupyter Notebook (ipykernel)

### Software Environment
The code has been tested with the following libraries and versions:

- numpy==1.23.5
- scipy==1.10.1
- matplotlib==3.7.1
- jupyter==1.0.0
