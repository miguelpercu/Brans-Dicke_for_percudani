# Brans-Dicke_for_percudani
estudio sobre brans dicke vs ACDM
markdown

Copy

Download
# Brans-Dicke vs ΛCDM Cosmological Analysis

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

## 📖 Description

Complete reproduction package for the research paper:

> **"Comparative Analysis: Brans-Dicke Theory vs ΛCDM Model using Pantheon Supernova Data"**  
> *Miguel Ángel Percudani*  
> *March 2025*

This repository contains the full computational pipeline demonstrating that Brans-Dicke theory with coupling parameter ω = 10 provides a better fit to Pantheon supernova data than the standard ΛCDM model (χ² = 5.62 vs 5.69, Δχ² = -0.069).

## 🚀 Quick Start for Peer Reviewers

### Prerequisites

- **Python 3.8+** 
- **Jupyter Notebook**
- Required packages: `numpy`, `scipy`, `matplotlib`, `pandas`

### Installation & Setup

```bash
# Clone the repository
git clone https://github.com/miguelpercu/Brans-Dicke_for_percudani.git
cd Brans-Dicke_for_percudani

# Install required packages
pip install numpy scipy matplotlib pandas astropy
One-Click Reproduction
Open Jupyter Notebook:

bash

Copy

Download
jupyter notebook
Run the main analysis script which executes the complete pipeline.

Manual Execution
If preferred, run the analysis step-by-step:

python

Copy

Download
# Import required libraries
import numpy as np
import matplotlib.pyplot as plt
from scipy.integrate import solve_ivp
import pandas as pd
import warnings
warnings.filterwarnings('ignore')

# Execute the analysis
exec(open('brans_dicke_analysis.py').read())
📁 Repository Structure
text

Copy

Download
Brans-Dicke_for_percudani/
├── brans_dicke_analysis.py          # Main analysis script (Jupyter-compatible)
├── figures/                         # Generated visualizations
│   └── comprehensive_analysis.png   # Main results figure
├── tables/                          # Parameter tables
│   └── cosmological_parameters.csv
├── data_observations/               # Observational data
│   └── observational_data.csv
├── data_curves/                     # Theoretical predictions
│   └── theoretical_curves.csv
└── statistical_analysis/            # Statistical results
    ├── statistical_results.csv
    └── best_fit_summary.csv
🔬 Key Results
Statistical Comparison
Model	Best ω	χ²	χ²_reduced	Δχ² vs ΛCDM
ΛCDM	-	5.69	0.219	-
Brans-Dicke	10	5.62	0.216	-0.069
Parameter Space Analyzed
ω values tested: [10, 50, 100, 500, 1000, 2000, 5000, 10000]

Redshift range: z ∈ [0.01, 2.0]

Data points: 28 Pantheon supernovae

🧪 Code Verification
Expected Output
Successful execution should generate:

text

Copy

Download
=== COSMOLOGICAL ANALYSIS: Brans-Dicke vs ΛCDM (FINAL) ===
✓ Created directory structure
✓ Loaded Pantheon data: 28 points
✓ Statistical analysis completed
✓ Best fit: ω = 10, χ² = 5.62, Δχ² = -0.069
✓ Analysis plots generated and saved
Output Files Verification
Check these files are generated:

figures/comprehensive_analysis.png (4-panel results figure)

statistical_analysis/statistical_results.csv (complete χ² table)

best_fit_summary.csv (best model parameters)

🔧 Technical Details
Numerical Methods
Brans-Dicke solver: Adaptive Runge-Kutta (RK45)

Statistical analysis: Marginalized χ² with normalization

Integration: Trapezoidal rule with 100-point sampling

Cosmological Parameters
python

Copy

Download
H0 = 70.0           # km/s/Mpc
Omega_m0 = 0.3      # Matter density
Omega_DE0 = 0.7     # Dark energy density
📊 Data Sources
Pantheon Supernova Survey: 28 data points (z = 0.01-2.0)

Distance modulus with associated uncertainties

Self-consistent covariance matrix handling

🐛 Troubleshooting
Common Issues
Package conflicts: Use a clean Python environment

Matrix loading errors: Ensure numpy version ≥ 1.21

Plot generation issues: Check matplotlib backend

Verification Steps
python

Copy

Download
# Test basic functionality
import numpy as np
from scipy.integrate import solve_ivp
print("✓ Basic imports successful")

# Test cosmology calculations
from astropy.cosmology import FlatLambdaCDM
cosmo = FlatLambdaCDM(H0=70, Om0=0.3)
print("✓ Cosmology calculations working")
📄 Citation
If using this code in research, please cite:

bibtex

Copy

Download
@article{percudani2025bransdicke,
  title={Comparative Analysis: Brans-Dicke Theory vs ΛCDM Model using Pantheon Supernova Data},
  author={Percudani, Miguel Ángel},
  journal={Preprint},
  year={2025},
  url={https://github.com/miguelpercu/Brans-Dicke_for_percudani}
}
📧 Contact
Miguel Ángel Percudani

Email: miguel_percudani@yahoo.com.ar

GitHub: @miguelpercu

Related work: UAT Framework

🙏 Acknowledgments
Pantheon collaboration for supernova data

Developers of scientific Python packages

Reviewers for valuable feedback
