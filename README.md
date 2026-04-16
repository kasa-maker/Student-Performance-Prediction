# Student Performance Prediction 🎓📈

## Overview
This project applies a **Linear Regression** machine learning model to predict a student's `Performance Index` based on their academic and lifestyle habits. It demonstrates an end-to-end machine learning workflow, including data preprocessing, model training, and performance evaluation.

## Author
**Kasaam Ali**

## Dataset
The dataset used is `student_performance.csv`, which contains the following features:
* `Hours Studied`: Number of hours a student studies.
* `Previous Scores`: The student's previous academic scores.
* `Extracurricular Activities`: Participation in extracurriculars (Yes/No).
* `Sleep Hours`: Average daily hours of sleep.
* `Sample Question Papers Practiced`: Number of practice papers solved.
* `Performance Index` **(Target Variable)**: The final predicted score of the student.

## Technologies Used
* **Python**
* **Pandas** (Data manipulation and preprocessing)
* **Scikit-Learn** (Model building and metrics)
* **Jupyter Notebook** (Development environment)

## Project Workflow
1. **Data Loading & Exploration:** Imported the dataset using Pandas to understand the data structure.
2. **Data Preprocessing:** * Removed duplicate records to ensure data quality.
   * Converted categorical data (`Extracurricular Activities`: 'Yes'/'No') into a numerical format (`1`/`0`) so the math model could process it.
3. **Train-Test Split:** Divided the data into a 70% training set and a 30% testing set.
4. **Model Training:** Trained a Multiple Linear Regression model on the training data.
5. **Evaluation:** Tested the model's accuracy on unseen data and calculated the error margins.

## Results & Performance
The model performed exceptionally well and generalized perfectly without overfitting:
* **R-squared (R^2) Score:** `0.988` (approx. 98.8% variance explained)
* **Training Mean Squared Error (MSE):** `4.11`
* **Testing Mean Squared Error (MSE):** `4.32`

The proximity of the Training and Testing MSE indicates a highly robust model.

## How to Run
1. Clone this repository to your local machine.
2. Ensure you have Python and Jupyter Notebook installed.
3. Install the required libraries by running: `pip install pandas scikit-learn`
4. Open the `Student_Performance.ipynb` file in Jupyter Notebook and run the cells.
