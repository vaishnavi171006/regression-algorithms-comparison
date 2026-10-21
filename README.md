# regression-algorithms-comparison
Comparison of Linear, Polynomial, Decision Tree, Random Forest, and Support Vector Regression algorithms using Python and Scikit-learn.
# Comparison of Different Regression Algorithms for Predictive Modeling

## 📌 Project Overview
This project compares five regression algorithms using Python and Scikit-learn to identify suitable models for predicting continuous values. The algorithms are evaluated on the California Housing dataset using standard regression metrics.

## 🎯 Aim
To compare the performance of different regression algorithms on a given dataset and identify the most suitable algorithm for accurate prediction.

## 🎯 Objectives
- Understand the working principles of different regression algorithms.
- Apply multiple regression models to the same dataset.
- Evaluate model performance using appropriate error metrics.
- Compare prediction accuracy and model performance.
- Identify a suitable regression algorithm based on experimental results.

## 🛠️ Technologies Used
- Python
- Jupyter Notebook
- NumPy
- Pandas
- Scikit-learn

## 📂 Project Structure

```text
regression-algorithms-comparison/
│
├── regression_comparison.ipynb
└── README.md
```

## 📊 Dataset
This project uses the California Housing dataset available through Scikit-learn.

The dataset contains information about housing districts in California, including median income, house age, average rooms, population, and other features.

**Target variable:** Median house value, represented in units of $100,000 in the original dataset.

The dataset is suitable for comparing regression models on a real-world prediction task.

## 📚 Theory

### 1. Linear Regression
Linear Regression models the relationship between input features and a continuous target using a linear equation.

**Use case:** Predicting house prices based on housing characteristics.

**Limitation:** May not capture complex nonlinear relationships.

### 2. Polynomial Regression
Polynomial Regression extends Linear Regression by adding polynomial combinations of input features.

**Use case:** Modeling nonlinear relationships.

**Limitation:** Higher polynomial degrees can cause overfitting and increase computational cost.

### 3. Decision Tree Regression
Decision Tree Regression divides the dataset into smaller regions using feature-based rules and predicts a continuous value for each region.

**Use case:** Predicting house prices when relationships between features and prices are complex.

**Limitation:** A deep tree can overfit the training data.

### 4. Random Forest Regression
Random Forest Regression combines multiple decision trees and averages their predictions to improve stability and predictive performance.

**Use case:** Predicting house prices from multiple interacting features.

**Limitation:** Requires more computational resources and is less interpretable than a simple linear model.

### 5. Support Vector Regression (SVR)
Support Vector Regression fits a function that attempts to keep prediction errors within a specified margin while balancing model complexity.

**Use case:** Predicting continuous values from scaled numerical features.

**Limitation:** Sensitive to feature scaling and parameter selection.

## ⚙️ Implementation Steps
1. Import the required libraries.
2. Load the California Housing dataset.
3. Separate input features and target values.
4. Split the dataset into training and testing sets.
5. Scale features and the target for SVR.
6. Generate polynomial features for Polynomial Regression.
7. Initialize all five regression models.
8. Train each model on the training dataset.
9. Predict target values for the test dataset.
10. Evaluate predictions using MAE, MSE, and R² score.
11. Compare the performance of all models.

## 🚀 How to Run the Project
1. Install Python and Jupyter Notebook.
2. Install the required libraries if they are not already installed:

   ```bash
   pip install numpy pandas scikit-learn jupyter
   ```

3. Open Jupyter Notebook.
4. Open `regression_comparison.ipynb`.
5. Run all notebook cells sequentially.
6. Observe the performance comparison table.

**Note:** An internet connection may be required the first time Scikit-learn downloads the California Housing dataset.

## 📈 Model Evaluation Metrics

### Mean Absolute Error (MAE)
Measures the average absolute difference between actual and predicted values. Lower MAE indicates better predictions.

### Mean Squared Error (MSE)
Measures the average squared prediction error. Lower MSE indicates smaller errors, with larger errors penalized more heavily.

### R² Score
Measures how well the model explains the variation in the target variable. A score closer to 1 generally indicates a better fit.

## 📋 Algorithms Compared

| Algorithm | Main Characteristic |
|---|---|
| Linear Regression | Models linear relationships |
| Polynomial Regression | Models nonlinear relationships using polynomial features |
| Decision Tree Regression | Learns rule-based feature splits |
| Random Forest Regression | Combines predictions from multiple decision trees |
| Support Vector Regression | Fits a function within an error margin |

## 📊 Expected Output
The notebook displays a comparison table containing:

- MAE for each algorithm.
- MSE for each algorithm.
- R² score for each algorithm.

The model with the lowest MAE and MSE and a strong R² score may be considered more suitable for this dataset, provided the evaluation results are comparable.

## 📚 Learning Outcomes
- Understand different regression algorithms.
- Train multiple models on the same dataset.
- Learn polynomial feature transformation.
- Understand feature scaling for SVR.
- Evaluate regression models using MAE, MSE, and R².
- Compare model performance and select an appropriate model based on experimental results.
