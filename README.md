# Student Academic Success Prediction Using Random Forest

## Project Overview
This project aims to predict students' academic outcomes using Machine Learning techniques. It uses student-related data to classify academic performance into three categories:

- **Dropout**
- **Enrolled**
- **Graduate**

The main focus is on building and evaluating a Random Forest classification model and improving its performance through hyperparameter tuning.

## Dataset
- Number of records: **4,424**
- Number of features: **36**
- Target variable: **Target**
- Classes: Dropout, Enrolled, Graduate

## Project Workflow

The project is organized into five Jupyter Notebooks:

1. **Data Preparation & EDA** – Data cleaning, preprocessing, and exploratory data analysis.
2. **Random Forest Baseline** – Building and evaluating the initial Random Forest model.
3. **Random Forest Optimization** – Improving model performance using GridSearchCV.
4. **Feature Importance** – Identifying the most influential features.
5. **Model Evaluation** – Comparing models and evaluating the optimized model using different metrics.

## Machine Learning Models

The following models were trained and compared:

- Random Forest
- Optimized Random Forest
- Decision Tree
- Gradient Boosting

## Hyperparameter Optimization

GridSearchCV with Stratified 3-Fold Cross-Validation was used to find the best Random Forest parameters.

**Best Parameters:**

```python
{
    'n_estimators': 200,
    'max_depth': 20,
    'min_samples_split': 5
}
```

Best cross-validation Macro F1-Score: **0.6871**

## Model Performance

The models were evaluated using Accuracy, Precision, Recall, and Macro F1-Score.

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Random Forest | 0.7672 | 0.7214 | 0.6802 | 0.6916 |
| **Optimized Random Forest** | **0.7763** | **0.7371** | **0.6898** | **0.7026** |
| Decision Tree | 0.6972 | 0.6378 | 0.6397 | 0.6385 |
| Gradient Boosting | 0.7593 | 0.7073 | 0.6813 | 0.6902 |

The **Optimized Random Forest** achieved the highest Macro F1-Score and Accuracy among the evaluated models.

## Classification Results

The optimized model achieved the following F1-Scores for each class:

| Class | F1-Score |
|---|---:|
| Dropout | 0.78 |
| Enrolled | 0.47 |
| Graduate | 0.86 |

The Enrolled class was more challenging for the model to predict compared with the other two classes.

## ROC-AUC Evaluation

The optimized Random Forest model was also evaluated using One-vs-Rest ROC-AUC.

| Class | ROC-AUC |
|---|---:|
| Dropout | 0.9136 |
| Enrolled | 0.8224 |
| Graduate | 0.9298 |

## Feature Importance

The most influential features identified by the Random Forest model included:

1. Curricular units 2nd semester (approved)
2. Curricular units 2nd semester (grade)
3. Curricular units 1st semester (approved)
4. Curricular units 1st semester (grade)
5. Admission grade

These features highlight the importance of students' academic performance in predicting their educational outcomes.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Conclusion

The results show that the Optimized Random Forest model achieved the best overall performance among the tested models, with an Accuracy of **77.63%** and a Macro F1-Score of **70.26%**.

The project demonstrates how Machine Learning can be used to analyze student data and predict academic outcomes, potentially helping educational institutions identify students who may need additional support.
