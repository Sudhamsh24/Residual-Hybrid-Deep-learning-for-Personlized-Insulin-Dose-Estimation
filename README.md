# 🚀 Personalized Insulin Dosage Prediction Using Hybrid LSTM–GRU  

![image](https://github.com/user-attachments/assets/cb878e26-ad5a-4d3d-bb03-73e74a0437f5)

---

## 🧠 Project Overview  
This project presents a **Residual Hybrid Deep Learning Model** for predicting personalized regular insulin dosages in diabetic patients.  

The architecture integrates **LSTM** and **GRU layers** with residual connections, enabling the model to capture both **short-term fluctuations** and **long-term glucose–insulin dependencies**.  

Using the **AIM94 dataset**, advanced preprocessing and temporal feature engineering were applied to transform event-based logs into model-ready time-series data.  

---

## 🔑 Key Highlights  

- 🌿 **Residual Hybrid Architecture** → Combines LSTM and GRU blocks with skip/residual connections to improve gradient flow and learning stability.  
- 🛠 **Raw Data Preprocessing** → Transforms AIM94 logs into time-series format with pivoting, cyclic encoding, and lagged features.  
- ⏳ **Time Window Sequence Modeling** → Generates multivariate input sequences using sliding windows.  
- 📊 **Superior Performance** → Achieved **R² = 0.805, MAE = 1.29, MSE = 3.27**, with ~30% higher R² and >60% lower MSE than baselines.  

---

## 🎯 Objectives  

- Predict **regular insulin dosages** using historical glucose readings, food intake, and physiological events.  
- Capture **temporal patterns** in diabetes management using hybrid recurrent architectures.  
- Preprocess raw medical records into **structured temporal sequences**.  
- Contribute to **personalized decision-support tools** in diabetic care.  

---

## 🧪 Preprocessing Pipeline  

Steps performed on **AIM94 Dataset**:  
- 🧹 **Data Cleaning** → Removed irrelevant codes, handled missing values, standardized timestamps.  
- 🔄 **Event Pivoting** → Converted event codes into structured columns: Glucose, Insulin types, Food, Hypoglycemia, Exercise.  
- 🧩 **Feature Engineering** →  
  - Cyclic encoding for time-of-day  
  - Lag features for glucose/insulin  
  - Temporal indicators (morning/afternoon/evening)  
  - Event flags (food, exercise, symptoms)  
- ⏱ **Sequence Generation** → Sliding window approach to generate input-output pairs.  
- 📏 **Normalization** → Min-Max scaling for convergence.  

### 🔁 Raw to Processed Data Example  

📂 Dataset Link: [AIM94 Diabetes Dataset](https://archive.ics.uci.edu/dataset/34/diabetes)  

<div align="center">

<table>
  <tr>
    <td align="center"><strong>Raw Event-Based Data</strong></td>
    <td></td>
    <td align="center"><strong>Processed Time-Series Data</strong></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/a9ff9fd5-4cda-4f1f-901e-230de855933a" width="360"/></td>
    <td align="center" style="vertical-align: middle;">
      <img src="https://e7.pngegg.com/pngimages/856/761/png-clipart-arrow-free-content-arrow-pointing-left-angle-rectangle.png" width="60"/>
    </td>
    <td><img src="https://github.com/user-attachments/assets/d4b6eccb-2697-4c4d-9821-d0f557c649aa" width="460"/></td>
  </tr>
</table>

</div>

---

## 🏗 Model Architecture  

- Baseline model → **Stacked LSTM + GRU + Dense layers**  
- Residual Hybrid Model → Adds **skip connections**, **normalization**, and **dropout** for improved stability and accuracy.  

<img width="971" height="689" alt="Architecture" src="https://github.com/user-attachments/assets/d1efc10b-dec6-485b-b0f4-0d28330fc2f6" />

---

## ⚙️ Algorithm Workflow  

<div align="center"> 
<img width="1273" height="747" alt="Workflow" src="https://github.com/user-attachments/assets/b47e08d3-2884-466e-8806-a108f8bbdde8" />
</div>  

---

## 📊 Results and Performance  

Comparison with baseline models:  

<div align="center">
<img width="655" height="198" alt="Results" src="https://github.com/user-attachments/assets/49db5e3c-e6e3-4701-a86c-172c51c03765" />
</div>  

- 📈 Residual Sequence Learning Model → **R² improved to 0.805** (vs. 0.52–0.62 baselines).  
- ⚡ MAE reduced by ~10%, MSE reduced by ~60%.  

---

## 🔭 Future Work  

- 🔹 **Multi-output Prediction** → Extend to other insulin types (NPH, UltraLente).  
- 🔹 **Reinforcement Learning Integration** → Adaptive dosage strategies based on real-time glucose response.  
- 🔹 **Attention/Transformers** → Enhance interpretability and time-step importance.  
- 🔹 **Cross-Dataset Testing** → Validate across additional diabetes datasets.  

---

## 📌 Final Hybrid Model  

The final hybrid LSTM-GRU model is available here:  
👉 [Hybrid Model Download](https://drive.google.com/file/d/10JspsXdBGk9TsfWnc3f7zO8Rk5nA15hW/view?usp=sharing)  

---
