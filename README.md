# Models Performance

This repository contains a comprehensive analysis of machine learning model performance using various preprocessing techniques. The project is structured to explore the impact of data preprocessing methods on the performance of a machine learning model using Target5 variable in Fuel-cell-Performance dataset

## Table of Contents
1. [Techniques and Approaches](#techniques-and-approaches)
2. [Usage](#usage)
3. [Dependencies](#dependencies)
4. [Project Structure](#project-structure)
5. [Results](#results)
6. [Contributing](#contributing)

## Techniques and Approaches
The notebook explores the following preprocessing techniques:

- **1.1 Model with No Parameters**: Baseline model without any preprocessing.
- **1.2 Normalization**: Evaluating the impact of data normalization.
- **1.3 Feature Selection**: Assessing the model’s performance with selected features.
- **1.4 Outlier Removal**: Analyzing the effect of removing outliers.
- **1.5 Transformation**: Applying data transformation techniques.
- **1.6 PCA**: Dimensionality reduction using Principal Component Analysis (PCA).

### Combined Techniques:
- **7.1 Normalization + Outlier Removal**
- **7.2 Normalization + Transformation**
- **7.3 Normalization + PCA**

## Usage
To explore the analysis and replicate the results:

1. Clone the repository:
   ```bash
   git clone <repository_url>
   ```

2. Install the required dependencies (see below).

3. Run the notebook `ML_Assignment.ipynb` using Jupyter Notebook or JupyterLab:
   ```bash
   jupyter notebook ML_Assignment.ipynb
   ```

## Dependencies
The project requires the following Python libraries:
- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`

Install all dependencies using:
```bash
pip install -r requirements.txt
```

## Project Structure
```
ML_Assignment/
|-- ML_Assignment.ipynb     # Main notebook with analysis
|-- data/                   # Dataset used in the analysis
|-- README.md               # Project documentation
```

## Results


