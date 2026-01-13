# AI Indoor Air Quality Health Predictor

## What are you going to build?

I am building an AI-powered indoor air quality monitoring and health prediction system using a Raspberry Pi. The system continuously measures indoor environmental conditions and uses edge AI to predict potential health effects such as fatigue, headaches, poor sleep quality, and respiratory discomfort. Unlike traditional monitors, this project focuses on actionable health insights, not just raw sensor data.

## How does your solution work? What are the main features?

The Raspberry Pi collects real-time data from multiple air quality and environmental sensors. This data is processed locally using a lightweight machine learning model combined with health-based inference rules.

### Main features include:

- Real-time monitoring of CO₂, particulate matter (PM2.5), temperature, humidity, and VOC levels

- AI-based prediction of health impacts based on exposure level and duration

- Trend analysis instead of single-value alerts

- Visual dashboard with easy-to-understand health indicators

- Local (offline) processing for privacy and low latency

 - Actionable recommendations such as improving ventilation or adjusting humidity

## 🧰 Hardware Stack (BOM)

### Core Components
- Raspberry Pi 5 (or Raspberry Pi 4)
- Air Quality Sensors:
   - CO₂ sensor (e.g., MH-Z19B or SCD40)
   - PM2.5 sensor (e.g., PMS5003)
   - Temperature & Humidity sensor (e.g., BME280)
   - VOC / gas sensor (e.g., SGP30 or CCS811)

### Optional
- Small display or HDMI monitor
- Speaker for alerts
- Enclosure for wall-mount or desktop use

Estimated Cost: ~$120–$150

## 💻 Software Stack
- Raspberry Pi OS (64-bit)
- Python
- OpenCV (optional, for future CV expansion)
- NumPy / Pandas (data processing)
- TensorFlow Lite or Scikit-learn (ML inference)
- Flask or Streamlit (dashboard UI)
- SQLite or CSV logging for historical analysis

## 🧪 AI & Health Prediction Logic
The AI component learns from:
- Sensor combinations (e.g., high CO₂ + low humidity)
- Exposure duration (e.g., CO₂ > 1200 ppm for 2+ hours)
- Time-of-day patterns (sleep vs daytime)

Example predictions:
- High CO₂ + long exposure → fatigue / poor concentration
- High PM2.5 → respiratory irritation risk
- Low humidity → dry throat, poor sleep
- High VOCs → headache probability

This transforms raw data into **human-centric insights**, which is what makes the project innovative.
