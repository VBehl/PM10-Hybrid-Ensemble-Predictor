
# 🔍 PM10-Hybrid-Ensemble-Predictor


A machine learning pipeline to forecast PM₁₀ concentration using a meta-ensemble framework that integrates XGBoost, Artificial Neural Networks (ANN), and a Random Forest meta-learner for robust, high-accuracy air quality prediction.

---

## 🚀 Project Overview

This project improves "air quality forecasting" by combining advanced regression models in a stacked ensemble:

- **XGBoost** models structured interactions and handles feature sparsity.
- **ANN** captures complex non-linear dependencies in environmental data.
- **Random Forest** meta-model fuses predictions from both models for robust output.


## 🧠 Methodology

1. **Data Preparation**
   - Collected PM₁₀ and meteorological data from 10 urban stations.
   - Handled missing values, removed outliers, and applied Min-Max scaling.
   - Engineered lag features and used **SMOTER** to balance target values.

2. **Base Models**
   - **XGBoost** trained to capture structured feature interactions.
   - **ANN** used to model non-linear dependencies with dropout regularization.

3. **Meta-Ensemble**
   - Combined predictions from XGBoost and ANN using a **Random Forest** meta-learner for enhanced accuracy.

4. **Evaluation & Visualization**
   - Assessed using **R², MAE, RMSE**.
   - Visualized results via scatter plots, residuals, and feature importance.
---

## 📦 Features

- Hybrid meta-ensemble learning pipeline
- Handles real-world environmental and pollution datasets
- Balances noisy and imbalanced data using **SMOTER**
- Compatible with both **local machines** and **cloud (GPU-enabled)** platforms
- Modular and reproducible code structure

## 📊 Results

| Model            | R² Score | MAE     | RMSE    |
|------------------|----------|---------|---------|
| XGBoost          | 0.9996   | 0.0027  | 0.0044  |
| ANN              | 0.9549   | 0.0364  | 0.0494  |
| **Meta-Ensemble**| **0.9997** | **0.0009** | **0.0039** |

---

## 🛠️ Requirements

- Python 3.9+
- `scikit-learn`
- `xgboost`
- `tensorflow`, `keras`
- `matplotlib`, `seaborn`
- `pandas`, `numpy`

### 📦 Install Dependencies

```bash
pip install -r requirements.txt
```
---
## 🖼️ Visual Outputs

- [XGBoost Scatter Plot](./results/XgBoost%20Scatter%20Plot.jpg)
- [ANN Scatter Plot](./results/ANN%20scatter%20plot.jpg)
- [Meta Model Plot](./results/Meta%20Model%20Plot.jpg)
- [Feature Correlation Matrix](./results/Feature%20Correlation%20Matrix.jpg)
- [Model Comparison](./results/Model%20Comparison.jpg)

---

## 📚 References
- [Comparative Analysis of Machine Learning Techniques for Predicting Air Quality in Smart Cities](./Comparative_Analysis_of_Machine_Learning_Techniques_for_Predicting_Air_Quality_in_Smart_Cities.pdf)
- [Comparative Analysis Study for Air Quality Prediction in Smart Cities Using Regression Techniques](./Comparative_Analysis_Study_for_Air_Quality_Predict.pdf)
- [A systematic study on PM2.5 and PM10 concentration prediction in air pollution using machine learning and deep learning model](https://www.sciencedirect.com/science/article/pii/S2590182625000967)

---

## 📌 License

This project is for academic and research use only. Feel free to adapt with credit.


