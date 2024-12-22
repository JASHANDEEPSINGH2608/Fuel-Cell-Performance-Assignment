# Models Performance

This repository contains a comprehensive analysis of machine learning model performance using various preprocessing techniques. The project is structured to explore the impact of data preprocessing methods on the performance of a machine learning model using Target5 variable in Fuel-cell-Performance dataset

## Table of Contents
1. [Techniques and Approaches](#techniques-and-approaches)
2. [Usage](#usage)
3. [Dependencies](#dependencies)
4. [Project Structure](#project-structure)
5. [Results](#results)


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



## Project Structure
```
ML_Assignment/
|-- ML_Assignment.ipynb     # Main notebook with analysis
|-- data/                   # Dataset used in the analysis
|-- README.md               # Project documentation
```

## Results
## Model Performance Comparison

| Index | Model                    | Parameters                   | R² Score   |
|-------|--------------------------|------------------------------|------------|
| 0     | ExtraTreesRegressor      | None, 10 folds              | 0.7611     |
| 1     | ExtraTreesRegressor      | None - shuffle, 10 folds    | 0.7673     |
| 2     | LGBMRegressor            | None, 15 folds              | 0.7672     |
| 3     | GradientBoostingRegressor| None, 15 folds              | 0.7544     |
| 4     | ExtraTreesRegressor      | Normalization, 10 folds     | 0.7675     |
| 5     | ExtraTreesRegressor      | Normalization, 15 folds     | 0.7735     |
| 6     | ExtraTreesRegressor      | Feature Selection, 10 folds | 0.6901     |
| 7     | ExtraTreesRegressor      | Feature Selection, 15 folds | 0.6936     |
| 8     | LGBMRegressor            | Outlier Removal, 10 folds   | 0.7671     |
| 9     | LGBMRegressor            | Outlier Removal, 15 folds   | 0.7621     |
| 10    | ExtraTreesRegressor      | Transformation, 10 folds    | 0.7704     |
| 11    | LGBMRegressor            | Transformation, 15 folds    | 0.7682     |
| 12    | LGBMRegressor            | PCA, 10 folds               | 0.7768     |
| 13    | LGBMRegressor            | PCA, 15 folds               | 0.7710     |
| 14    | ExtraTreesRegressor      | N+OR, 10 folds              | 0.7606     |
| 15    | LGBMRegressor            | N+T, 10 folds               | 0.7680     |
| 16    | BayesianRidge            | N+PCA, 10 folds             | 0.7140     |
| 17    | ExtraTreesRegressor      | OR+PCA, 10 folds            | 0.7616     |
| 18    | LGBMRegressor            | OR+T, 10 folds              | 0.7619     |
| 19    | LGBMRegressor            | PCA+T, 10 folds             | 0.7696     |
| 20    | AdaBoostRegressor        | PCA - kernel, 10 folds      | -0.0099    |
| 21    | ExtraTreesRegressor      | PCA - incremental, 10 folds | 0.7680     |

## BEST MODEL
LGBMRegressor (0.7768)


