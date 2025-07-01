# 🧠 Air Quality Index (AQI) Prediction using Deep Learning – Hyderabad, India

This project presents a deep learning-based system to forecast the Air Quality Index (AQI) in Hyderabad using a decade’s worth of pollution and meteorological data. Leveraging historical time-series data and advanced models like **LSTM** and **GRU**, the goal is to build a robust prediction framework that helps inform environmental decisions, public health alerts, and smart city operations.

---

## 📌 Problem Statement

Air pollution in growing urban centers like Hyderabad is a critical challenge, impacting health, climate, and quality of life. Timely and accurate AQI predictions can empower policymakers, environmental bodies, and citizens with early warnings and actionable insights.

---

## 📊 Dataset

- **Source**: Central Pollution Control Board (CPCB), India
- **Period**: 2013–2023
- **Coverage**: 13 monitoring stations across Hyderabad
- **Pollutants**: PM2.5, PM10, SO₂, NOx, NH₃, CO, Ozone
- **Preprocessing**:
  - KNN Imputation for missing values
  - Z-score normalization
  - AQI calculation using national formula
  - Class balancing using SMOTE

---

## ⚙️ Tech Stack

- **Languages**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Imbalanced-learn
- **Deep Learning**: TensorFlow (Keras), PyTorch
- **Tools**: Jupyter Notebook, Google Colab, VS Code

---

## 🧠 Models Used

- LSTM (Long Short-Term Memory)
- GRU (Gated Recurrent Unit)

---

## 📈 Performance

| Metric | LSTM  | GRU   |
|--------|-------|-------|
| R²     | 0.99  | 0.98  |
| MAE    | 0.77  | 0.94  |
| MAPE   | 1.15% | 1.32% |

---

## 🧪 Methodology

1. Combined multi-station time-series data
2. Cleaned and normalized pollutant readings
3. Computed AQI values from raw concentrations
4. Engineered sequential datasets for LSTM/GRU
5. Trained deep models and performed hyperparameter tuning
6. Evaluated using MAE, RMSE, R², and MAPE
7. Visualized model trends, errors, and station-specific insights

---

## 📍 Key Highlights

- Benchmarked LSTM vs GRU on structured air quality sequences
- Used real-world government-grade data
- Created interpretable visualizations (scatter, residual, and line plots)
- Framework can generalize to other cities or pollutants

---

## 📌 Future Work

- Integration with real-time AQI APIs
- Streamlit dashboard for public access
- Forecasting across seasonal trends
- Deployment on cloud platforms (GCP/AWS)

---

## 📚 References

- [CPCB India](https://cpcb.nic.in/)
- [Keras Documentation](https://keras.io/)
- [AQI Computation Standards](https://app.cpcbccr.com/AQI_India/)

---

#
## 📁 Dataset Access

The dataset used in this project was obtained from the [Central Pollution Control Board (CPCB), India](https://app.cpcbccr.com/AQI_India/).  
It includes hourly pollutant concentrations from 13 AQI monitoring stations across Hyderabad (2013–2023).

Due to size constraints, the dataset is not hosted directly on GitHub. You can access a processed version here:

👉 [Download Preprocessed AQI Dataset (Google Drive)](https://drive.google.com/file/d/1KEhKI-57pXY7leEJDmIIbWoVrr5rINy8/view?usp=sharing)

> Note: Please ensure proper attribution if using this dataset elsewhere.

