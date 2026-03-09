# 🚗 AI-Based Multi-Vehicle Health Monitoring System

An intelligent web-based system that monitors vehicle health using simulated IoT sensor data and AI-based fault prediction. The system analyzes parameters such as temperature, vibration, battery voltage, and fuel level to determine vehicle condition and predict potential faults.

---

## 📌 Features

* Real-time vehicle health monitoring
* AI-based fault detection
* Vehicle Health Index (VHI) calculation
* Fault severity classification
* Remaining Useful Life estimation
* Multi-vehicle monitoring dashboard
* Interactive charts for sensor data
* Export vehicle data as CSV

---

## 🧠 AI Capabilities

The system uses machine learning models to analyze sensor patterns and predict vehicle faults such as:

* Normal condition
* Engine overheating
* Battery issues
* Abnormal vibration

Based on the prediction, the system assigns:

* Fault status
* Severity level
* Estimated remaining useful life

---

## 📊 Parameters Monitored

The system monitors the following simulated IoT sensor data:

* Temperature (°C)
* Vibration (g-force)
* Battery Voltage (V)
* Fuel Level (%)

These parameters are used to calculate the **Vehicle Health Index (VHI)** and detect abnormal conditions.

---

## 🛠️ Technologies Used

* **Python**
* **Flask**
* **Machine Learning (Scikit-learn)**
* **HTML / CSS / JavaScript**
* **Chart.js**
* **SQLite Database**

---

## 📁 Project Structure

```
vehicle_health_monitor/
│
├── app.py                 # Main Flask application
├── model.py               # AI model logic
├── train_model.py         # Model training script
├── sensor_simulator.py    # Simulated IoT data generator
├── database.py            # Database setup
│
├── templates/
│   └── dashboard.html     # Frontend dashboard
│
├── static/                # CSS / JS / assets
│
├── vehicle_health.db      # SQLite database
└── README.md
```

---



## 📷 Dashboard

The dashboard displays:

* Vehicle Health Index
* Fault status
* Severity level
* Remaining useful life
* Sensor data charts

---

## 🎯 Use Cases

* Smart vehicle maintenance
* Fleet monitoring systems
* Predictive maintenance solutions
* IoT-based automotive analytics

---

## 📄 License

This project is open-source and available under the MIT License.
