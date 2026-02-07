# cgm-glucose-forecasting-lstm-gru
An end-to-end time-series forecasting pipeline using LSTM, GRU, and Random Forest ensemble learning to predict short-term blood glucose levels from CGM data.
#  CGM Blood Glucose Forecasting using Hybrid LSTM–GRU Ensemble

A hybrid deep learning and ensemble learning system for short-term blood glucose prediction using Continuous Glucose Monitoring (CGM) time-series data**.  
The project combines LSTM, GRU, and a Random Forest meta-learner to capture both long-term and short-term glucose patterns for accurate forecasting.

This work demonstrates how AI can enable **proactive diabetes monitoring** by predicting glucose trends before abnormal levels occur.

---

📌 Project Highlights
✔ Forecasts glucose values using CGM time-series data  
✔ Hybrid deep learning architecture (LSTM + GRU)  
✔ Ensemble learning via Random Forest meta-learner  
✔ Handles noisy real-world healthcare data  
✔ Achieves strong performance using RMSE & R² evaluation  

---
 🎯 Problem Statement
Continuous Glucose Monitoring generates large amounts of time-series data, but most monitoring systems react only after glucose levels become abnormal.  

This project aims to **predict future glucose values** using historical CGM data so corrective action can be taken earlier.

---

📂 Dataset
The project uses **AZT1D CGM dataset**, which contains:
- Real-world CGM readings
- Multiple Type-1 Diabetes subjects
- Weeks of glucose data per subject
- Natural noise and missing readings

---
 ⚙️ Pipeline Overview
The system follows this pipeline:

1. Load CGM time-series data
2. Timestamp parsing & chronological ordering
3. Resampling to 15-minute intervals
4. Missing value interpolation
5. CGM feature selection
6. MinMax normalization
7. Sliding window sequence creation
8. Train LSTM model
9. Train GRU model
10. Stack predictions
11. Random Forest meta-learning
12. Model evaluation & visualization

---
 Model Architecture
The system uses a stacked ensemble:

• LSTM captures long-term glucose patterns  
• GRU captures short-term fluctuations  
• Random Forest combines predictions to improve robustness  

This hybrid approach reduces prediction error compared to single models.

---

Evaluation Metrics
Performance evaluated using:

- RMSE (prediction error magnitude)
- R² Score (trend alignment)
- Actual vs predicted glucose visualization

---

 Tech Stack
- Python
- Pandas & NumPy
- TensorFlow / Keras
- Scikit-learn
- Matplotlib
- Google Colab

---

 Results
The hybrid ensemble model achieved:
- High R² values
- Low RMSE
- Stable glucose forecasting performance

Ensemble learning improved robustness across different subjects.

---

Challenges Addressed
- Noisy CGM sensor data
- Missing readings
- Subject variability
- Time-series consistency issues

---

Future Enhancements
- Multi-step glucose forecasting
- Personalized user models
- Real-time deployment
- Meal & insulin data integration
- Model optimization for wearable devices




## ⭐ Repository Structure

