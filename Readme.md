# 🔌 SmartPlug: Multi-level Power Monitoring System

## 📖 Project Overview
**SmartPlug** is a multi-level energy monitoring system developed as part of the **The NEXGen 2025 – Energy Innovation Challenge**.

This project addresses a key issue in Vietnam: most small and medium-sized enterprises (SMEs) have not yet adopted effective energy-saving solutions. Instead of designing hardware from scratch, this project focuses on **system integration**, leveraging affordable, off-the-shelf IoT modules to build a reliable, scalable, and cost-efficient energy monitoring solution.

This project helped the team achieve **Top 11 Finalist** in The NEXGen 2025 competition.

---

## 🎥 Project Presentation

[![Watch the video]([https://img.youtube.com/vi/YOUR_VIDEO_ID/0.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID](https://www.youtube.com/watch?v=U9Njz0QgUYU))

> 📌 Click the image above to watch the full presentation on YouTube.

---

## ⚙️ System Architecture

The system is designed with a **two-level (multi-level) monitoring approach**:

### 1. Micro Level – Smart Power Outlet
Acts as a smart plug for monitoring individual devices.

- **Voltage & Current Measurement**
  - ACS712 current sensor  
  - ZMPT101B voltage sensor  

- **Safety Module**
  - DHT11 temperature sensor  
  - KY-019 relay module  
  - Automatically cuts off power in case of overload or overheating  

- **Energy Calculation**
  - Power consumption calculated using:  
    P = V × I × cos(φ)

---

### 2. Macro Level – Smart Main Panel
Monitors total system power consumption at the electrical panel.

- **Non-invasive Monitoring**
  - CT sensor (STC013) for safe measurement without rewiring  

- **Local Display**
  - 20x4 LCD (I2C interface) for real-time monitoring  

---

## 💻 Technologies Used

### Hardware
- ESP32-S3 microcontroller  
- Wi-Fi communication via MQTT / HTTP  
- OTA (Over-the-Air) firmware updates  

### Software
- Backend: Node.js  
- Frontend: React + TailwindCSS  
- Database: PostgreSQL  

### AI Integration
- AI Chatbot using OpenAI API for natural language control  
- Energy analysis with:
  - LSTM (time-series forecasting)  
  - K-means (usage pattern clustering)  

---

## 💰 Deployment Cost

Using modular components significantly reduces cost.

- Standard system includes:
  - 10 smart outlets  
  - 1 main panel  

**Estimated total cost: ~3,021,000 VND (~120 USD)**

---

## 🚀 Key Features

- Real-time monitoring (device-level & system-level)  
- Overload & overheating protection  
- Remote monitoring via web dashboard  
- AI-powered insights and control  
- Scalable and easy to deploy  
- Cost-optimized design  

---

## 👨‍💻 Team Members

- Hoàng – Project Manager  
- Hải – Hardware Engineer  
- Tiền – Software & AI Developer  

---

## 📌 Future Improvements

- Mobile application development  
- Advanced anomaly detection  
- Integration with renewable energy systems  
- Improved analytics dashboard  

---

## 📄 License
This project is developed for research and competition purposes. License details will be updated.
