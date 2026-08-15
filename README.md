# Heart Disease Prediction using Logistic Regression

A machine learning classification project that uses Logistic Regression to predict the presence of heart disease based on patient health and clinical features. The project covers the complete machine learning workflow, including exploratory data analysis, data preprocessing, feature scaling, model training, hyperparameter tuning, and model evaluation.

---

## 📌 Project Overview

Heart disease is one of the major health challenges worldwide. Machine learning can be used to analyze clinical and health-related features and identify patterns associated with the presence of heart disease.

In this project, **Logistic Regression** is used as a binary classification algorithm to predict whether a patient is likely to have heart disease based on the available input features.

The project focuses not only on training a model, but also on understanding the data, preparing it correctly, optimizing the model, and evaluating its performance using multiple classification metrics.

---

## 🎯 Problem Statement

The objective of this project is to build a machine learning classification model capable of predicting the presence of heart disease from patient-related clinical features.

The target variable represents the presence or absence of heart disease, making this a **binary classification problem**.

---

## 🧠 Machine Learning Approach

The project follows a structured machine learning workflow:

1. Data loading
2. Data understanding and inspection
3. Exploratory Data Analysis (EDA)
4. Data preprocessing
5. Train-test split
6. Feature scaling
7. Logistic Regression model training
8. Hyperparameter tuning using GridSearchCV
9. Model evaluation
10. Saving the final trained model

---

## 📊 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the dataset and identify relationships between the input features and the target variable.

The analysis included:

* Distribution analysis
* Feature relationships
* Target variable analysis
* Correlation analysis
* Visualization of important patterns
* Identification of potential outliers and data characteristics

These steps helped provide a better understanding of the dataset before model training.

---

## ⚙️ Data Preprocessing

Before training the model, the dataset was prepared for machine learning.

The preprocessing workflow included:

* Checking the structure of the dataset
* Separating input features and target variable
* Splitting the data into training and testing sets
* Feature scaling
* Preparing the data for Logistic Regression

Feature scaling is particularly important for Logistic Regression because the magnitude of input features can affect the optimization process.

---

## 🤖 Model Used

### Logistic Regression

Logistic Regression was selected as the primary machine learning algorithm because it is a widely used and interpretable algorithm for binary classification problems.

The model estimates the probability of an observation belonging to a particular class and uses a classification threshold to determine the predicted class.

---

## 🔧 Hyperparameter Tuning

To improve the model's performance, **GridSearchCV** was used for hyperparameter tuning.

The tuning process evaluated different combinations of Logistic Regression hyperparameters using cross-validation.

The parameters explored included:

* Regularization type
* Regularization strength
* L1 ratio where applicable

This process helped identify a better-performing configuration for the final model.

---

## 📈 Model Evaluation

The trained model was evaluated using multiple classification metrics rather than relying only on accuracy.

The evaluation included:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* ROC Curve
* ROC-AUC Score

These metrics provide a more comprehensive understanding of the model's classification performance.

---

## 💾 Saved Model

The final trained model has been saved using **Joblib**.

The model file included in this repository is:

```text
Final_Model.joblib
```

This allows the trained model artifact to be stored separately from the Jupyter Notebook and reused without retraining the model from scratch, subject to using the same preprocessing workflow expected by the saved model.

---

## 📁 Project Structure

```text
heart-disease-logistic-regression/
│
├── Heart_Disease_Logistic_Regression.ipynb
├── Final_Model.joblib
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**
* **Joblib**

---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/SiddharthPatil-57/heart-disease-logistic-regression.git
```

### 2. Navigate to the project directory

```bash
cd heart-disease-logistic-regression
```

### 3. Install the required dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open the notebook

Open:

```text
Heart_Disease_Logistic_Regression.ipynb
```

and execute the cells to reproduce the analysis and model training workflow.

---

## 📌 Results

The final model was evaluated using several classification metrics, including accuracy, precision, recall, F1-score, confusion matrix, and ROC-AUC.

### Model Performance

| Metric    |      Result |
| --------- | ----------: |
| Accuracy  | To be added |
| Precision | To be added |
| Recall    | To be added |
| F1-Score  | To be added |
| ROC-AUC   | To be added |

> **Note:** The final values will be added based on the results obtained from the completed notebook.

---

## 📉 Model Evaluation Visualizations

The project includes evaluation visualizations such as:

* Confusion Matrix
* ROC Curve
* Precision-Recall analysis where applicable

These visualizations help understand the model's classification behavior beyond a single performance metric.

---

## 🔍 Key Learnings

Through this project, I worked with several important concepts in machine learning, including:

* Exploratory Data Analysis
* Data preprocessing
* Feature scaling
* Binary classification
* Logistic Regression
* L1 and L2 regularization
* Hyperparameter tuning
* GridSearchCV
* Cross-validation
* Classification metrics
* Confusion Matrix
* ROC Curve and ROC-AUC
* Model serialization using Joblib

---

## 🔮 Future Improvements

Possible improvements to this project include:

* Comparing Logistic Regression with other classification algorithms
* Performing more extensive feature selection
* Exploring additional hyperparameter configurations
* Building an interactive prediction interface
* Deploying the trained model as an API or web application
* Monitoring model performance on new data

---

## ⚠️ Disclaimer

This project is developed for **educational and machine learning practice purposes**.

The predictions generated by this model should not be considered medical advice or used as a substitute for professional medical diagnosis.

---

## 👨‍💻 Author

**Siddharth Patil**

B.Tech — Artificial Intelligence & Data Science

GitHub: [SiddharthPatil-57](https://github.com/SiddharthPatil-57)
