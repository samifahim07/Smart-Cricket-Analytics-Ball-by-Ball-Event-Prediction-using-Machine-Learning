# IPL Boundary Prediction Using Machine Learning

## Overview

Cricket has become increasingly data-driven, with teams and analysts relying on match statistics to better understand player performance and game situations. This project explores how machine learning can be used to predict whether a delivery will result in a boundary (4 or 6) based on the context of the match and player performance.

The project follows a complete machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, model training, hyperparameter tuning, model comparison, and explainability using SHAP. The goal was to build a reliable prediction model while understanding the factors that influence boundary scoring.

---

## Dataset

The dataset consists of ball-by-ball cricket data along with batting, bowling, and match-related information. It provides the necessary context to train machine learning models for predicting boundary outcomes.

---

## Project Workflow

The project includes the following stages:

* Data loading and inspection
* Data cleaning and preprocessing
* Exploratory Data Analysis (EDA)
* Feature engineering
* Feature encoding
* Handling class imbalance using SMOTE
* Training multiple machine learning models
* Hyperparameter tuning
* Model evaluation and comparison
* Model interpretation using SHAP
* Saving the best-performing model

---

## Feature Engineering

To improve prediction performance, several cricket-specific features were created, including:

* Current Score
* Current Run Rate
* Batter Strike Rate
* Bowler Economy Rate
* Boundary Rate
* Dot Ball Rate
* Rolling Runs
* Rolling Wickets
* Batter Form
* Bowler Form
* Over Phase

These features capture the state of the match more effectively than the raw data alone and help the models learn meaningful patterns.

---

## Models Used

The following machine learning algorithms were trained and evaluated:

* Random Forest
* Extra Trees
* XGBoost
* CatBoost
* HistGradientBoosting
* LightGBM

Each model was evaluated before and after hyperparameter tuning to determine the best-performing approach.

---

## Evaluation Metrics

Model performance was measured using:

* Accuracy
* Precision
* Recall
* F1 Score

The results from all models were compared to identify the most reliable model for boundary prediction.

---

## Model Explainability

SHAP (SHapley Additive exPlanations) was used to interpret the predictions of the final model. This made it possible to identify which features had the greatest influence on predicting whether a ball would result in a boundary.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* CatBoost
* LightGBM
* SHAP
* Imbalanced-learn

---

## Project Structure

```text
Cricket-Boundary-Prediction/
│
├── smart_analysis.ipynb
├── best_model.pkl
├── README.md
└── requirements.txt
└── dataset/
```

---

## Results

Multiple machine learning models were trained and compared after applying feature engineering and hyperparameter tuning. The final model demonstrated strong predictive performance while maintaining interpretability through SHAP, providing useful insights into the key factors associated with boundary scoring.

---

## Future Improvements

Possible future improvements include:

* Using a larger and more diverse dataset
* Adding more player and match-level statistics
* Developing a web application using Flask or Streamlit
* Deploying the model for real-time predictions

---

