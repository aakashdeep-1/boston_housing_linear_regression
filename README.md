# Boston Housing Linear Regression

A beginner-friendly machine learning project exploring the **Boston Housing dataset** and preparing the data for a linear regression model to predict housing prices.

## Overview

The project includes:

* Loading the Boston Housing dataset
* Exploratory data analysis
* Checking for missing values
* Handling missing observations
* Correlation analysis
* Correlation heatmap
* Identifying variables strongly related to housing prices
* Visualizing relationships between features and housing prices
* Creating a feature dataset for linear regression

## Dataset

The dataset contains **506 observations** and **14 columns**.

### Features

| Column    | Description                                          |
| --------- | ---------------------------------------------------- |
| `CRIM`    | Per capita crime rate                                |
| `ZN`      | Proportion of residential land zoned for large lots  |
| `INDUS`   | Proportion of non-retail business acres              |
| `CHAS`    | Charles River dummy variable                         |
| `NOX`     | Nitric oxide concentration                           |
| `RM`      | Average number of rooms per dwelling                 |
| `AGE`     | Proportion of owner-occupied units built before 1940 |
| `DIS`     | Weighted distance to employment centres              |
| `RAD`     | Index of accessibility to radial highways            |
| `TAX`     | Property tax rate                                    |
| `PTRATIO` | Pupil-teacher ratio                                  |
| `B`       | Proportion of population of lower status             |
| `LSTAT`   | Percentage of lower-status population                |
| `MEDV`    | Median value of owner-occupied homes                 |

## Exploratory Analysis

The analysis identified **`LSTAT`** and **`RM`** as the two strongest predictors of `MEDV` based on their correlation with the target variable.

The notebook visualizes these relationships using:

* Scatter plots
* Correlation heatmap
* 3D scatter plot of `LSTAT`, `RM`, and `MEDV`

## Data Preprocessing

The dataset contains **5 missing values in `RM`**.

These observations are removed before performing the correlation analysis and further processing.

The final feature set used for the planned regression model consists of:

```text
LSTAT
RM
```

with:

```text
Target: MEDV
```

## Tools & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Project Structure

```text
boston_housing_linear_regression/
│
├── notebook/
│   └── Boston_linear_regression.ipynb
│
├── data/
│   └── BostonHousing.csv
│
└── README.md
```

## Notebook

The complete analysis is available in:

`notebook/Boston_linear_regression.ipynb`
