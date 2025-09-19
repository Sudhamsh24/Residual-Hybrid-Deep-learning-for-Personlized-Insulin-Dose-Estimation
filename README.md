# 🚀 Personalized Insulin Dosage Prediction Using Hybrid LSTM–GRU  

## 📌 Project Overview  
This project introduces a **Hybrid Deep Learning Framework** for predicting personalized insulin dosages in diabetic patients.  
By combining **LSTM** and **GRU** layers with residual learning, the model captures both short-term glucose fluctuations and long-term physiological patterns.  

The model processes the **AIM94 dataset**, applying advanced preprocessing and temporal feature engineering to transform irregular event logs into structured time-series suitable for deep learning.  

---

## 🔑 Key Highlights  
- 🌿 **Residual Hybrid Architecture** → LSTM + GRU with skip connections for stable and efficient learning.  
- 🛠 **Advanced Preprocessing** → Converts raw event-based records into structured multivariate time series.  
- ⏳ **Sliding Window Modeling** → Generates sequences to forecast insulin dosage.  
- 📊 **Superior Performance** → Achieved **R² = 0.805**, **MAE = 1.29**, and **MSE = 3.27**, improving accuracy significantly compared to baselines.  

---

## 🎯 Objectives  
- Develop a robust hybrid deep learning model for insulin prediction.  
- Improve accuracy and stability over traditional models.  
- Provide a foundation for **personalized diabetes management systems**.  

---

## 📂 Dataset  
- Source: **AIM94 Dataset**  
- Type: Multivariate time-series (event-based logs).  
- Preprocessing: Missing value handling, normalization, and feature engineering.  

---

## ⚙️ Methodology  
1. **Data Preprocessing** – cleaning, normalization, and structuring.  
2. **Sliding Window Generation** – creating input sequences.  
3. **Model Design** – Hybrid LSTM + GRU with residual connections.  
4. **Training & Validation** – optimizing loss and tuning hyperparameters.  
5. **Evaluation** – measuring R², MAE, and MSE metrics.  

---

## 📈 Results  
- R² = **0.805**  
- MAE = **1.29**  
- MSE = **3.27**  
- Outperformed baseline models significantly.  

---

## 🏗 Future Scope  
- Integrating Reinforcement Learning for real-time dosage optimization.  
- Extending to continuous glucose monitoring (CGM) devices.  
- Deploying as a **mobile application** for personalized healthcare.  
