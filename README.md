# Titanic Survival Prediction

## Overview

This project predicts passenger survival on the Titanic using machine learning techniques. The workflow includes data preprocessing, feature engineering, model training, hyperparameter tuning, model comparison, and evaluation.

The project compares Logistic Regression and Random Forest Classifier models and selects the better-performing model based on test set accuracy and classification metrics.

---

## Dataset

The dataset was loaded using Seaborn's built-in Titanic dataset:

```python
import seaborn as sns
titanic = sns.load_dataset('titanic')
```

Target Variable:

* `survived`

  * 0 = Did Not Survive
  * 1 = Survived

---

## Machine Learning Workflow

### Data Preprocessing

Numerical Features:

* Missing value imputation using median values
* Feature scaling using StandardScaler

Categorical Features:

* Missing value imputation using most frequent category
* One-Hot Encoding

### Pipeline Construction

Implemented Scikit-Learn:

* Pipeline
* ColumnTransformer

to automate preprocessing and model training.

### Models Trained

#### Logistic Regression

* Trained using preprocessing pipeline
* Evaluated using classification metrics
* Confusion Matrix generated
* Feature importance analyzed using coefficients

#### Random Forest Classifier

* Hyperparameter tuning using GridSearchCV
* Stratified K-Fold Cross Validation
* Feature importance analysis
* Confusion Matrix generated

### Hyperparameter Tuning

GridSearchCV was used to optimize Random Forest parameters such as:

* Number of Trees
* Maximum Tree Depth
* Minimum Samples Split

### Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

## Key Concepts Demonstrated

* Data Cleaning
* Missing Value Imputation
* Feature Scaling
* One-Hot Encoding
* Machine Learning Pipelines
* Column Transformers
* Logistic Regression
* Random Forest Classifier
* Cross Validation
* Hyperparameter Tuning
* Model Evaluation
* Feature Importance Analysis

---

## Results

Both Logistic Regression and Random Forest models were trained and evaluated.

The final model was selected based on test set performance and classification metrics.

Important predictive features were analyzed to better understand the factors influencing passenger survival.

---

## Author

Roselyn Miriam Sunil

