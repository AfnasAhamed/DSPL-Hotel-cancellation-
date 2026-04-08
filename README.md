# Hotel Chain A — Booking Cancellation Prediction
**University of Westminster | 5DATA004C Data Science Project Lifecycle**
**Client: Hotel Chain A (OCTAVE — John Keells Group, Sri Lanka)**

## Project Overview
This project analyses hotel booking cancellation and no-show patterns
for Hotel Chain A, delivering EDA, revenue loss analysis, predictive
modelling, and client recommendations.

## Project Structure
```
data/raw/           — Original datasets provided by client
data/processed/     — Cleaned and feature engineered datasets
notebooks/          — Jupyter notebooks for each project phase
src/                — Reusable Python modules
artifacts/models/   — Saved trained models
artifacts/plots/    — Saved visualisations
artifacts/results/  — Saved metrics and evaluation outputs
reports/            — Final report and figures
```

## Notebooks
| Notebook | Description |
|---|---|
| 01_eda_preliminary | Data loading, cleaning, quality checks |
| 02_eda_univariate | Univariate analysis |
| 03_eda_multivariate | Multivariate analysis, PCA, pairplot |
| 04_feature_engineering | Derived features, encoding |
| 05_preprocessing | Final preprocessing pipeline |
| 06_modelling_random_forest | RF baseline, SMOTE, tuning |
| 07_modelling_xgboost | XGB baseline, SMOTE, tuning |
| 08_modelling_neural_network | MLP neural network |
| 09_model_comparison | Final model comparison |

## Models Used
- Random Forest Classifier
- XGBoost Classifier
- Multi-Layer Perceptron (Neural Network)

## Experiment Tracking
MLflow is used to track all model experiments.
Run `mlflow ui` to view the dashboard at http://127.0.0.1:5000

## Team
- Afnas Ahamed — Chief Data Scientist
- Haritha Sugathadasa — Chief Business Analyst
- Adeeb Shiham — Project Manager
- Rashmi Tharuka — Chief Data Engineer
- Maneth Premarathne — Chief Researcher
```

---

## Step 5 — Update .gitignore

Open your `.gitignore` and make sure it has these so you don't push data files or model binaries to GitHub:
```
# Data files
data/raw/
data/processed/

# Python
__pycache__/
*.pyc
*.pyo
.ipynb_checkpoints/
venv/

# MLflow
mlflow.db
mlruns/

# Environment
.env
*.env

# Models
artifacts/models/*.pkl
artifacts/models/*.joblib
