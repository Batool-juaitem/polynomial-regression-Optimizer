# Polynomial Linear Regression: Optimization Algorithms

## Project Overview

This project implements and compares five optimization algorithms for Polynomial Linear Regression using the California Housing Prices dataset.

The main objective is to study how different optimization algorithms affect model training, convergence, and prediction performance. Momentum is also incorporated into the optimization methods.

## Dataset

- **Dataset:** California Housing Prices
- **Source:** [Kaggle – California Housing Prices](https://www.kaggle.com/datasets/camnugent/california-housing-prices)
- **Number of records:** 20,640
- **Target variable:** `median_house_value`
- **Input features:** 8 numerical features
- **Polynomial degree:** 2

## Data Preprocessing

The following preprocessing steps were applied:

1. Checked and handled missing values using the median.
2. Selected numerical features and the target variable.
3. Split the dataset into 80% training and 20% testing.
4. Applied StandardScaler to the input features and target.
5. Generated Polynomial Features with degree 2.
6. Scaled the polynomial features while keeping the bias column unchanged.

## Optimization Algorithms

Five optimization algorithms were implemented and evaluated:

1. **Gradient Descent (GD) with Momentum**
2. **Stochastic Gradient Descent (SGD) with Momentum**
3. **Mini-Batch Gradient Descent with Momentum**
4. **RMSProp with Momentum**
5. **Adam with Momentum**

The algorithms were implemented using NumPy to study their weight updates and optimization behavior.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Kaggle Notebooks

## Evaluation Metrics

The models were evaluated using:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score

## Results Comparison

| Optimizer | MSE | RMSE | MAE | R² |
|---|---:|---:|---:|---:|
| GD with Momentum | 4.925B | 70,181.65 | 51,138.37 | 0.6241 |
| SGD with Momentum | 4.449B | 66,699.25 | 47,678.51 | 0.6605 |
| Mini-Batch GD with Momentum | 4.378B | 66,165.04 | 47,321.84 | 0.6659 |
| RMSProp with Momentum | 4.438B | 66,616.14 | 47,843.00 | 0.6613 |
| Adam with Momentum | 4.368B | 66,091.06 | 46,812.38 | 0.6667 |

## Conclusion

Based on the experimental results, Adam with Momentum achieved the best overall performance among the five optimizers, obtaining the highest R² score and the lowest MSE, RMSE, and MAE.

Mini-Batch Gradient Descent achieved very similar performance. The results demonstrate how different optimization algorithms can affect model convergence and predictive performance.

## Repository Structure

- `01_GD_Polynomial_Regression.ipynb`
- `02_SGD_Polynomial_Regression.ipynb`
- `03_Mini_Batch_GD_Polynomial_Regression.ipynb`
- `04_RMSProp_Polynomial_Regression.ipynb`
- `05_Adam_Polynomial_Regression.ipynb`
- `README.md`

## Author

Machine Learning Course Project.
