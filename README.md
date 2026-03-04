# Machine Learning Models for Predicting Mechanical Properties of Gypsum-Based Composites

This repository presents a comprehensive machine learning framework for predicting:

- **Compressive Strength (MPa)**
- **Flexural Strength (MPa)**

of gypsum-based composite materials reinforced with wheat straw and chemical additives.

The study evaluates and compares five advanced regression algorithms:

- Artificial Neural Network (ANN)
- Gaussian Process Regression (GPR)
- Random Forest (RF)
- Extreme Gradient Boosting (XGBoost)
- Support Vector Machine (SVM)

---

## Input Features

The following material parameters are used as model inputs:

1. Gypsum Strength  
2. Gypsum Quantity  
3. Water Quantity  
4. Water-to-Gypsum Ratio  
5. Wheat Straw Content  
6. Calcium Chloride (CaCl₂)  
7. Calcium Hydroxide (Ca(OH)₂)

---

## Target Variables

- Compressive Strength (MPa)
- Flexural Strength (MPa)

Missing values were removed before training.

---

## Machine Learning Models

### Artificial Neural Network (ANN)
- Fully connected feedforward network
- Non-linear activation functions
- Optimized via backpropagation

### Gaussian Process Regression (GPR)
- RBF kernel
- Probabilistic regression
- Provides uncertainty estimation

### Random Forest (RF)
- Ensemble of decision trees
- Bagging-based
- Robust to overfitting

### XGBoost
- Gradient boosting framework
- Regularized boosting
- High predictive performance

### Support Vector Machine (SVM)
- SVR with RBF kernel
- Standardized input features
- Effective in high-dimensional spaces

---

## Model Evaluation Metrics

Each model is evaluated using:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Coefficient of Determination (R²)

An 80/20 train-test split is used with fixed random seed for reproducibility.

---

## Visualizations Included

- Learning Curves (R² vs Training Size)
- Actual vs Predicted Plots
- ±10% and ±20% Error Bands
- Prediction Error Distribution
- Permutation Feature Importance

---

## 📁 Project Structure
