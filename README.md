# 🔥 Employee Burnout Prediction using Machine Learning

## 📌 Overview

Burnout is a state of physical, emotional, and mental exhaustion caused by prolonged workplace stress. It is recognized by the World Health Organization (WHO) as an occupational phenomenon.

This project develops a machine learning model to predict employee burnout rates using workplace and personal factors. The goal is to help organizations proactively identify burnout risks and improve employee well-being.

---

## 🎯 Objective

* Predict employee burnout levels
* Analyze factors contributing to burnout
* Compare multiple regression models
* Identify the most accurate predictive model

---

## 📊 Dataset Description

### 🔹 Features

| Feature                  | Definition                                                     |
| ------------------------ | -------------------------------------------------------------- |
| **Employee ID**          | Unique identifier for each employee (e.g., `fffe390032003000`) |
| **Date of Joining**      | Date the employee joined the organization                      |
| **Gender**               | Employee gender (Male/Female)                                  |
| **Company Type**         | Type of company (Service/Product)                              |
| **WFH Setup Available**  | Availability of work-from-home option (Yes/No)                 |
| **Designation**          | Job level (0.0 – 5.0, higher = senior role)                    |
| **Resource Allocation**  | Workload level (1.0 – 10.0, higher = more working hours)       |
| **Mental Fatigue Score** | Mental fatigue level (0.0 – 10.0)                              |

---

## 🎯 Target Variable

| Feature       | Definition                                                                                          |
| ------------- | --------------------------------------------------------------------------------------------------- |
| **Burn Rate** | Target variable representing burnout level (0.0 – 1.0), where higher values indicate higher burnout |

---

## 📊 Problem Type

This is a **Supervised Machine Learning Regression Problem**, where the goal is to predict a continuous value (**Burn Rate**) based on multiple input features.

---

## 🧠 Models Used

The following regression algorithms were implemented and compared:

* Linear Regression
* Polynomial Regression
* Support Vector Regression (SVR)
* Decision Tree Regression
* Ridge Regression
* Lasso Regression
* K-Nearest Neighbors (KNN)
* Random Forest Regression

---

## ⚙️ Methodology

* Data preprocessing and cleaning
* Feature selection and encoding
* Model training using multiple regression algorithms
* Performance evaluation using Accuracy and Mean Squared Error (MSE)
* Model comparison and selection

---

## 📈 Model Performance

| Model                           | Accuracy (3 Features) | Accuracy (7 Features) | MSE (3 Features) | MSE (7 Features) |
| ------------------------------- | --------------------- | --------------------- | ---------------- | ---------------- |
| Polynomial Regression           | 93.08%                | 92.96%                | 0.0027           | 0.0028           |
| K-Nearest Neighbors (KNN)       | 92.84%                | 89.12%                | 0.0028           | 0.0043           |
| Random Forest                   | 92.65%                | 92.01%                | 0.0029           | 0.0031           |
| Decision Tree                   | 92.57%                | 85.99%                | 0.0029           | 0.0056           |
| Linear Regression               | 92.12%                | 92.21%                | 0.0031           | 0.0031           |
| Ridge Regression                | 91.92%                | 92.01%                | 0.0031           | 0.0031           |
| Lasso Regression                | 91.92%                | 92.01%                | 0.0031           | 0.0031           |
| Support Vector Regression (SVR) | 91.78%                | -260426.42%           | 0.0032           | 10422.3          |

---

## 🏆 Best Model

* **Polynomial Regression** achieved the highest accuracy (**93.08%**) with the lowest MSE (**0.0027**)
* **Random Forest** showed strong and consistent performance across both feature sets

---

## ⚠️ Observations

* Increasing the number of features did not always improve performance
* Some models (like SVR) were highly sensitive to feature scaling and parameters
* Tree-based models provided stable and reliable predictions
* Feature selection plays a critical role in model performance

---

## 💡 Impact

This project helps organizations:

* Detect burnout early
* Improve workplace conditions
* Support employee mental health
* Increase productivity and job satisfaction

---

## 🚀 Future Work

* Deploy the model as a web application
* Integrate real-time prediction systems
* Expand dataset with behavioral and psychological features

---

## 🛠️ Technologies Used

* Python
* Scikit-learn
* Pandas & NumPy
* Matplotlib / Seaborn

---

## 👩‍💻 Author

Nouf Alshehri
Master’s in Artificial Intelligence

---
