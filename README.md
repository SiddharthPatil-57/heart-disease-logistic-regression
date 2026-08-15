# Heart Disease Prediction using Logistic Regression

A machine learning classification project that uses **Logistic Regression** to predict the presence of heart disease based on patient health and clinical features.

The project follows an end-to-end machine learning workflow, including **data understanding, exploratory data analysis, preprocessing, feature scaling, model training, hyperparameter tuning, and model evaluation**.

---

## 📌 Project Overview

Heart disease is one of the major health challenges worldwide. Machine learning can be used to analyze health-related and clinical features to identify patterns associated with the presence or absence of heart disease.

In this project, **Logistic Regression** is used as a binary classification algorithm to predict whether a patient belongs to the class representing the presence or absence of heart disease based on the available input features.

The project focuses not only on training a machine learning model, but also on understanding the dataset, preparing the data correctly, applying feature scaling, tuning model hyperparameters, and evaluating the final model using multiple classification metrics.

---

## 🎯 Problem Statement

The objective of this project is to build a machine learning classification model capable of predicting the presence or absence of heart disease from patient-related clinical features.

The target variable represents two possible classes, making this a **binary classification problem**.

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

## 📊 Dataset

The dataset used in this project was provided as part of course material for educational and machine learning practice purposes.

The dataset contains patient-related health and clinical features used to perform binary classification for heart disease prediction.

The original course-provided dataset is **not included in this public repository**.

The Jupyter Notebook contains the complete workflow used for data exploration, preprocessing, model training, hyperparameter tuning, and evaluation.

---

## 📊 Exploratory Data Analysis

Exploratory Data Analysis (EDA) was performed to understand the structure and characteristics of the dataset and to identify relationships between the input features and target variable.

The analysis included:

- Distribution analysis
- Feature relationship analysis
- Target variable analysis
- Correlation analysis
- Data visualization
- Identification of potential outliers
- Examination of important patterns and data characteristics

These steps helped provide a better understanding of the dataset before applying the machine learning model.

---

## ⚙️ Data Preprocessing

Before training the model, the dataset was prepared for machine learning.

The preprocessing workflow included:

- Inspecting the dataset structure
- Separating input features and target variable
- Splitting the dataset into training and testing sets
- Feature scaling
- Preparing the processed data for Logistic Regression

Feature scaling was applied because Logistic Regression can be affected by differences in the scale and magnitude of input features.

---

## 🤖 Model Used

### Logistic Regression

**Logistic Regression** was selected as the primary machine learning algorithm because it is a widely used and interpretable algorithm for binary classification problems.

The model estimates the probability of an observation belonging to a particular class and uses a classification threshold to determine the predicted class.

---

## 🔧 Regularization

Regularization was considered during model optimization to help control model complexity and reduce the risk of overfitting.

The hyperparameter search included different regularization configurations, including:

- **L1 regularization**
- **L2 regularization**
- **Elastic Net regularization**
- Regularization strength (`C`)
- `l1_ratio` for Elastic Net where applicable

These configurations were evaluated during hyperparameter tuning to identify a suitable Logistic Regression model.

---

## 🔍 Hyperparameter Tuning

**GridSearchCV** was used to systematically evaluate different combinations of Logistic Regression hyperparameters.

Cross-validation was used during the grid search to compare different parameter configurations and identify a suitable configuration for the final model.

The hyperparameters explored included:

- Regularization type (`penalty`)
- Regularization strength (`C`)
- L1 ratio (`l1_ratio`) where applicable

The selected configuration was then used to train the final Logistic Regression model.

---

## 📈 Model Evaluation

The final Logistic Regression model was evaluated on the test dataset using multiple classification metrics rather than relying only on accuracy.

The evaluation included:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

These metrics provide a broader understanding of the model's classification performance across both classes.

---

## 📌 Results

The final Logistic Regression model achieved an overall **test accuracy of 84%** on the test dataset.

### Classification Report

