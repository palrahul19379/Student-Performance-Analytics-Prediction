# Student Performance Analytics & Prediction

##  Project Overview

This project analyzes student academic data using Python and explores the relationship between study hours, attendance, and academic performance.

The project demonstrates a complete data analysis and machine learning workflow, including data cleaning, exploratory data analysis, visualization, feature analysis, train-test splitting, linear regression, and model evaluation.

## Objectives

* Analyze student academic performance data.
* Identify patterns and relationships between study hours, attendance, and marks.
* Perform data cleaning and missing-value handling.
* Conduct exploratory data analysis using visualizations.
* Apply Linear Regression as a machine learning experiment.
* Evaluate model performance using MAE, MSE, RMSE, and R² Score.

## Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**

##  Dataset

The dataset contains student-related information including:

| Feature    | Description                   |
| ---------- | ----------------------------- |
| ID         | Unique student identifier     |
| Name       | Student name                  |
| StudyHours | Student study hours           |
| Attendance | Student attendance percentage |
| Marks      | Student academic marks        |

The `ID` and `Name` columns were excluded from the modeling stage because they are not meaningful predictive features.

## Data Analysis

The project includes:

* Dataset structure and statistical analysis
* Missing-value analysis
* Duplicate-value checking
* Data cleaning
* Study Hours vs Marks analysis
* Attendance vs Marks analysis
* Marks distribution analysis
* Correlation analysis
* Feature selection

##  Machine Learning Experiment

A **Linear Regression** model was trained using:

**Input Features**

* StudyHours
* Attendance

**Target**

* Marks

The dataset was divided into training and testing sets using an **80:20 split**.

##  Model Evaluation

The Linear Regression model produced the following results on the test data:

| Metric   |   Score |
| -------- | ------: |
| MAE      |   14.45 |
| MSE      |  281.02 |
| RMSE     |   16.76 |
| R² Score | -0.0025 |

The results indicate that the available features have limited linear predictive power for the target variable in this dataset.

##  Key Finding

The correlation analysis showed very weak relationships between the available features and student marks:

* StudyHours → Marks: approximately **0.02**
* Attendance → Marks: approximately **0.03**

Therefore, the Linear Regression model demonstrated limited predictive performance.

Rather than artificially improving the model results, this project documents the limitation of the available dataset and demonstrates the importance of evaluating data quality and feature relationships before selecting a machine learning model.

##  Project Structure

```text
Student-Performance-Analytics-Prediction/
│
├── Student Performance Analytics & Prediction.ipynb
├── student_dataset_v2 (1).csv
└── README.md
```

## ▶️ How to Run

1. Clone or download this repository.
2. Open the Jupyter Notebook.
3. Make sure the CSV dataset is in the same directory as the notebook.
4. Install the required Python libraries.
5. Run the notebook cells sequentially.

### Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Author

Rahul Pal

B.Tech CSE (AI/ML)
Maharana Institute of Professional Studies, Kanpur
