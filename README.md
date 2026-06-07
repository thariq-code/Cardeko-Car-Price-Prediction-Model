Car Price Prediction Model
1. Project Introduction

This project predicts the selling price of a used car using Machine Learning. The model is trained on historical car data containing vehicle specifications and selling prices. A Flask web application is developed to allow users to enter car details and receive a predicted selling price instantly.

The project demonstrates:

Data preprocessing
Feature engineering
Model training
Model evaluation
Deployment using Flask
2. Dataset Information
Dataset Source

CarDekho Used Car Dataset

Features Used
Feature	Description
vehicle_age	Age of the vehicle
km_driven	Total kilometers driven
mileage	Mileage of the car
engine	Engine capacity (CC)
max_power	Maximum power (BHP)
seats	Number of seats
seller_type	Dealer / Individual / Trustmark Dealer
fuel_type	Petrol / Diesel / CNG / LPG / Electric
transmission_type	Manual / Automatic
Target Variable
selling_price
3. Data Preprocessing

The following preprocessing steps were performed:

Data Cleaning
Removed null values
Removed duplicate records
Converted categorical variables into numerical form
Feature Engineering

Categorical features were converted using One-Hot Encoding:

Seller Type
Dealer
Individual
Trustmark Dealer
Fuel Type
Petrol
Diesel
CNG
LPG
Electric
Transmission Type
Manual
Automatic
Feature Selection

Selected features:

vehicle_age
km_driven
mileage
engine
max_power
seats
seller_type
fuel_type
transmission_type
4. Machine Learning Models

The following regression algorithms were tested:

Linear Regression
Decision Tree Regressor
Random Forest Regressor
Extra Trees Regressor
Best Model

Random Forest Regressor was selected because it achieved the highest prediction accuracy and lowest prediction error.

5. Model Evaluation

The dataset was split into:

Training Data: 80%
Testing Data: 20%

Evaluation Metrics:

R² Score

Measures how well the model explains variance in the target variable.

Formula:

R² = 1 - (SSR / SST)

RMSE (Root Mean Squared Error)

Measures prediction error.

Formula:

RMSE = √(Σ(y - ŷ)² / n)

MAE (Mean Absolute Error)

Average absolute difference between actual and predicted values.

6. Flask Web Application

The trained model was saved using Pickle and deployed through Flask.

Workflow
User enters car details.
Flask receives input.
Input is converted into feature vector.
Trained model predicts price.
Predicted price is displayed on webpage.
7. Project Structure
Car-Price-Prediction/
│
├── app.py
├── best_model.pkl
├── requirements.txt
├── README.md
│
├── templates/
│   └── index.html
│
├── notebook/
│   └── Car_Price_Prediction.ipynb
│
└── dataset/
    └── car_data.csv
8. Installation and Setup
Clone Repository
git clone https://github.com/yourusername/car-price-prediction.git
Install Dependencies
pip install -r requirements.txt
Run Application
python app.py

Open browser:

http://localhost:8001
9. Results
Model Performance
Metric	Value
R² Score	(Your Value)
RMSE	(Your Value)
MAE	(Your Value)
Example Prediction

Input:

Vehicle Age = 7
KM Driven = 73000
Mileage = 16.47
Engine = 1198
Max Power = 74
Seats = 5
Fuel = Petrol
Transmission = Manual

Predicted Price:

₹5,48,790
10. Key Findings
Vehicle age significantly impacts resale value.
Cars with lower kilometers driven generally have higher prices.
Diesel vehicles tend to have higher resale value in certain segments.
Engine capacity and maximum power strongly influence selling price.
Automatic transmission vehicles often command higher prices.
11. Future Enhancements
Hyperparameter tuning using GridSearchCV.
Use XGBoost and LightGBM models.
Add car brand and model information.
Deploy application on Render or AWS.
Create responsive UI with Bootstrap.
Add graphical analytics dashboard.
12. Technologies Used
Python
Pandas
NumPy
Scikit-Learn
Matplotlib
Seaborn
Flask
HTML/CSS
Pickle