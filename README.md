# Customer Churn Prediction — Phase 1

A leakage-aware machine-learning workflow for the Telco Customer Churn dataset.

## Setup

```bash
python -m venv .venv
# Windows:
.venv\\Scripts\\activate
# macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt
```

Place `WA_Fn-UseC_-Telco-Customer-Churn.csv` inside `data/`, then launch:

```bash
jupyter notebook
```

Open `notebooks/customer_churn_analysis_phase1.ipynb` and run all cells.

## Key improvements

- Stratified train/test split before fitting.
- `ColumnTransformer` with numeric imputation/scaling and categorical one-hot encoding.
- SMOTE inside an imbalanced-learn pipeline, so resampling occurs independently within each CV training fold.
- Logistic Regression baseline plus Decision Tree, Random Forest and optional XGBoost.
- Randomized hyperparameter search selected by average precision.
- Held-out test evaluation: precision, recall, F1, ROC-AUC, PR-AUC and confusion matrix.
- Model-agnostic permutation importance.
- Complete fitted pipeline saved with joblib; prediction accepts raw customer fields.

## Important

The dataset is not included. No performance results are claimed until the notebook is run with the dataset. SMOTE after one-hot encoding is a practical baseline; compare with SMOTENC and class weighting in follow-up experiments.
