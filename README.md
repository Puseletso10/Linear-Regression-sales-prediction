# Ice Cream Sales Prediction

## Project Overview
This project uses **Linear Regression** to predict ice cream sales revenue based on temperature data.  
The notebook demonstrates a complete beginner-friendly machine learning workflow, including:

- Importing and exploring data
- Data cleaning
- Data visualization
- Building a Linear Regression model
- Evaluating model performance
- Making predictions
- Saving and loading the trained model

The project was implemented in Python using libraries such as Pandas, NumPy, Matplotlib, and Scikit-learn.

---

## Dataset
The dataset contains 500 rows and two main variables:

| Variable | Description |
|---|---|
| temperature | Temperature values |
| revenue | Ice cream sales revenue |

The dataset is loaded from:

```python
IceCreamData.csv
```

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Pickle

---

## Project Workflow

### 1. Importing Libraries
The notebook begins by importing the required Python libraries for data analysis, visualization, and machine learning.

### 2. Loading the Dataset
The dataset is loaded into a Pandas DataFrame using:

```python
pd.read_csv()
```

### 3. Data Exploration
Several exploratory analysis steps are performed:

- Checking dataset shape
- Viewing dataset information
- Generating descriptive statistics

### 4. Data Cleaning
An outlier row where revenue equals 1 is removed from the dataset to improve model performance.

### 5. Data Visualization
A scatter plot is created to visualize the relationship between:

- Temperature (independent variable)
- Revenue (dependent variable)

The visualization shows a strong positive linear relationship.

### 6. Building the Model
A **Linear Regression** model is trained using Scikit-learn.

```python
LinearRegression()
```

### 7. Model Evaluation
The notebook evaluates the model using:

- Mean Squared Error (MSE)
- Residual Sum of Squares (RSS)
- R-squared Score

The model achieved approximately:

```text
R² = 0.979
```

This indicates that the model explains about 97.9% of the variation in revenue.

### 8. Saving and Loading the Model
The trained model is saved using the Pickle library and later restored for future predictions.

---

### 9. Model Prediction
The trained model predicts ice cream revenue based on temperature values.

Example prediction:

```python
today_temp = 25
```

Predicted revenue:

```python
revenue_predict = lm.predict(today_temp)
```

---

## Key Learning Outcomes

This project demonstrates:

- Data preprocessing
- Exploratory Data Analysis (EDA)
- Regression modeling
- Data visualization
- Model persistence using Pickle
- Basic machine learning workflow in Python

---

## How to Run the Project

1. Clone the repository
2. Install required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn
```

3. Open the notebook:

```bash
jupyter notebook
```

4. Run all notebook cells

---

## Future Improvements

Possible improvements include:

- Adding multiple features
- Using larger datasets
- Comparing different regression models
- Deploying the model as a web application

---

## Author

Prepared by Puseletso Motsoari
