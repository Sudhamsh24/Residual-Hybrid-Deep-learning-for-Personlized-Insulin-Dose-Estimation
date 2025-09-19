🩺 Personalized Insulin Dosage Prediction Using Hybrid LSTM–GRU
🚀 Project Overview

This project introduces a Hybrid Deep Learning Framework for predicting personalized insulin dosages in diabetic patients.
By combining LSTM and GRU layers with residual learning, the model captures both short-term glucose fluctuations and long-term physiological patterns.

The model processes the AIM94 dataset, applying advanced preprocessing and temporal feature engineering to transform irregular event logs into structured time-series suitable for deep learning.

🔑 Key Highlights

🧩 Residual Hybrid Architecture → LSTM + GRU with skip connections for stable and efficient learning.

🛠️ Advanced Preprocessing → Converts raw event-based records into structured multivariate time series.

⏳ Sliding Window Modeling → Generates sequences to forecast insulin dosage.

📈 Superior Performance → Achieved R² = 0.805, MAE = 1.29, and MSE = 3.27, improving accuracy significantly compared to baselines.

🎯 Objectives

Predict regular insulin dosage with high accuracy.

Model temporal dependencies in glucose–insulin interactions.

Provide a scalable decision-support tool for diabetes management.

Explore hybrid architectures in biomedical time-series modeling.

🧪 Preprocessing Pipeline

Steps followed to prepare the dataset:

Data Cleaning → Remove missing/irrelevant entries and standardize timestamps.

Event Pivoting → Structure data into columns like:

Glucose readings

Insulin doses (Regular, NPH, UltraLente)

Food intake

Hypoglycemia events

Exercise

Feature Engineering →

Cyclical encoding for time-of-day (sine/cosine)

Lag features for past glucose/insulin values

Temporal indicators (morning/evening/night)

Binary event flags

Sequence Generation → Create input sequences via sliding windows.

Normalization → Apply Min–Max scaling for faster convergence.

🔄 Data Transformation Example
<div align="center">
Raw Event Log	→	Processed Time-Series Data

		
</div>
🏗️ Model Architecture

The Hybrid Residual Model includes:

Stacked LSTM and GRU layers

Residual skip connections for stable gradient flow

Batch Normalization and Dropout

Dense output layers

<div align="center"> <img src="https://github.com/user-attachments/assets/d1efc10b-DEC6-485b-b0f4-0d28330fc2f6" width="720"/> </div>
⚙️ Algorithm Workflow
<div align="center"> <img src="https://github.com/user-attachments/assets/b47e08d3-2884-466e-8806-a108f8bbdde8" width="850"/> </div>
📊 Results & Evaluation

Comparison with baseline models:

<div align="center"> <img src="https://github.com/user-attachments/assets/49db5e3c-e6e3-4701-a86c-172c51c03765" width="600"/> </div>

R² Score: 0.805 (↑ 30% vs. baselines)

MAE: 1.29 (↓ 10%)

MSE: 3.27 (↓ 60%)

🔭 Future Work

🔄 Extend prediction to NPH and UltraLente insulin.

🤖 Add Reinforcement Learning for adaptive dosage adjustment.

🎯 Use Attention/Transformers for better interpretability.

🌐 Validate across multiple diabetes datasets.

📌 Final Hybrid Model

The final trained model is available here:
👉 Download Hybrid Model

✨ This project shows how hybrid deep learning can advance personalized healthcare by supporting clinicians in precise insulin dosage prediction.
