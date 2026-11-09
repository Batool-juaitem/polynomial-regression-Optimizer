# Polynomial Regression Using Different Optimization Algorithms

## Project Overview

This project implements Polynomial Regression to predict the Heating Load of buildings using the Energy Efficiency Dataset.

The main objective is to compare the performance of five different optimization algorithms and evaluate their prediction accuracy.

## Dataset

- **Dataset:** Energy Efficiency Dataset
- **Total Samples:** 768
- **Input Features:** 8
- **Target Variable:** Y1 (Heating Load)
- **Training Data:** 80%
- **Testing Data:** 20%

## Data Preprocessing

The following preprocessing steps were applied:

- Separated input features and target variables.
- Applied StandardScaler to numerical features.
- Applied OneHotEncoder to categorical features.
- Generated polynomial features using PolynomialFeatures with degree 2.
- Applied StandardScaler to the target variable.
- Split the dataset into training and testing sets using an 80/20 ratio.

## Optimization Algorithms

The project consists of five separate Jupyter Notebooks:

1. **gradient descent (gd)**
2. **stochastic gradient descent (sgd)**
3. **mini-batch gradient descent**
4. **rmsprop**
5. **adam**

## Evaluation Metrics

The models were evaluated using the following metrics:

- **MAE:** Mean Absolute Error
- **MSE:** Mean Squared Error
- **RMSE:** Root Mean Squared Error
- **R² Score:** Coefficient of Determination

## Final Results

| Optimizer | MAE | MSE | RMSE | R² Score |
|---|---:|---:|---:|---:|
| gd | 1.6835 | 5.6204 | 2.3707 | 0.9461 |
| sgd | 2.4362 | 10.1531 | 3.1864 | 0.9026 |
| mini-batch gd | 1.7623 | 6.4866 | 2.5469 | 0.9378 |
| rmsprop | 1.9965 | 8.9383 | 2.9897 | 0.9142 |
| adam | 1.7515 | 5.8876 | 2.4264 | 0.9435 |

## Conclusion

Based on the experimental results, gradient descent achieved the best overall performance among the five optimization algorithms.

It obtained the lowest MAE, MSE, and RMSE values, along with the highest R² score.

Adam achieved the second-best performance, showing that Adam is not always the best optimizer for every dataset.

The results demonstrate that optimizer performance depends on the dataset and the selected hyperparameters.

## Project Structure

1. `1_gd_polynomial_regression.ipynb`
2. `2_sgd_polynomial_regression.ipynb`
3. `3_minibatch_polynomial_regression.ipynb`
4. `4_rmsprop_polynomial_regression.ipynb`
5. `5_adam_polynomial_regression.ipynb`

## Tools and Libraries

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
