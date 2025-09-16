# 🚗 Car Price Prediction  

An end-to-end machine learning project for predicting car prices based on various features such as manufacturer, model, year, mileage, engine specs, and more. The project combines **data preprocessing, feature engineering, multiple ML models, and a Streamlit web app** for real-time predictions.  

## 📌 Project Overview  
- **Goal**: Predict car prices using structured tabular data.  
- **Dataset**: Contains car attributes like brand, model, production year, mileage, fuel type, engine volume, gearbox type, drive wheels, color, airbags, and levy (tax).  
- **Tech Stack**:  
  - **Python** (pandas, NumPy, matplotlib, seaborn, scikit-learn, XGBoost, PyTorch)  
  - **Streamlit** for GUI/web app  
  - **Joblib & Pickle** for saving and loading models  

## 🛠️ Key Features  
- Comprehensive **EDA & visualization** (distribution plots, correlations, categorical/numerical feature analysis).  
- **Data preprocessing pipeline**:  
  - Cleaning invalid entries  
  - Handling missing values  
  - Outlier detection (IQR capping)  
  - Label encoding & feature scaling  
- **Models Implemented**:  
  - Linear Regression  
  - Polynomial Regression  
  - Support Vector Regression (SVR)  
  - XGBoost Regressor  
  - Decision Tree & Random Forest  
  - Neural Networks (PyTorch)  
  - **Stacking (meta-model with XGBoost)**  
- **Streamlit App** for interactive predictions.  

## 📊 Model Evaluation  
Each model was trained and evaluated using:  
- Mean Squared Error (MSE)  
- Mean Absolute Error (MAE)  
- R² Score  

The **Stacking approach (with XGBoost as meta-model)** showed the best performance among tested methods.  

## 🌐 Web Application  
The Streamlit app allows users to:  
- Input car details (manufacturer, model, mileage, etc.)  
- Get instant price predictions using the **trained XGBoost model**  
- Optionally test with mock predictions if the model files are missing  

### Run the app locally:
```bash
pip install -r requirements.txt
streamlit run app.py
