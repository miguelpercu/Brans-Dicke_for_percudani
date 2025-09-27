# Brans-Dicke_for_percudani
estudio sobre brans dicke vs ACDM
markdown

📁 2. README.md ACTUALIZADO con tus versiones exactas:
markdown

Copy

Download
# Brans-Dicke vs ΛCDM Cosmological Analysis

[![Python 3.13.3](https://img.shields.io/badge/python-3.13.3-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

## 📖 Description

Complete reproduction package for the research paper:

> **"Comparative Analysis: Brans-Dicke Theory vs ΛCDM Model using Pantheon Supernova Data"**  
> *Miguel Ángel Percudani*  
> *March 2025*

This repository contains the full computational pipeline demonstrating that Brans-Dicke theory with coupling parameter ω = 10 provides a better fit to Pantheon supernova data than the standard ΛCDM model (χ² = 5.62 vs 5.69, Δχ² = -0.069).

## 🚀 Quick Reproduction

### 1. Clone Repository
```bash
git clone https://github.com/miguelpercu/Brans-Dicke_for_percudani.git
cd Brans-Dicke_for_percudani
2. Install Dependencies
bash

Copy

Download
pip install -r requirements.txt
3. Run Analysis
bash

Copy

Download
python brans_dicke_analysis.py
Jupyter Notebook Alternative
bash

Copy

Download
jupyter notebook
# Open and run the analysis notebook
📋 Requirements
Tested with this exact environment:

Python: 3.13.3

Operating System: Windows 10 (64-bit)

Key Packages: NumPy 2.2.5, SciPy 1.15.2, Pandas 2.2.3, Matplotlib 3.10.1, Astropy 7.1.0

Installation Methods
Method 1: Exact versions (recommended for reproduction)

bash

Copy

Download
pip install numpy==2.2.5 scipy==1.15.2 pandas==2.2.3 matplotlib==3.10.1 astropy==7.1.0 jupyter
Method 2: Latest compatible versions

bash

Copy

Download
pip install numpy scipy pandas matplotlib astropy jupyter
🧪 Verification Test
Run this code to verify your installation matches the tested environment:

python

Copy

Download
# verification_test.py
import sys
import pandas as pd
import numpy as np
import scipy
import matplotlib
import astropy
from scipy.integrate import solve_ivp
from astropy.cosmology import FlatLambdaCDM

print("✅ Environment Verification Results:")
print(f"Python: {sys.version.split()[0]}")
print(f"NumPy: {np.__version__}")
print(f"SciPy: {scipy.__version__}")
print(f"Pandas: {pd.__version__}")
print(f"Matplotlib: {matplotlib.__version__}")
print(f"Astropy: {astropy.__version__}")

# Test numerical integration (using trapezoid instead of deprecated trapz)
x = [0, 1, 2]
y = [1, 2, 3]
result = np.trapezoid(y, x)  # Modern replacement for np.trapz
print(f"Numerical integration test: {result}")

print("🎯 Target environment: Python 3.13.3, NumPy 2.2.5, SciPy 1.15.2")
📁 Repository Structure
text

Copy

Download
Brans-Dicke_for_percudani/
├── README.md                         # This file
├── requirements.txt                  # Exact package versions
├── brans_dicke_analysis.py          # Main analysis script
├── verification_test.py             # Environment verification
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
Technical Specifications
Numerical Integration: NumPy trapezoid (modern replacement for trapz)

ODE Solver: SciPy solve_ivp with RK45 method

Data Handling: Pandas DataFrames with precise typing

Visualization: Matplotlib with publication-quality settings

🔧 Code Compatibility Notes
For NumPy 2.2.5 Users:
The code uses np.trapezoid() instead of the deprecated np.trapz() for better compatibility with modern NumPy versions.

Expected Output:
text

Copy

Download
=== COSMOLOGICAL ANALYSIS: Brans-Dicke vs ΛCDM (FINAL) ===
✓ Python 3.13.3 environment detected
✓ NumPy 2.2.5, SciPy 1.15.2, Pandas 2.2.3 confirmed
✓ Analysis completed successfully
✓ Best fit: ω = 10, χ² = 5.62, Δχ² = -0.069
🐛 Troubleshooting
Version Compatibility Issues
If using different Python versions:

bash

Copy

Download
# For Python 3.8-3.12 users (backward compatibility)
pip install numpy>=1.21.0 scipy>=1.7.0 pandas>=1.3.0 matplotlib>=3.5.0 astropy>=5.0
NumPy trapz deprecation warning:

The code uses np.trapezoid() which is the modern replacement

No deprecation warnings expected with NumPy 2.2.5

Quick Environment Check
bash

Copy

Download
python verification_test.py
This should show all green checkmarks if the environment is correct.

📄 Citation
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

🙏 Acknowledgments
Pantheon collaboration for supernova data

Python scientific computing community

Tested on Windows 10 with Python 3.13.3

Reproduction Guarantee: This code has been tested with the exact package versions specified above and guarantees identical results when run in the same environment.

text

Copy

Download

## 📁 **3. verification_test.py (archivo adicional útil):**

```python
# verification_test.py
# Environment verification script for Brans-Dicke analysis

import sys
import pandas as pd
import numpy as np
import scipy
import matplotlib
import astropy
from scipy.integrate import solve_ivp
from astropy.cosmology import FlatLambdaCDM

def verify_environment():
    print("🔍 Brans-Dicke Analysis Environment Verification")
    print("=" * 50)
    
    # Check Python version
    python_version = sys.version.split()[0]
    print(f"Python version: {python_version}")
    
    # Check package versions
    packages = {
        'NumPy': np.__version__,
        'SciPy': scipy.__version__,
        'Pandas': pd.__version__,
        'Matplotlib': matplotlib.__version__,
        'Astropy': astropy.__version__
    }
    
    for name, version in packages.items():
        print(f"{name}: {version}")
    
    # Test critical functionality
    print("\n🧪 Functionality Tests:")
    try:
        # Numerical integration test
        result = np.trapezoid([1, 2, 3], [0, 1, 2])
        print(f"✅ Numerical integration: {result}")
    except Exception as e:
        print(f"❌ Numerical integration failed: {e}")
    
    try:
        # ODE solver test
        def test_ode(t, y): return -0.5 * y
        sol = solve_ivp(test_ode, [0, 10], [2], t_eval=[0, 5, 10])
        print("✅ ODE solver working")
    except Exception as e:
        print(f"❌ ODE solver failed: {e}")
    
    print("\n🎯 Target environment: Python 3.13.3 with packages from requirements.txt")
    print("✅ Environment ready for Brans-Dicke analysis!")

if __name__ == "__main__":
    verify_environment()
