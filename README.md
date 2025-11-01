# Wind Energy Prediction LSTM  
## Overview  
This project focuses on predicting wind energy generation using Long Short-Term Memory (LSTM) neural networks.  
By leveraging historical wind speed, weather, and turbine data, the model aims to fore­cast future energy output and support renewable energy scheduling decisions.

## Repository Structure  
Wind-Energy-Prediction-LSTM/
│── data/ # Raw & processed datasets
│ ├── wind_speed_data.csv
│ ├── turbine_output_data.csv
│ ├── feature_engineered_data.csv
│ └── …
│
│── notebooks/ # Jupyter notebooks illustrating the workflow
│ ├── data_preprocessing.ipynb
│ ├── modelling_lstm.ipynb
│ └── results_analysis.ipynb
│
│── scripts/ # Python scripts for key steps
│ ├── preprocess.py
│ ├── train_model.py
│ ├── evaluate_model.py
│ └── deploy_model.py
│
│── results/ # Model outputs, evaluation metrics & plots
│ ├── predictions_test_set.csv
│ ├── training_history.png
│ ├── performance_metrics.txt
│ └── …
│
│── README.md # ← You are here
│── requirements.txt # Python dependencies



## ⚙️ Workflow  
### 1. Data Preprocessing  
- Clean and merge raw wind speed, weather and turbine output datasets  
- Handle missing values and outliers  
- Feature-engineering (e.g., lag features, rolling averages of wind speed)  

### 2. Feature Engineering  
- Create new features: e.g., wind speed × turbine blade pitch angle, ambient temperature × wind speed  
- Normalize/scale numeric features  
- Encode categorical features (if any)  

### 3. Model Training (LSTM)  
- Design an LSTM architecture for time-series forecasting  
- Split data into training, validation and test sets  
- Train the model on historical sequences to predict future energy output  

### 4. Evaluation  
- Key metrics: RMSE (Root Mean Squared Error), MAE (Mean Absolute Error), R² (coefficient of determination)  
- Visualise predictions vs actual: line plots, residual plots  
- Save model, training history and evaluation reports  

## Key Results  
- Best achieved test R²: ~X.XX  
- Best achieved test RMSE: ~YY.YY  
- Notable feature importances: wind speed lag 3h, ambient temperature, turbine blade pitch angle  
- Sample optimal conditions: for wind speed ~12-15 m/s → predicted energy output ~ZZ.Z MW  

*(Replace the above with your actual results.)*

## How to Run  
1. Clone the repository  
```bash
git clone https://github.com/hasini3107/Wind-Energy-Prediction-LSTM.git  
cd Wind-Energy-Prediction-LSTM
 
