# 🧠 Human Activity Recognition using Machine Learning and LSTM

## 📌 Overview
This project develops and evaluates machine learning and deep learning models for **Human Activity Recognition (HAR)** using smartphone sensor data from the UCI HAR dataset.

The goal is to classify human activities such as walking, sitting, and standing based on time-series signals captured from accelerometers and gyroscopes.

---

## 🎯 Objectives
- Build classification models for activity recognition
- Compare traditional ML models with deep learning (LSTM)
- Evaluate model performance using classification metrics
- Analyse misclassifications using a confusion matrix
- Demonstrate time-series modelling capabilities

---

## 📊 Dataset
- **Source:** UCI Human Activity Recognition Dataset  
- **Features:** Sensor signals (accelerometer & gyroscope)  
- **Target Classes:**
  - WALKING
  - WALKING_UPSTAIRS
  - WALKING_DOWNSTAIRS
  - SITTING
  - STANDING
  - LAYING

---

## ⚙️ Models Implemented
- Logistic Regression
- Random Forest
- Long Short-Term Memory (LSTM)

---

## 🧪 Model Performance

| Model               | Accuracy |
|--------------------|---------|
| Logistic Regression| ~XX%    |
| Random Forest      | ~XX%    |
| LSTM               | ~XX%    |

👉 The LSTM model achieved the best performance by capturing temporal dependencies in the sensor data.

---

## 📈 Results

### 🔹 Confusion Matrix (LSTM)

![Confusion Matrix](results/confusion_matrix.png)

### 🔍 Key Insights
- High classification accuracy across all activities
- Minor confusion between:
  - **SITTING vs STANDING** (similar stationary patterns)
  - **WALKING vs stair-related activities** (similar motion dynamics)
- Strong performance on distinct activities like **LAYING**


## Confusion Matrix Analysis

The LSTM model demonstrates strong classification performance across all activity classes, with most predictions correctly aligned along the diagonal.

Minor misclassifications occur between:
- Sitting and Standing (due to similar stationary patterns)
- Walking and stair-related activities (due to similar motion dynamics)

These results indicate that the model effectively captures temporal patterns in human activity data, while highlighting expected challenges in distinguishing closely related movements.
---

## 🧠 Technical Approach

### 🔹 Data Processing
- Label encoding for activity classes
- Feature scaling and normalization
- Train-test split

### 🔹 Deep Learning (LSTM)
- Sequential model architecture
- Dense + Dropout layers for regularization
- Optimized using Adam optimizer

---

## 🛠️ Technologies Used
- Python
- NumPy, Pandas
- Scikit-learn
- TensorFlow / Keras
- Matplotlib, Seaborn

---

## 📁 Project Structure
