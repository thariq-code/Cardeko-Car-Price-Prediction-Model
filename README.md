🚗 Car Price Prediction Model

A Machine Learning web application that predicts the selling price of a used car based on various vehicle specifications such as age, kilometers driven, mileage, engine capacity, power, fuel type, seller type, and transmission type. The model is deployed using Flask and provides predictions through a user-friendly web interface.

📌 Project Overview

The objective of this project is to build a machine learning model capable of estimating the resale value of a car using historical vehicle data. The application helps users get an approximate market price for a used vehicle by entering its details through a web form.

🚀 Features
Predicts used car selling price instantly
Interactive web interface built with HTML & CSS
Flask-based backend
Machine Learning regression model
Supports multiple vehicle attributes
Easy deployment and usage
🛠️ Technologies Used
Frontend
HTML5
CSS3
Backend
Python
Flask
Libraries
NumPy
Pandas
Scikit-learn
Pickle
Machine Learning
Random Forest Regressor
📊 Dataset Features

The model uses the following input features:

Feature	Description
Vehicle Age	Age of the car in years
Kilometers Driven	Total distance traveled
Mileage	Fuel efficiency (km/l)
Engine	Engine capacity (CC)
Max Power	Maximum power output (BHP)
Seats	Number of seats
Seller Type	Dealer / Individual / Trustmark Dealer
Fuel Type	Petrol / Diesel / CNG / LPG / Electric
Transmission Type	Manual / Automatic
📂 Project Structure
Car-Price-Prediction/
│
├── app.py
├── best_model.pkl
├── templates/
│   └── index.html
│
├── notebooks/
│   └── Project_Cardeko_Car_Price_Prediction.ipynb
│
├── requirements.txt
├── README.md
└── dataset.csv
⚙️ Installation
1. Clone Repository
git clone https://github.com/your-username/car-price-prediction.git
cd car-price-prediction
2. Create Virtual Environment
python -m venv venv
3. Activate Environment

Windows:

venv\Scripts\activate

Linux/Mac:

source venv/bin/activate
4. Install Dependencies
pip install -r requirements.txt
▶️ Run the Application
python app.py

Open browser:

http://localhost:8001
🧠 Machine Learning Workflow
Data Collection
Data Cleaning
Feature Engineering
Data Preprocessing
Train-Test Split
Model Training
Model Evaluation
Model Serialization using Pickle
Flask Deployment
📈 Model Evaluation Metrics

The model performance was evaluated using:

R² Score
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
💡 Future Improvements
Add car brand and model selection
Deploy on cloud platforms
Improve UI/UX design
Add image-based car analysis
Real-time market value integration
👨‍💻 Developed By

Thariq Arsath

B.Tech Artificial Intelligence and Machine Learning

📜 License

This project is developed for educational and learning purposes. Feel free to use and modify it for academic projects.

⭐ If you found this project useful, don't forget to star the repository! 🚀
