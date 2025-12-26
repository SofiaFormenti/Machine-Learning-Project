<div align="center">
 
# Medical Cost prediction - Machine Learning project

<br/>

Kaggle Dataset: https://www.kaggle.com/datasets/mirichoi0218/insurance

**Number of observations:** 1,338  
**Number of features:** 6  
**Target variable:** `charges`

Each row represents one insurance beneficiary.
 </div>
<br/>
<br/>

📓 **Notebook visualization**  
Due to GitHub rendering limitations, interactive pipeline diagrams are best viewed via nbviewer:

👉 https://nbviewer.org/github/SofiaFormenti/Machine-Learning-Project/blob/main/Project.ipynb

<br/>
## Dataset Overview

| Column Name | Type | Description |
|------------|------|-------------|
| `age` | Numerical (int) | Age of the individual in years |
| `sex` | Categorical | Biological sex (`male`, `female`) |
| `bmi` | Numerical (float) | Body Mass Index (BMI), a measure of body fat |
| `children` | Numerical (int) | Number of dependent children covered by insurance |
| `smoker` | Categorical | Smoking status (`yes`, `no`) |
| `region` | Categorical | Residential area in the US (`northeast`, `northwest`, `southeast`, `southwest`) |
| `charges` | Numerical (float) | Medical insurance costs (target variable) |
<br/>

---
<br/>


- **Problem type:** Supervised learning  
- **Task:** Regression  
- **Objective:** Predict individual medical insurance charges based on demographic and lifestyle information.
<br/>

---

This project presents a **complete end-to-end regression workflow**, covering every step from data exploration to model optimization and evaluation. The focus is not only on building accurate models, but also on understanding their behavior and performance.

<br/>

## Components

### Exploratory Data Analysis (EDA)
- Visual exploration of the dataset using **histograms, density plots, correlation matrices, and scatter plots** to uncover patterns and relationships between variables.

### Data Preprocessing
- **Missing data imputation**  
  *(The original dataset is fully clean; controlled noise was intentionally introduced for practice.)*
- **Feature scaling** to ensure numerical stability and fair model comparisons.

### Train–Test Split
- Division of the dataset into training and testing sets to properly evaluate model generalization.

### Regression Pipeline
- Construction of a **modular and reusable regression pipeline** integrating preprocessing, dimensionality reduction, and model fitting.

### Model Evaluation
- Performance assessment using multiple error metrics:
  - **MAE**
  - **MSE**
  - **RMSE**
  - **R²**

### Hyperparameter Optimization
- **Dimensionality reduction techniques**:
  - Principal Component Analysis (PCA)
  - Linear Discriminant Analysis (LDA)
  - SelectKBest
- **Regression models explored**:
  - Linear Regression
  - Ridge Regression
  - Lasso Regression
  - Decision Tree Regressor
  - Random Forest Regressor
  - K-Nearest Neighbors Regressor
- Model comparison performed using **cross-validation**.

### Model Selection & Fine-Tuning
- Identification of the best-performing model across experiments.
- Further optimization of the top candidate — **Random Forest emerged as the strongest performer 🌳**.

### Learning & Validation Curves
- Visualization of learning and validation curves to analyze **bias, variance, and overfitting behavior**.

---

## onus: Neural Network Model

As an additional experiment, a **simple sequential neural network** was implemented using **TensorFlow**, providing a comparison between classical machine-learning models and a neural approach.



