# 🌊 Flood Early-Warning System

This project is a **rule-based flood alert system** that takes a city name and river level as input, fetches live rainfall data using the **OpenWeatherMap API**, and outputs a **binary flood alert (YES/NO)** based on pre-defined thresholds.

## 🚀 Objective

To design a lightweight, real-time, and explainable flood early-warning tool that works without AI or human judgment — using only real-world data and deterministic logic.

---

## 🧠 How It Works

### ✔ Inputs:
- `City Name`: Entered by the user.
- `River Level (%)`: Also entered manually (based on available data or field estimates).

### 🌐 Data Source:
- **Rainfall (1h)** from [OpenWeatherMap](https://openweathermap.org/api)

### ⚙️ Logic:
```cpp
if (rainfall > 200)
    Alert = YES;
else if (rainfall > 100 && riverLevel > 80)
    Alert = YES;
else
    Alert = NO;



