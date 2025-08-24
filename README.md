# Predicting Helmet Usage in Accidents: A Machine Learning Analysis

This project uses machine learning to predict whether a rider was wearing a helmet at the time of an accident, based on a dataset of accident reports. The primary goal is to identify key factors correlated with helmet use and to build an interpretable model to inform safety policies.

## Project Structure

```
.
├── accident_data.csv         # The raw dataset used for the analysis
├── Helmet_model.ipynb        # Main Jupyter Notebook with the full analysis
├── README.md                 # This file
└── ...                       # Other project files
```

## How to Run the Model

Follow these steps to set up your environment and run the analysis notebook.

### 1. Prerequisites

*   Python 3.8 or higher
*   `pip` and `venv` for package management

### 2. Setup Instructions

First, clone the repository and navigate into the project directory.

**Create and activate a virtual environment:**

*   **Windows:**
    ```bash
    python -m venv .venv
    .\.venv\Scripts\activate
    ```

*   **macOS / Linux:**
    ```bash
    python3 -m venv .venv
    source .venv/bin/activate
    ```

**Install the required packages:**

A `requirements.txt` file is recommended for larger projects, but you can install the necessary packages directly using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 3. Running the Analysis

Once your environment is set up and the packages are installed, you can run the analysis.

**Start Jupyter Notebook:**

From your terminal, run the following command to start the Jupyter Notebook server:

```bash
jupyter notebook
```

This will open a new tab in your web browser showing the project directory.

**Open and run the notebook:**

1.  Click on `Helmet_model.ipynb` to open it.
2.  To run the entire analysis from top to bottom, go to the menu and select **Cell > Run All**.
3.  Alternatively, you can run each cell individually by selecting it and pressing **Shift + Enter**.

### 4. Understanding the Model and Results

*   **Models Trained:** The notebook trains three models: Logistic Regression, Decision Tree, and Random Forest.
*   **Best Performing Model:** The **Logistic Regression** model was identified as the most reliable and interpretable model, as the other two showed significant signs of overfitting.
*   **Key Metric:** The analysis prioritizes **Precision** as the most important metric to ensure that safety interventions are targeted effectively and resources are not wasted.
*   **Results:** The final report sections in the notebook detail the model's performance, including its cross-validation scores, confusion matrix, and ROC curve analysis.
# Helmet Use Prediction Model

This guide explains how to recreate the machine learning model for predicting helmet use in motorcycle accidents using the provided notebooks and dataset.

## Prerequisites
- Python 3.8 or newer
- PowerShell (Windows) or Bash (Linux/Mac)
- Recommended: VS Code or Jupyter Lab

## 1. Clone or Download the Project
Download or clone the repository and ensure the following files are present:
- `accident_data.csv` (dataset)
- `newest.ipynb` (main notebook)
- `requirements.txt` (dependencies)

## 2. Set Up a Virtual Environment
Open PowerShell in the project folder and run:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

## 3. Install Required Packages
Install all dependencies:

```powershell
pip install -r requirements.txt
```

If using `uv` for fast installs:
```powershell
uv pip install -r requirements.txt --active
```

## 4. Start Jupyter Lab or VS Code
You can use either Jupyter Lab or VS Code to run the notebook:

```powershell
jupyter lab
```
Or open the folder in VS Code and launch the notebook interface.

## 5. Run the Notebook
Open `newest.ipynb` and run all cells in order. The notebook will:
- Import libraries
- Load and clean the data
- Visualize key distributions
- Engineer features
- Prepare train/test splits
- Train and evaluate Logistic Regression, Decision Tree, and Random Forest models
- Tune hyperparameters for the best model
- Show metrics, confusion matrix, ROC curve, and feature importances
- Summarize results

## 6. Reproduce Results
- Ensure all cells run without errors.
- If you want to use a different dataset, replace `accident_data.csv` and rerun the notebook.
- For custom model settings, adjust parameters in the notebook cells.

## Troubleshooting
- If you see import errors, check that your virtual environment is activated and all packages are installed.
- If you see kernel errors, ensure `ipykernel` is installed:
    ```powershell
    pip install ipykernel
    python -m ipykernel install --user --name helmet-venv --display-name "Python (.venv - Helmet)"
    ```
- For missing data columns, check your CSV file for correct formatting.

## Project Files
- `accident_data.csv` — main dataset
- `newest.ipynb` — main notebook for model creation
- `requirements.txt` — Python dependencies
- `README.md` — this guide

---

For questions or issues, open an issue in the repository or contact the project maintainer.
