# Helmet-Machine-Learning-Prediction

Brief instructions to run `helmet_accident_analysis.ipynb`:

Prerequisites
- Python 3.8+ and a virtual environment (recommended).
- A working `pip` installation.

Setup (PowerShell)
1. Create and activate venv:

	python -m venv .venv
	.\\.venv\\Scripts\\Activate.ps1

2. Install core packages:

	pip install -r requirements.txt

If `requirements.txt` is not available, install minimal packages:

	pip install pandas numpy matplotlib seaborn scikit-learn jupyterlab nbformat nbconvert python-docx

Running the notebook
- Open the workspace in VS Code and open `helmet_accident_analysis.ipynb`, then run cells interactively.
- Or start Jupyter Lab in the project root:

jupyter lab nd open the notebook from the browser.