| Class | Precision | Recall | F1-Score | Support |
|:---:|---:|---:|---:|---:|
| 0 | 0.86 | 0.80 | 0.83 | 15 |
| 1 | 0.82 | 0.88 | 0.85 | 16 |
| **Accuracy** | — | — | **0.84** | **31** |
| **Macro Average** | **0.84** | **0.84** | **0.84** | **31** |
| **Weighted Average** | **0.84** | **0.84** | **0.84** | **31** |

### Performance Summary

- **Test Accuracy:** 84%
- **Precision — Class 0:** 86%
- **Recall — Class 0:** 80%
- **F1-Score — Class 0:** 83%
- **Precision — Class 1:** 82%
- **Recall — Class 1:** 88%
- **F1-Score — Class 1:** 85%

The model achieved an overall **84% accuracy** on the test set.

For Class 1, the model achieved a **recall of 88%**, meaning that it correctly identified 88% of the actual Class 1 samples in the test dataset.

> **Note:** These results are specific to the test split used in this project and should not be interpreted as clinical performance or medical diagnostic accuracy.

---

## 📉 Model Evaluation Visualization

The project includes visual evaluation of the trained model, including:

### Confusion Matrix

The confusion matrix provides insight into the model's classification behavior by showing the number of correct and incorrect predictions for each class.

The complete visualization and analysis can be found in the Jupyter Notebook.

---

## 💾 Saved Model

The final trained Logistic Regression model was serialized using **Joblib**.

The saved model file included in this repository is:

```text
Final_Model.joblib
```

Saving the trained model allows the model artifact to be stored separately from the Jupyter Notebook and reused without retraining, provided that the input data follows the preprocessing workflow expected by the saved model.

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

### File Description

| File | Description |
|---|---|
| `Heart_Disease_Logistic_Regression.ipynb` | Complete data analysis, preprocessing, model training, tuning, and evaluation workflow |
| `Final_Model.joblib` | Serialized final Logistic Regression model |
| `requirements.txt` | Python dependencies required for the project |
| `README.md` | Project documentation |
| `.gitignore` | Specifies files and directories that should not be tracked by Git |

---

## 🛠️ Technologies Used

- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Jupyter Notebook**
- **Joblib**

---

## 📦 Requirements

The main Python libraries used in this project are:

```text
numpy
pandas
matplotlib
seaborn
scikit-learn
jupyter
joblib
```

The complete dependency list is available in:

```text
requirements.txt
```

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

The dataset used in this project was provided as course material and is not included in the public repository.

The notebook can be used to review the complete machine learning workflow, including:

- Data exploration
- Data preprocessing
- Feature scaling
- Logistic Regression training
- Hyperparameter tuning
- Model evaluation

---

## 🔍 Key Learnings

Through this project, I worked with several important machine learning concepts, including:

- Exploratory Data Analysis
- Data preprocessing
- Feature scaling
- Binary classification
- Logistic Regression
- L1 regularization
- L2 regularization
- Elastic Net regularization
- Hyperparameter tuning
- GridSearchCV
- Cross-validation
- Classification metrics
- Confusion Matrix
- Model serialization using Joblib

---

## 🔮 Future Improvements

Possible improvements to this project include:

- Comparing Logistic Regression with other classification algorithms
- Performing more extensive feature selection
- Exploring additional hyperparameter configurations
- Improving the preprocessing workflow using a complete machine learning pipeline
- Building an interactive prediction interface
- Deploying the trained model as an API or web application
- Evaluating the model on additional datasets
- Performing more extensive model validation

---

## ⚠️ Disclaimer

This project was developed for **educational and machine learning practice purposes**.

The predictions generated by this model should **not** be considered medical advice, medical diagnosis, or a substitute for evaluation by a qualified healthcare professional.

The reported model performance is based only on the test split used in this project and does not represent clinically validated diagnostic performance.

---

## 👨‍💻 Author

**Siddharth Patil**

B.Tech — Artificial Intelligence & Data Science

GitHub: [SiddharthPatil-57](https://github.com/SiddharthPatil-57)

---

## ⭐ Project

If you find this project useful or informative, feel free to explore the repository and review the complete machine learning workflow implemented in the Jupyter Notebook.
