# DL_Assignment1_MLP_Credit_Risk
#  Credit Risk Prediction using Multi-Layer Perceptron (MLP)

A **Deep Learning project** that applies a **Multi-Layer Perceptron (MLP) neural network** to predict credit risk using structured financial data.

The project uses the **German Credit Dataset** to classify applicants into **good or bad credit risks**, demonstrating how neural networks can be used for financial risk assessment.

This assignment showcases practical concepts in **data preprocessing, neural network modeling, feature scaling, model evaluation, and performance visualization**.

---

#  Project Overview

Financial institutions must assess the **creditworthiness of applicants** before approving loans.

This project builds a **neural network-based classification model** that predicts whether a loan applicant is a **good or bad credit risk** using historical financial data.

The workflow includes:

* Data preprocessing and cleaning
* Feature encoding and normalization
* Training an MLP neural network
* Evaluating model performance using classification metrics
* Visualizing training behavior and prediction results

---

#  Problem Statement

Credit risk assessment is critical for financial institutions because incorrect predictions may lead to:

* Financial losses due to loan defaults
* Rejection of reliable borrowers

Traditional rule-based approaches may not capture complex relationships in financial data.

This project explores how **neural networks can learn patterns in structured financial data** to improve credit risk prediction.

---

#  Dataset Description

The model uses the **German Credit Dataset**, which contains:

* **1000 samples**
* **20 financial and demographic features**

Each record represents a loan applicant and includes attributes such as:

* Credit history
* Loan amount
* Employment status
* Personal information
* Financial background

The dataset is used to classify applicants as:

```id="a6h3qv"
Good Credit Risk
Bad Credit Risk
```

---

#  Data Preprocessing

Before training the model, several preprocessing steps are performed:

* Handling missing or inconsistent data
* Encoding categorical variables into numerical format
* Feature normalization to standardize value ranges
* Preparing features for neural network input

These steps ensure the dataset is **clean and suitable for machine learning models**.

---

#  Train–Test Split

The dataset is divided into:

* **Training Set** – used to train the neural network
* **Testing Set** – used to evaluate the model’s generalization performance

This prevents overfitting and provides a fair evaluation of model accuracy.

---

# Feature Scaling

Feature scaling is performed using **StandardScaler** to normalize feature values.

Benefits of scaling include:

* Faster neural network convergence
* Improved model stability
* Better gradient optimization

---

#  Model Architecture

The predictive model uses a **Multi-Layer Perceptron (MLP)** neural network with the following architecture:

```id="h5w6fd"
Input Layer
      │
      ▼
Hidden Layer 1 (ReLU)
      │
      ▼
Hidden Layer 2 (ReLU)
      │
      ▼
Output Layer (Sigmoid)
```

### Activation Functions

| Layer         | Activation |
| ------------- | ---------- |
| Hidden Layers | ReLU       |
| Output Layer  | Sigmoid    |

The sigmoid output layer enables **binary classification** for credit risk prediction.

---

#  Model Training

The neural network is trained using:

| Component         | Method                          |
| ----------------- | ------------------------------- |
| Loss Function     | Binary Cross-Entropy            |
| Optimizer         | Adam                            |
| Training Strategy | Iterative gradient optimization |

During training, the model learns patterns that distinguish **reliable borrowers from risky applicants**.

---

#  Training Visualization

Training performance is monitored using:

* **Training Loss**
* **Validation Loss**
* **Training Accuracy**
* **Validation Accuracy**

Graphs are plotted to visualize how the model improves during training.

These curves help detect issues such as:

* Overfitting
* Underfitting
* Training instability

---

# Model Evaluation

The trained model is evaluated using standard classification metrics:

| Metric    | Purpose                              |
| --------- | ------------------------------------ |
| Accuracy  | Overall prediction correctness       |
| Precision | Correct positive predictions         |
| Recall    | Ability to detect risky applicants   |
| F1 Score  | Balance between precision and recall |

These metrics provide a comprehensive evaluation of model performance.

---

# Confusion Matrix

A **confusion matrix** is generated to visualize prediction results:

```id="38hd5p"
                Predicted
               Good   Bad
Actual Good      ✔     ✖
Actual Bad       ✖     ✔
```

The confusion matrix helps analyze:

* True positives
* True negatives
* False positives
* False negatives

This provides deeper insight into model decision behavior.

---

#  Project Structure

```id="ijh1rq"
├── Assignment1_Report.pdf
├── MLP_Credit_Risk_Prediction.ipynb            
└── README.md                 
```

---

#  Challenges & Learnings

### Data Preprocessing

Handling categorical financial data required careful encoding and scaling.

### Neural Network Optimization

Selecting appropriate activation functions and training parameters was important for model convergence.

### Model Evaluation

Using multiple evaluation metrics provided a deeper understanding of classification performance.

---

#  Author

**Saksham Semwal*

GitHub
https://github.com/sakshamsemwal10

LinkedIn
https://www.linkedin.com/in/saksham-semwal-380220394/
---
