🚗 AI-Based Vehicle Health Monitoring System using IoT Sensors
📌 Project Overview

The AI-Based Vehicle Health Monitoring System is an intelligent predictive maintenance solution that integrates IoT sensors, Machine Learning, Edge Processing, and Cloud Analytics to continuously monitor vehicle health in real time.

This system collects vehicle parameters such as engine temperature, vibration level, battery voltage, and fuel level, analyzes them using AI models, and generates:
🔍 Real-time fault detection
📊 Vehicle Health Index (VHI) score
⚠️ Predictive maintenance alerts
📈 Dashboard visualization
The system helps reduce sudden vehicle breakdowns, improves safety, and lowers maintenance costs.

🎯 Problem Statement
Traditional vehicle maintenance systems:
❌ Do not provide real-time monitoring
❌ Detect faults only after breakdown
❌ Use manual inspection
❌ Cause high repair cost
This project solves these problems using AI-driven predictive monitoring.

🏗️ System Architecture
IoT Sensors → ESP32 / API → Cloud Storage → AI Model → Dashboard + Alerts
Modules:
IoT Data Collection Module
Engine Temperature
Vibration Level
Battery Voltage
Fuel Level
Cloud Data Storage Module
SQLite database
Real-time storage
AI Analysis & Alert Module
Random Forest Classification
Fault Prediction
Vehicle Health Index (VHI)
Severity Classification
Remaining Useful Life (RUL)

🧠 Machine Learning Model
The system uses:
RandomForestClassifier for fault detection
Regression model for Remaining Useful Life (RUL)
Synthetic dataset generation for training
Fault Classes:
Label	Condition
0	Normal
1	Engine Overheating
2	Battery Issue
3	Abnormal Vibration

📊 Vehicle Health Index (VHI)
The Vehicle Health Index is a score from 0 to 100 calculated based on sensor conditions.
90 – 100 → Healthy
70 – 89 → Moderate
40 – 69 → Risk
0 – 39 → Critical

🛠️ Technologies Used
Programming
Python
Embedded C (for ESP32)
Backend
Flask
SQLite
Machine Learning
Scikit-learn
Pandas
NumPy
Joblib
Frontend
HTML
CSS
JavaScript
Chart.js
Hardware
ESP32 / Arduino
IoT Sensors

📂 Project Structure
vehicle_health_monitor/
│
├── app.py
├── model.py
├── database.py
├── train_model.py
├── utils.py
├── requirements.txt
│
├── templates/
│   └── dashboard.html
│
├── static/
│   ├── css/style.css
│   └── js/dashboard.js
│
└── dataset/
    └── synthetic_data.csv
🚀 Installation & Setup
1️⃣ Clone Repository
git clone https://github.com/YOUR_USERNAME/AI-Vehicle-Health-Monitoring-IoT.git
cd AI-Vehicle-Health-Monitoring-IoT
2️⃣ Install Dependencies
pip install -r requirements.txt
3️⃣ Train Model
python train_model.py
4️⃣ Run Application
python app.py

Open in browser:
http://127.0.0.1:5000
📡 API Example
POST Sensor Data
curl -X POST http://127.0.0.1:5000/api/sensor-data \
-H "Content-Type: application/json" \
-d '{
  "temperature": 95,
  "vibration": 1.5,
  "battery_voltage": 12.4,
  "fuel_level": 70
}'
Response:
{
  "prediction": "Normal",
  "vhi": 92,
  "severity": "Low",
  "rul_estimation": "120 hours",
  "alert": "No critical issue detected"
}
📈 Features
✔ Real-time sensor monitoring
✔ AI-based fault prediction
✔ Vehicle Health Index (VHI)
✔ Remaining Useful Life estimation
✔ Severity classification
✔ Alert logging system
✔ Interactive dashboard
✔ Cloud-ready architecture
✔ Scalable for fleet management

🔮 Future Enhancements
GPS tracking integration
CAN Bus direct integration
Deep Learning (LSTM) for time-series prediction
Fleet-wide analytics dashboard
Mobile application
OTA model updates

🎓 Academic Information
Course: 21CSP302L – Project
Branch: Information Technology
Institution: SRM Institute of Science & Technology, Tiruchirappalli

📜 License
This project is licensed under the MIT License.

