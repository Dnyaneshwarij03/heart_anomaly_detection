# heart_anomaly_detection
# 🩺 Heart Monitoring & Anomaly Detection System using Machine Learning

A Machine Learning-based system that analyzes health vitals (heart rate and SpO₂) to detect anomalies and simulate alerts. This project demonstrates how AI can be applied to real-world healthcare problems, using unsupervised learning, visualizations, and an interactive app.

---

## 📌 Project Summary

This project aims to monitor a person's vital signs and identify abnormal patterns using **Isolation Forest**, a powerful anomaly detection algorithm. Users can input their current heart rate and SpO₂ level to check whether their vitals are within a normal range, and view anomaly trends over time through interactive charts.

---

## 📊 Technologies Used

| Technology     | Purpose                               |
|----------------|----------------------------------------|
| Python         | Programming language                   |
| Pandas         | Data manipulation                      |
| NumPy          | Numerical operations                   |
| Scikit-learn   | ML model: Isolation Forest             |
| Matplotlib     | Data visualization                     |
| Gradio         | Live UI for user interaction           |
| Jupyter Notebook | Development & execution environment |

---

## 🧠 How It Works

1. **Dataset**: Uses a heart health dataset containing maximum heart rate (`thalach`).
2. **Feature Engineering**:
   - Renames `thalach` as `heart_rate`
   - Simulates SpO₂ (oxygen saturation) values using synthetic data
   - Creates timestamp to simulate real-time data
3. **Preprocessing**:
   - Missing value handling
   - Feature scaling using `StandardScaler`
4. **Model**:
   - Trains `IsolationForest` on `heart_rate` and `spo2`
   - Flags abnormal data points as anomalies
5. **Visualization**:
   - Time-series chart showing anomalies using `matplotlib`
6. **User App**:
   - Built with `Gradio`
   - Allows user input for heart rate and SpO₂
   - Returns a real-time prediction (Normal / Anomaly)

---
