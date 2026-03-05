## Machine Learning Models for Predicting Mechanical Properties of Gypsum-Based Composites

## This repository presents a comprehensive machine learning framework for predicting:

Compressive Strength (MPa)

Flexural Strength (MPa)

of gypsum-based composite materials reinforced with wheat straw and chemical additives.

## The study evaluates and compares five advanced regression algorithms:

Artificial Neural Network (ANN)

Gaussian Process Regression (GPR)

Random Forest (RF)

Extreme Gradient Boosting (XGBoost)

Support Vector Machine (SVM)


## INPUT FEATURES

The following material parameters are used as model inputs:

Gypsum Strength

Gypsum Quantity

Water Quantity

Water-to-Gypsum Ratio

Wheat Straw Content

Calcium Chloride (CaCl2)

Calcium Hydroxide (Ca(OH)2)


## TARGET VARIABLES


Compressive Strength (MPa)

Flexural Strength (MPa)

Note:
Missing values must be removed before training. All variables must be numeric.

================================================================================
## MACHINE LEARNING MODELS
================================================================================

Artificial Neural Network (ANN)
===============================
Fully connected feedforward network

Non-linear activation functions

Optimized via backpropagation


Gaussian Process Regression (GPR)
=================================
RBF kernel

Probabilistic regression

Provides uncertainty estimation

Random Forest (RF)
=================================
Ensemble of decision trees

Bagging-based approach

Robust to overfitting

XGBoost
================================
Gradient boosting framework

Regularized boosting

High predictive performance

Support Vector Machine (SVM)
========================================
Support Vector Regression (SVR) with RBF kernel

Standardized input features

Effective in high-dimensional spaces

MODEL EVALUATION METRICS
===============================================
Each model is evaluated using:

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Mean Absolute Error (MAE)

Coefficient of Determination (R2)

An 80/20 train-test split is used with a fixed random seed for reproducibility.


VISUALIZATIONS GENERATED
===============================================

The Python script produces:

Learning Curves (R2 vs Training Size)

Actual vs Predicted plots

±10% and ±20% error bands

Prediction error distribution plots

Permutation feature importance plots


## HOW TO USE THE PYTHON FILE


Follow the steps below to run the project properly.

STEP 1: PREPARE YOUR DATA
-------------------------
Place your raw dataset file named:

data.csv in the SAME directory as the Python script.

Required Format of data.csv

The CSV file must contain the following column names EXACTLY as written:


Input Columns:
===============================================

Gypsum Strength

Gypsum Quantity

Water Quantity

Water-to-Gypsum Ratio

Wheat Straw Content

Calcium Chloride

Calcium Hydroxide


Output Columns:
===============================================

Compressive Strength

Flexural Strength

Important:

No missing values

No extra spaces in column names

All values must be numeric

File must be saved as CSV format

STEP 2: INSTALL REQUIRED LIBRARIES
----------------------------------
Before running the script, install the required Python libraries:

pip install numpy pandas matplotlib scikit-learn xgboost scipy

STEP 3: CHECK DATA LOADING IN SCRIPT
------------------------------------
Inside the Python file, make sure the dataset is loaded as:

df = pd.read_csv("data.csv")

If your file is in another folder, update the path accordingly.

STEP 4: RUN THE SCRIPT
----------------------
Open Command Prompt or Terminal in the project folder and run:

python your_script_name.py

Example:

python ANN_compressive_strength.py

STEP 5: OUTPUT RESULTS
----------------------
After execution, the script will:

Print model performance metrics in the console

Display evaluation plots

Show feature importance ranking

Compare the prediction performance of all models


Same preprocessing applied to all models. Note: GPR code also includes the SHAP analysis code.

Consistent evaluation metrics across models

End of README File
