# Titanic Survival Prediction using Logistic Regression

## Overview
This project explores the Titanic dataset to predict passenger survival using Logistic Regression.  
It goes beyond a basic model by visualizing prediction correctness and analyzing patterns in model errors.  

The goal was to:
- Build a baseline Logistic Regression model.
- Evaluate its performance with metrics and visualizations.
- Explore patterns in **where** the model succeeds and fails.

---

## Key Results
- **Test Accuracy:** 83.5%
- **Strengths:** The model performs well at predicting non-survivors.
- **Weaknesses:** Struggles with predicting survivors — opportunity for feature engineering.

---

## Visuals
### **1. Correct vs Incorrect Predictions**
Side-by-side scatterplots show:
- **Left:** Actual survival by Age & Gender.
- **Right:** Model correctness (green = correct, red = incorrect).


### **2. Confusion Matrix**
A heatmap to understand classification performance at a glance.

---

## Methods
1. **Data Cleaning**  
   - Handled missing Age values using median imputation.
   - Encoded categorical variables (Sex).

2. **Feature Selection**  
   - Used core features: `Age`, `Fare`, `Sex`, `SibSp`, `Pclass`.  

3. **Modeling**  
   - Trained a Logistic Regression classifier using scikit-learn.  
   - Split data into 70/30 train-test sets for evaluation.  

4. **Evaluation**  
   - Metrics: Accuracy, Confusion Matrix, Classification Report.  
   - Visualizations: Side-by-side scatterplots of predictions vs correctness.

---

## Next Steps
- **Feature Engineering:** Add `FamilySize`, `Title`, and `IsAlone`.  
- **Model Comparison:** Test Random Forest and Gradient Boosting for improved performance.  
- **Hyperparameter Tuning:** Use GridSearchCV for logistic regression and ensemble methods.

---

## Dataset
The dataset comes from the [Titanic Dataset](https://www.kaggle.com/datasets/heptapod/titanic)

---

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/peytonrivers/Titanic-Logistic-Regression.git

