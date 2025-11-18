#  Data Mining Project: Iris Flower Species Classification with Decision Trees

##  Group Details

| Name | ID |
| :--- | :--- |
| Abel Tamiru | 1213 |
| Fikremariyam Tadesse | 0990 |
| Jalane Lamessa | 1244 |
| Meseret Kassa | 1433 |
| Natinael Tegegne | 1570 |

---

##  Project Objectives

This project fulfills the requirements for the **Data Mining and Data Warehouse** course. Our goal was to implement a complete data mining workflow, focusing on **simple predictive modeling** using the classic Iris dataset.

The core objectives were:
1.  **Data Preparation:** Load, clean, and preprocess the raw data.
2.  **Exploratory Data Analysis (EDA):** Visually identify patterns and correlations between the four physical features (sepal length/width, petal length/width).
3.  **Model Implementation:** Build and train an interpretable **Decision Tree Classifier** to predict one of three species: *Iris-Setosa*, *Iris-Versicolor*, or *Iris-Virginica*.
4.  **Evaluation:** Rigorously assess model performance using key classification metrics.

---

##  Methodology Overview

The project followed a standard Machine Learning pipeline as outlined in the course guidelines:

1.  **Data Cleaning:** Checked for and handled missing values and duplicate records to ensure data quality.
2.  **Feature Engineering:** The categorical `Species` column was converted into numerical labels using `LabelEncoder`. Features were separated from the target variable.
3.  **Data Splitting:** The dataset was partitioned into training (80%) and testing (20%) sets to facilitate unbiased performance evaluation.
4.  **Model Training:** A `DecisionTreeClassifier` was trained on the training data using the entropy criterion for splitting.
5.  **Model Evaluation:** Performance was measured using Accuracy, a Classification Report, and a Confusion Matrix on the unseen test data.

---

##  Detailed Results and Insights

### 1. Model Performance Summary

The Decision Tree classifier demonstrated strong ability to distinguish between the three Iris species, achieving high accuracy on the test set.

| Metric | Value |
| :--- | :--- |
| **Test Accuracy** | **89.5%** |

### 2. Feature Importance

The model determined that **Petal Length** is overwhelmingly the most crucial factor for classification, confirming insights often drawn during the EDA phase.

| Feature | Importance Value | **Significance** |
| :--- | :--- | :--- |
| **Petal Length (cm)** | **0.92** | Primary determinant of species. |
| Petal Width (cm) | 0.05 | Secondary factor. |
| Sepal Width (cm) | 0.02 | Minimal influence. |
| Sepal Length (cm) | 0.01 | Minimal influence. |

### 3. Confusion Matrix Analysis

The raw output of the Confusion Matrix confirms the classification performance: `[[12, 0, 0], [0, 12, 1], [0, 3, 10]]`.

-   **Perfect Classification:** The model successfully classified **all 12 instances of *Iris-Setosa*** (100% accuracy for this class).
-   **Confusion Points:** The only classification errors occurred between *Iris-Versicolor* and *Iris-Virginica*, where 1 *Versicolor* was misclassified as *Virginica*, and 3 *Virginica* were misclassified as *Versicolor*.

---

##  Key Visualizations


### 1. Decision Tree Structure

The visualization of the trained tree provides a transparent, rule-based view of how the model makes decisions. This is crucial for interpretability.



<img width="1105" height="636" alt="download" src="https://github.com/user-attachments/assets/8373fae7-f28d-4bc9-92c1-648353d08155" />



### 2. Exploratory Data Analysis (EDA)

The Pairplot and scatter plots were vital for confirming the linear separability of the Setosa species and the overlapping nature of Versicolor and Virginica, which explains the minor misclassifications observed in the Confusion Matrix.



---

## 🔗 Repository Contents

* `iris_classification.ipynb`: The fully executed Jupyter Notebook containing all code and outputs (the primary deliverable).
* `README.md`: This project summary and documentation file.
* `Iris.csv`: The dataset used for the project.
