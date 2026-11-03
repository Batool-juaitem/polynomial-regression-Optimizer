# Polynomial Linear Regression – Optimization Algorithms

## Project Overview
This project implements and compares five optimization algorithms for Polynomial Linear Regression using the California Housing Prices dataset.

The main goal is to understand how different optimization algorithms affect model training, convergence, and prediction performance.

## Dataset
- **Name:** California Housing Prices
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/camnugent/california-housing-prices)
- **Target Variable:** `median_house_value`
- **Polynomial Degree:** 2

## Optimization Algorithms
The following algorithms were implemented from scratch using NumPy:

1. Gradient Descent (GD) with Momentum
2. Stochastic Gradient Descent (SGD) with Momentum
3. Mini-Batch Gradient Descent with Momentum
4. RMSProp with Momentum
5. Adam with Momentum

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Kaggle Notebooks

## Model Evaluation
The models were evaluated using:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score

## Results Comparison

| Optimizer | RMSE | MAE | R² |
|---|---:|---:|---:|
| GD with Momentum | 70,181.65 | 51,138.37 | 0.6241 |
| SGD with Momentum | 66,699.25 | 47,678.51 | 0.6605 |
| Mini-Batch GD with Momentum | 66,165.04 | 47,321.84 | 0.6659 |
| RMSProp with Momentum | 66,616.14 | 47,843.00 | 0.6613 |
| Adam with Momentum | 66,091.06 | 46,812.38 | 0.6667 |

## Conclusion
Adam with Momentum achieved the best overall performance among the five optimizers, with the highest R² score and the lowest error metrics.

The experiment demonstrates how optimization algorithms influence model convergence and predictive performance in Polynomial Linear Regression.

## Project Structure
- `01_GD_Polynomial_Regression.ipynb`
- `02_SGD_Polynomial_Regression.ipynb`
- `03_Mini_Batch_GD_Polynomial_Regression.ipynb`
- `04_RMSProp_Polynomial_Regression.ipynb`
- `05_Adam_Polynomial_Regression.ipynb`
- `06_Optimizers_Comparison.ipynb`

## Author
Created as a Machine Learning course project.
