# Student Pass/Fail Prediction Using Machine Learning Pipeline

## Project Overview
This project builds a complete **Machine Learning Pipeline** to predict whether a student will **Pass** or **Fail** based on academic performance data.

Target Variable:
- **1 = Pass**
- **0 = Fail**

This is a **Binary Classification Problem**.

---

## Dataset Features

The dataset contains the following columns:

- Student_ID
- Student_Name
- Study_Hours_Per_Day
- Attendance_%
- Previous_GPA
- Assignments_Submitted
- Sleep_Hours
- Final_Marks (Target Variable)

---

## Project Objectives

This project includes:

- Exploratory Data Analysis (EDA)
- Missing Value Handling
- Duplicate Removal
- Data Type Fixing
- Feature Engineering
- Feature Transformation
- Feature Scaling
- Column Transformer
- Machine Learning Pipeline
- Model Evaluation
- Model Saving
- Prediction Function

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Joblib

---

# Project Workflow

## 1. Data Loading
Load dataset using Pandas.

```python
df = pd.read_csv("studentbinaryclass.csv")
```

---

## 2. Exploratory Data Analysis (EDA)

Performed:

- Dataset shape
- Column analysis
- Data types
- Missing values
- Duplicate values
- Statistical summary
- Target variable distribution
- Correlation heatmap

---

## 3. Data Cleaning

Removed unnecessary columns:

- Unnamed: 0
- Student_ID
- Student_Name

Converted columns into numeric format:

- Assignments_Submitted
- Sleep_Hours

---

## 4. Feature Engineering

Separated:

- Features (X)
- Target (y)

---

## 5. Preprocessing Pipeline

### Numerical Pipeline
- Missing value handling
- Power transformation
- Standard scaling

### Categorical Pipeline
- Missing value handling
- One-hot encoding

---

## 6. Column Transformer

Used to combine numerical and categorical pipelines.

```python
ColumnTransformer()
```

---

## 7. Machine Learning Models

The following models were trained:

- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)

---

## 8. Model Evaluation

Evaluation metrics used:

- Accuracy Score
- Classification Report
- Confusion Matrix

---

## 9. Best Model Selection

The model with highest accuracy was selected as final model.

---

## 10. Model Saving

```python
joblib.dump(best_model, "student_pass_fail_pipeline.pkl")
```

---

## 11. Prediction Function

A user input function was created where users enter:

- Study Hours
- Attendance
- Previous GPA
- Assignments Submitted
- Sleep Hours

The system predicts:

- Pass ✅
- Fail ❌

---

# Project Structure

```bash
student-project/
│
├── studentbinaryclass.csv
├── student_pipeline.ipynb
├── student_pass_fail_pipeline.pkl
├── README.md
```

---

# Example Prediction

### Input:
- Study Hours: 6
- Attendance: 85
- Previous GPA: 3.5
- Assignments Submitted: 9
- Sleep Hours: 7

### Output:
Student will PASS ✅

---

# Conclusion

This project successfully demonstrates an end-to-end Machine Learning Pipeline for predicting student pass/fail performance.

It includes:

✔ EDA  
✔ Data Cleaning  
✔ Feature Engineering  
✔ Preprocessing  
✔ Pipeline Building  
✔ Model Training  
✔ Evaluation  
✔ Model Saving  
✔ Prediction System  

This project can be further improved by deploying it using Flask, Streamlit, or Django.
