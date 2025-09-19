🩺 Personalized Insulin Dosage Prediction Using Hybrid LSTM–GRU
🚀 Project Overview

This project proposes a Hybrid Deep Learning Framework for predicting personalized insulin dosages in diabetic patients. By combining LSTM and GRU layers with residual learning, the model captures both short-term glucose fluctuations and long-term physiological patterns.

The system processes the AIM94 diabetes dataset, performing advanced preprocessing and temporal feature engineering to transform irregular event logs into structured time-series suitable for deep learning models.

🔑 Key Highlights

🧩 Residual Hybrid Architecture → LSTM + GRU with skip connections for stable and efficient learning.

🛠️ Advanced Preprocessing → Converts raw event-based records into structured multivariate time series.

⏳ Sliding Window Modeling → Generates input-output sequences to forecast the next insulin dose.

📈 Superior Performance → Achieved R² = 0.805, MAE = 1.29, and MSE = 3.27 — a significant improvement over baselines.

🎯 Objectives

Predict regular insulin dosage with high accuracy using patient history.

Encode temporal dependencies in glucose–insulin interactions.

Develop a scalable framework for clinical decision support in diabetes care.

Explore hybrid recurrent architectures for biomedical sequence modeling.

🧪 Preprocessing Pipeline

The data preprocessing transforms raw medical logs into time-series suitable for modeling. Steps include:

Data Cleaning → Handle missing values, standardize timestamps, and filter irrelevant codes.

Event Pivoting → Expand event logs into structured features:

Glucose values

Insulin dosages (Regular, NPH, UltraLente)

Food intake

Hypoglycemia events

Exercise logs

Feature Engineering →

Cyclical encoding of time-of-day (sine/cosine transformation)

Lag features for past glucose/insulin levels

Temporal markers (morning, afternoon, night)

Binary indicators for events (food, activity, symptoms)

Sequence Generation → Sliding windows create patient sequences for supervised learning.

Normalization → Min–Max scaling ensures stable convergence during training.

🔄 Data Transformation Example
<div align="center">
Raw Event Log	→	Processed Time-Series Data

		
</div>
🏗️ Model Architecture

The Hybrid Residual Model consists of:

Stacked LSTM and GRU layers

Residual skip connections for improved gradient flow

Batch Normalization & Dropout to prevent overfitting

Dense layers for final regression output

<div align="center"> <img src="https://github.com/user-attachments/assets/d1efc10b-dec6-485b-b0f4-0d28330fc2f6" width="720"/> </div>
⚙️ Algorithm Workflow
<div align="center"> <img src="https://github.com/user-attachments/assets/b47e08d3-2884-466e-8806-a108f8bbdde8" width="850"/> </div>
📊 Results & Evaluation

Performance comparison against baseline models:

<div align="center"> <img src="https://github.com/user-attachments/assets/49db5e3c-e6e3-4701-a86c-172c51c03765" width="600"/> </div>

R² Score: 0.805 (↑ 30% vs. baselines)

MAE: 1.29 (↓ 10%)

MSE: 3.27 (↓ 60%)

🔭 Future Enhancements

🔄 Multi-output prediction → Extend framework for NPH & UltraLente insulin types.

🤖 Reinforcement Learning Integration → Adaptive dosage adjustment based on glucose trends.

🎯 Attention/Transformers → Improve interpretability by focusing on critical time steps.

🌐 Cross-dataset validation → Evaluate robustness across multiple diabetes datasets.

📌 Final Hybrid Model

The trained model integrating LSTM + GRU with residual connections is available here:
👉 Download Hybrid Model

✨ This project demonstrates how hybrid deep learning models can enhance personalized healthcare, supporting clinicians in precise insulin dosage recommendations.
