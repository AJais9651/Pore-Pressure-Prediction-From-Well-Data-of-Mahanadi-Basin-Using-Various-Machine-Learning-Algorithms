## Machine Learning Models and Hyperparameters

This project implements four machine learning models to predict pore pressure (PP) values calculated using Eaton’s and Bower’s methods for individual wells. Below are the details of each model and their corresponding hyperparameters.

### 1. **Random Forest Regressor**
This model employs an ensemble learning method for regression tasks, optimizing predictions through a combination of decision trees.

| **Hyperparameter** | **Value**         |
|---------------------|-------------------|
| n_estimators        | 1000             |
| max_depth           | 20               |
| random_state        | 42               |
| criterion           | 'absolute_error' |

---

### 2. **Extreme Gradient Boosting Regressor (XGBoost)**
An advanced boosting algorithm designed for efficiency and accuracy, tuned for regression problems.

| **Hyperparameter**     | **Value**         |
|-------------------------|-------------------|
| n_estimators            | 100              |
| max_depth               | 3                |
| random_state            | 42               |
| objective               | 'reg:squarederror' |
| learning_rate           | 0.1              |
| min_child_weight        | 1                |
| gamma                   | 0                |
| subsample               | 0.8              |
| colsample_bytree        | 0.8              |

---

### 3. **K Nearest Neighbour Regressor (KNN)**
A non-parametric algorithm that predicts based on the similarity of neighboring data points.

| **Hyperparameter** | **Value**         |
|---------------------|-------------------|
| n_neighbors         | 10               |
| weights             | 'distance'       |
| algorithm           | 'auto'           |
| leaf_size           | 30               |
| p                   | 2                |

---

### 4. **Decision Tree Regressor**
A simple yet powerful model that splits data into subsets based on feature importance for regression tasks.

| **Hyperparameter** | **Value**         |
|---------------------|-------------------|
| max_depth           | None             |
| splitter            | 'best'           |
| random_state        | 100              |

---

These models were selected for their ability to handle varying data complexities and regression challenges. The hyperparameters were tuned to achieve optimal performance for pore pressure predictions.
