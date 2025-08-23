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
