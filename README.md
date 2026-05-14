# Titanic-Survival-Prediction-Task03
# Titanic Survival Prediction using Machine Learning

## Project Overview
This project focuses on predicting passenger survival on the Titanic using Machine Learning classification algorithms. The objective is to analyze passenger information and determine whether a passenger survived or not based on different attributes such as passenger class, gender, age, fare, family size, and title.

## Dataset
Dataset used:
https://www.kaggle.com/datasets/bhanupratapbiswas/titanic-survival-datasets

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

## Feature Engineering
The following feature engineering techniques were performed:
- Extracted passenger titles
- Created Family Size feature
- Cabin Presence analysis
- Encoded categorical variables
- Handled missing values

## Missing Value Handling
Missing values were handled using:
- Median imputation for Age
- Mode imputation for categorical columns
- Cabin presence feature creation

## Machine Learning Models
The following classification algorithms were trained and compared:
- Logistic Regression
- Random Forest Classifier

## Model Explainability
Feature importance analysis was performed using Random Forest feature importance to understand which features contributed most to survival prediction.

## Evaluation Metrics
Models were evaluated using:
- Accuracy Score
- Confusion Matrix
- Precision
- Recall
- F1-Score

## Best Model
Random Forest Classifier achieved the best performance for survival prediction.

## Saved Model
The trained model is saved as:

```text
titanic_model.pkl
```

## Example Inference Code

```python
import joblib

# Load model
model = joblib.load("titanic_model.pkl")

# Example prediction
sample = [[3, 1, 22, 1, 0, 7.25, 2, 1, 0]]

prediction = model.predict(sample)

print("Survival Prediction:", prediction)
```

## Project Files

```text
Titanic_Project/
│
├── Titanic-Dataset.csv
├── titanic_survival_prediction.ipynb
├── titanic_survival_prediction.html
├── titanic_model.pkl
├── README.md
├── screenshots/

## Author
Sharanya N
