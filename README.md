# EV Charge Demand Prediction
This project predicts the future demand for electric vehicle (EV) charging using historical population data and forecasting models.

## 📁 Project Structure
📦 EV-Charge-Demand-Prediction/
├── EV_Vehicle_Charge_Demand_Prediction.ipynb   # Jupyter Notebook for data exploration and modeling
├── app.py                                      # Streamlit web application
├── requirements.txt                            # Required Python dependencies
├── Electric_Vehicle_Population_By_County.csv   # Raw dataset from Washington State
├── preprocessed_ev_data.csv                    # Cleaned and feature-engineered dataset
├── forecasting_ev_model.pkl                    # Trained ML model for forecasting
└── ev image.png                                # Project cover image
└── README.md  

📊 Dataset
Source: Electric vehicle population by county
File: Electric_Vehicle_Population_By_County.csv
Content: Contains EV registration data by geography and time, used for training the demand prediction model.

🧹 Preprocessing
Removed missing or duplicate records
Aggregated population data by time (monthly/yearly)
Saved as preprocessed_ev_data.csv 

🤖 Model
A time series forecasting model was trained to predict EV charging demand
The trained model is saved as: forecasting_ev_model.pkl

📈 Notebook Overview
EV_Vehicle_Charge_Demand_Prediction.ipynb includes:
Data loading and exploration
Data cleaning and preprocessing
Model training and forecasting
Visualizations of historical and predicted demand
Model export to .pkl
Data export to .csv

## Tools Used
- Python (Pandas, NumPy, Scikit-learn, etc.)
- Google Colab
- Jupyter Notebook

🚀 How to Run
1. Clone the repo:
  git clone https://github.com/2300033094/EV-Charge-Demand-Prediction.git
  cd EV-Charge-Demand-Prediction
2. Install Dependencies:
  pip install -r requirements.txt
3. Run the App:
   streamlit run app.py
Then open your browser and visit http://localhost:8501 (this link works only on your own machine after running the app).

** How It Works**
Uses historical EV registration data per county
Extracts features like:
Lag values
Rolling averages
Percent changes
Growth trends (slope)
Forecasts future EV totals using a regression model
Visualizes the cumulative adoption trend for user-selected counties

Install dependencies (e.g., pandas, matplotlib, joblib, sklearn/statsmodels)
Run the notebook step-by-step
The model and outputs will be generated in the working directory

## Author
Chebrolu Chaithanya Kumar (2300033094)
