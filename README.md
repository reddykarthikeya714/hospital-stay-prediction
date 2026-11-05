# Hospital Stay Duration Prediction

A machine-learning classification project that explores predicting a patient's **hospital-stay category** from structured hospital admission and patient-related data.

## Project at a glance

| Item | Details |
|---|---|
| Problem type | Multiclass classification |
| Domain | Healthcare analytics |
| Target | `Stay` (stay-duration category) |
| Models compared | Logistic Regression, Decision Tree, Random Forest |
| Evaluation | Accuracy, weighted F1-score, classification report, confusion matrix |

## Objective

Build a reproducible classification workflow to estimate the hospital-stay category represented in the dataset. The target is a set of duration ranges/categories, not an exact number of days.

This project is for learning and portfolio demonstration. It is not a clinical decision-support system.

## Data preparation and analysis

The notebook workflow includes:

- Excluding identifier columns such as `case_id` and `patientid` from model inputs.
- Exploring target-category counts and selected feature relationships.
- Removing duplicate rows.
- Imputing numeric missing values with the median.
- Imputing categorical missing values with the most frequent category.
- One-hot encoding categorical features.
- Scaling numeric features for Logistic Regression.
- Using a stratified 80/20 train-test split and a DummyClassifier baseline.

## Models and evaluation

The project compares:

1. Logistic Regression
2. Decision Tree
3. Random Forest

Models are compared using accuracy and weighted F1-score. The notebook also generates a classification report and confusion matrix to inspect class-level performance.

No numerical performance score is published here because a verified final result has not been recorded in this project summary.

## Tools and technologies

Python · Jupyter Notebook · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn

## Run locally

1. Clone this repository.
2. Open the notebook in Jupyter Notebook, JupyterLab, or Google Colab.
3. Install the required Python libraries.
4. Update the dataset path in the notebook. The original notebook contains a machine-specific Windows path; replace it with the path to your local CSV file.
5. Run the notebook cells in order.

## Limitations and responsible use

- The target represents stay-duration categories, not an exact length of stay.
- Class imbalance can affect model performance; inspect per-class precision, recall, and F1-score.
- A random row split may place records from the same patient in both training and test sets if repeated patient records exist. Patient-level splitting should be considered to reduce leakage risk.
- Coded dataset fields need clear definitions before meaningful interpretation.
- Predictions must not be used to make clinical or patient-care decisions.

## Future improvements

- Use patient-level validation where the data structure permits.
- Add a separate final hold-out evaluation.
- Investigate class imbalance and report per-class metrics.
- Document dataset field definitions and data provenance.
- Make data paths configurable rather than machine-specific.

---

*Portfolio project | Data Science · Machine Learning · Healthcare Analytics*
