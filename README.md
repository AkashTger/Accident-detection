# 🪖 SMART HELMET – Vehicular Safety Monitoring System

## 📌 Overview
The **SMART HELMET** project is an intelligent vehicular safety system designed to reduce road accidents and enhance driver safety. It integrates multiple sensors and real-time monitoring to detect driver impairment, monitor vehicle dynamics, and send instant alerts using a Telegram bot.

---

## 🚀 Key Features
- 🍺 Alcohol Detection (Prevents drunk driving)
- 📉 Accelerometer-based Accident Detection
- 📍 Real-time GPS Location Tracking
- 🤖 Telegram Bot Alerts & Remote Control
- 📟 LCD Display for live system feedback
- 🔔 Buzzer Alerts
- ⚙️ Motor Relay Control (Engine lock/unlock)

---

## 🧠 Abstract
This project presents an advanced safety system using embedded sensors like accelerometers, alcohol sensors, and GPS modules. It continuously monitors driver behavior and vehicle conditions to detect accidents and impairment. Upon detecting anomalies, it sends alerts via Telegram with location details, enabling quick response and preventive action.

---

## ❗ Problem Statement
- Drunk driving leading to fatal accidents
- No early accident detection systems in conventional vehicles
- Lack of real-time alerting and remote monitoring

---

## 💡 Solution
A smart helmet system that:
- Detects alcohol levels before ignition
- Monitors sudden movements to identify accidents
- Sends GPS-based alerts via Telegram
- Prevents vehicle ignition in unsafe conditions

---

## 🛠️ Hardware Components
- Arduino / ESP32 Microcontroller
- MQ-3 / MQ-9 Alcohol Sensor
- ADXL345 Accelerometer
- Neo-6M GPS Module
- 16x2 LCD Display
- Buzzer
- Motor Relay Module
- Push Button
- Resistors, Wires, Breadboard
- Power Supply / Battery

---

## 💻 Software Tools
- Arduino IDE
- ESP32 Board Package

### Libraries Used
- `LiquidCrystal`
- `Adafruit_Sensor`
- `Adafruit_ADXL345_U`
- `TinyGPS`
- `WiFi`
- `UniversalTelegramBot`
- `ArduinoJson`

---

## ⚙️ System Functionality

### 1. System Initialization
- Displays **WELCOME** on LCD
- Initializes all sensors
- Waits for alcohol sensor calibration

### 2. Driver Impairment Detection
- Reads alcohol level on button press
- If above threshold:
  - Activates buzzer
  - Disables motor (engine lock)

### 3. Accident Detection
- Uses accelerometer (X/Y axis)
- Detects sudden impact or abnormal motion
- Triggers alarm and stops vehicle

### 4. Telegram Alerts
- Sends accident and alcohol alerts
- Shares GPS location via Google Maps link
- Supports remote commands

---

## 🤖 Telegram Bot Integration
- 📩 Sends real-time alerts with location
- 🔐 Authorized user access using `CHAT_ID`
- ⚡ Commands supported:
  - `/led_on`
  - `/led_off`
  - `/state`

---

## 🧾 Code Structure

### Arduino Code
- Initializes sensors and LCD
- Reads alcohol levels
- Detects acceleration anomalies
- Sends serial data to ESP32

### ESP32 Code
- Connects to Wi-Fi
- Handles Telegram bot communication
- Sends alerts and GPS data
- Processes commands and controls GPIO

---

## 🔮 Future Enhancements
- 📡 GSM module for SMS alerts (no internet dependency)
- 🧪 Advanced electrochemical alcohol sensors
- 🗣️ Voice alerts and emergency calling
- ☁️ Cloud integration (Firebase / Blynk)
- 🆘 SOS emergency button

---

## 📚 References
1. Muhammad Ahmad Baballe (2022) – Accident Detection Systems  
2. Bruno Fernandes et al. (2016) – Multi-modal ITS Alert Systems  
3. Akshay Agrawal et al. (2013) – Accident Detection Application  
4. Vaishali Shrivastava et al. (2020) – Accident Detection Review  

---

## 📄 License
This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute this project.

---

## 🙌 Contribution
Pull requests are welcome. For major changes, open an issue first to discuss improvements.

---

## 📬 Contact
For queries or collaboration, feel free to reach out.
