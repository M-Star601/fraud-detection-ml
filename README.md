# Fraud Detection Using Supervised Machine Learning

## 📌 Project Overview

This project focuses on detecting fraudulent transactions using **Supervised Machine Learning** techniques.

Fraud detection is an important real-world problem in financial systems because fraudulent transactions are usually much fewer than legitimate transactions. This creates a **class imbalance** problem.

To address this problem, this project uses **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the training data and compares two machine learning models:

* Logistic Regression
* Random Forest Classifier

The models are evaluated using **Precision, Recall, and ROC-AUC**, rather than relying on Accuracy alone.

---

## 🎯 Objectives

The main objectives of this project are:

1. Analyze a real-world fraud detection dataset.
2. Perform data preprocessing and exploratory data analysis.
3. Identify the class imbalance between legitimate and fraudulent transactions.
4. Apply SMOTE to balance the training dataset.
5. Train a Logistic Regression model.
6. Train a Random Forest Classifier.
7. Perform hyperparameter tuning.
8. Evaluate the models using:

   * Precision
   * Recall
   * ROC-AUC
9. Compare the performance of the models.
10. Identify the model that performs better for fraud detection.

---

## 📊 Dataset

The project uses a credit card transaction dataset containing information about transactions and their corresponding class labels.

The target variable is:

* `0` → Normal transaction
* `1` → Fraudulent transaction

The dataset is highly imbalanced because legitimate transactions are much more common than fraudulent transactions.

### Dataset Handling

The dataset is **not included in this GitHub repository** because of its large size.

Place the dataset in your local/Colab environment before running the notebook.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Imbalanced-learn
* Matplotlib
* Seaborn
* Google Colab / Jupyter Notebook
* Git & GitHub

---

## 🤖 Machine Learning Models

### 1. Logistic Regression

Logistic Regression is used as a baseline classification model for detecting fraudulent transactions.

### 2. Random Forest

Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve classification performance.

### 3. Hyperparameter Tuning

GridSearchCV is used to find better Random Forest parameters and improve model performance.

---

## ⚖️ Handling Class Imbalance

Fraudulent transactions represent a minority class.

To address this problem, **SMOTE** is applied only to the training data.

```text
Original Training Data
        ↓
      SMOTE
        ↓
Balanced Training Data
        ↓
Machine Learning Models
```

The test data is kept unchanged so that the models are evaluated on realistic transaction distributions.

---

## 📈 Evaluation Metrics

Accuracy is not used as the primary evaluation metric because an imbalanced dataset can make Accuracy misleading.

The following metrics are used:

### Precision

Precision measures how many transactions predicted as fraud are actually fraudulent.

### Recall

Recall measures how many actual fraudulent transactions are correctly detected.

### ROC-AUC

ROC-AUC measures the model's ability to distinguish between legitimate and fraudulent transactions across different classification thresholds.

---

## 🔍 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Exploration
   ↓
Data Cleaning
   ↓
Class Imbalance Analysis
   ↓
Train-Test Split
   ↓
SMOTE on Training Data
   ↓
Feature Scaling
   ↓
Logistic Regression
   ↓
Random Forest
   ↓
Hyperparameter Tuning
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Final Fraud Detection Model
```

---

## 📊 Model Evaluation

The models are compared using:

| Model               | Precision | Recall | ROC-AUC |
| ------------------- | --------: | -----: | ------: |
| Logistic Regression |         — |      — |       — |
| Random Forest       |         — |      — |       — |
| Tuned Random Forest |         — |      — |       — |

The actual values are generated when the notebook is executed.

---

## 📉 Visualizations

The project includes visualizations such as:

* Class distribution
* Confusion matrix
* ROC curve
* Model performance comparison

These visualizations help understand the performance of the fraud detection models.

---

## 📁 Project Structure

```text
fraud-detection-ml/
│
├── Fraud_Detection_Project_ipynb.ipynb
├── README.md
└── .gitignore
```

The dataset is excluded from the repository because of its large size.

---

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/fraud-detection-ml.git
```

### 2. Open the project

Open the project folder in **VS Code**, **Jupyter Notebook**, or **Google Colab**.

### 3. Install required libraries

```bash
pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn
```

### 4. Add the dataset

Place the fraud detection CSV dataset in your working environment.

### 5. Open the notebook

```text
Fraud_Detection_Project_ipynb.ipynb
```

### 6. Run all cells

Execute the notebook cells from beginning to end.

---

## 🧠 Key Learning Outcomes

Through this project, the following concepts are demonstrated:

* Supervised Machine Learning
* Binary Classification
* Fraud Detection
* Exploratory Data Analysis
* Class Imbalance
* SMOTE
* Logistic Regression
* Random Forest
* Hyperparameter Tuning
* Confusion Matrix
* Precision
* Recall
* ROC-AUC
* Model Comparison

---

## 🚀 Future Improvements

Possible improvements include:

* Testing additional classification algorithms.
* Using XGBoost or other ensemble models.
* Improving feature engineering.
* Using cross-validation techniques.
* Deploying the trained model as a web application or API.
* Building a real-time fraud detection system.

---


