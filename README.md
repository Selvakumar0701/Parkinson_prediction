# Parkinson_prediction
# 🧠 IoMT-based Parkinson's Prediction with Edge AI + AWS Integration

This project presents a low-cost, AI-powered wearable system for early detection of Parkinson’s and neuro-muscular disorders using MAX30102, MPU6050, and ESP32. Edge inference is done using a TensorFlow Lite LSTM model, and abnormal conditions trigger local alerts and cloud actions via AWS.

## 🔗 Features
- Real-time vitals + motion monitoring (SpO₂, HR, tremor)
- Edge AI-based prediction (on-device)
- DF Player for audio guidance
- AWS IoT Core + Lambda for remote alerts
- Emergency notifications to caregivers

## ⚙️ Hardware
- ESP32
- MAX30102
- MPU6050
- DF Mini Player + speaker
- GSM (optional for fallback)
- 9V Battery + regulator

## ☁️ Cloud Components (AWS)
- AWS IoT Core: MQTT publish/subscribe
- AWS Lambda: Respond to alerts
- AWS SNS: Notify via SMS/email (optional)
- AWS DynamoDB: Store event logs (optional)

## 📦 Model
The `.tflite` model in `/model/` is trained on Parkinson’s motion/HR datasets using LSTM for time series anomaly prediction.

## 🛠 How to Use
1. Upload the ESP32 firmware (`firmware/esp32_wearable.ino`)
2. Configure AWS IoT Core & attach a certificate
3. Upload model to ESP32 flash
4. Play sample MP3 on condition alert

## 📡 Live Demo Coming Soon!
