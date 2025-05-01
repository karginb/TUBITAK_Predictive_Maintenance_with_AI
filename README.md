# 🔧 Predictive Maintenance with AI

This project aims to optimize maintenance processes by predicting machine failures in an industrial setting. The dataset includes parameters such as air and process temperatures, torque, rotational speed, and tool wear — all of which contribute to anticipating equipment failures.

> 📌 This project is developed in collaboration with [TÜBİTAK (The Scientific and Technological Research Council of Türkiye)](https://www.tubitak.gov.tr).

---

## 🚀 Project Objective

The goal of the project is to minimize unplanned downtimes and reduce maintenance costs by predicting equipment failures in advance, thereby ensuring production continuity and efficiency.

Sensor data from machines are processed and analyzed using various machine learning techniques to achieve accurate failure predictions.

---

## 🧠 Methodology

### 🔹 Data Preprocessing
- Missing data handling
- Categorical encoding: One-Hot and Label Encoding
- Feature scaling:
  - **Normalization** with MinMaxScaler (for KNN)
  - **Standardization** with StandardScaler (for tree-based models)

### 🔹 Feature Selection Techniques
Applied independently:
- **Random Forest Feature Importance** + **Correlation Analysis**
- **Recursive Feature Elimination (RFE)**

### 🔹 Machine Learning Models
- K-Nearest Neighbors (with normalized data)
- Random Forest (with standardized data)
- Decision Tree (with standardized data)

---

## 📊 Evaluation Metrics
Each model is evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC-AUC Curve

---

## 🗃️ Dataset Overview

Key columns in the dataset:
- `Air temperature [K]`
- `Process temperature [K]`
- `Rotational speed [rpm]`
- `Torque [Nm]`
- `Tool wear [min]`
- `Machine failure`: Overall machine failure (binary)
- `TWF`, `HDF`, `PWF`, `OSF`, `RNF`: Specific failure types (binary)

---

## 🧪 How to Run

### Install dependencies

```bash
pip install -r requirements.txt
python Development_of_Machine_Learning_Models_on_Predictive_Maintenance_Dataset.ipynb
