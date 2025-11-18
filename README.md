#  Iris Flower Species Classification with Decision Trees

##  Project Overview

This project implements a complete data mining and predictive modeling workflow on the **Iris Flower Dataset**. The primary goal is to build a classification model to accurately predict the species of an iris flower (**Setosa**, **Versicolor**, or **Virginica**) based on its sepal and petal measurements.

The assignment was completed as a requirement for the **Data Mining and Data Warehouse** course.

**Key Technologies Used:** Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn.

---

## 📊 Key Results

The model, a **Decision Tree Classifier**, was trained and evaluated on a held-out test set, demonstrating strong predictive performance.

### 1. Model Performance

| Metric | Value |
| :--- | :--- |
| **Test Accuracy** | **89.5%** |

### 2. Feature Importance

The analysis confirmed that **petal-related features** are the most critical for species differentiation.

| Feature | Importance Value |
| :--- | :--- |
| **Petal Length (cm)** | **0.92** |
| Petal Width (cm) | 0.05 |
| Sepal Width (cm) | 0.02 |
| Sepal Length (cm) | 0.01 |

### 3. Confusion Matrix

The confusion matrix shows the distribution of actual vs. predicted classes on the test data. The model achieved perfect classification for the *Setosa* species.

| Actual / Predicted | Setosa | Versicolor | Virginica |
| :---: | :---: | :---: | :---: |
| **Setosa (Actual)** | 12 | 0 | 0 |
| **Versicolor (Actual)** | 0 | 12 | 1 |
| **Virginica (Actual)** | 0 | 3 | 10 |

---

##  Key Visualizations

The following visualizations were key to understanding the data patterns and the model's logic.

### 1. Decision Tree Diagram

This plot shows the rules the model learned to classify the species. Each node represents a condition (e.g., `Petal Length <= 2.45`) used to split the data.



[Image of Decision Tree Classification Diagram]


### 2. Exploratory Data Analysis (EDA)

The scatter plot highlights the clear separation between the three species, especially when comparing Petal Length and Petal Width.



---

##  Repository Contents

* `iris_classification.ipynb`: The primary project file containing all executed code for data loading, cleaning, EDA, model training, and evaluation.
* `README.md`: This summary file.
* `Iris.csv`: The raw dataset used.
