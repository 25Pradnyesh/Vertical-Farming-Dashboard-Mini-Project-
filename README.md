# 🌱 Vertical Farming Dashboard

> A modern frontend dashboard for monitoring and visualizing an AI + IoT powered vertical farming system.

![Next.js](https://img.shields.io/badge/Next.js-16-black?style=flat-square&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=flat-square&logo=typescript)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4-06B6D4?style=flat-square&logo=tailwindcss)
![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react)
![Recharts](https://img.shields.io/badge/Recharts-Data_Visualization-22C55E?style=flat-square)

## Overview

The **Vertical Farming Dashboard** is a frontend interface designed to visualize and monitor key environmental parameters in a smart vertical farming setup.

The dashboard provides a centralized view of:

- 🌡️ Temperature
- 💧 Humidity
- 🌱 Soil Moisture
- 🧪 Soil pH
- ⚡ TDS
- 💦 Water Pump Status
- 📊 Real-time sensor trends
- 🚨 Farming alerts
- 📡 Sensor health
- 🧠 AI disease detection interface

The current version is focused on the **frontend experience**. Sensor readings are simulated locally so the dashboard can run without requiring an external IoT device, Firebase project, or backend server.

---

## ✨ Features

### 📊 Dashboard

A centralized overview of the vertical farming environment with real-time-looking sensor values and system status.

### 🌡️ Environmental Monitoring

The dashboard displays:

| Parameter     | Unit |
| ------------- | ---- |
| Temperature   | °C   |
| Humidity      | %    |
| Soil Moisture | %    |
| Soil pH       | pH   |
| TDS           | ppm  |

Sensor values are simulated and automatically updated during development.

### 📈 Real-Time Data Visualization

Interactive charts visualize changes in:

- Temperature
- Humidity
- Soil Moisture
- pH
- TDS

The chart continuously receives new simulated readings to demonstrate the intended real-time monitoring experience.

### 🚨 Smart Alerts

The dashboard evaluates sensor values and displays alerts when parameters move outside defined ranges.

Examples include:

- Low soil moisture
- Abnormal pH
- High temperature
- Normal operating conditions

### 📡 Sensor Status

Displays the operational status of the connected sensor categories:

- Temperature & Humidity
- Soil Moisture
- pH
- TDS

### 🧠 AI Disease Detection Interface

The dashboard includes a dedicated interface for plant disease detection with:

- Plant image preview
- Disease classification display
- Confidence score
- Recommendations
- Analysis workflow

The current frontend version demonstrates the interface without requiring the complete AI inference backend.

### 💦 Water Pump Monitoring

Displays the current simulated water pump state:

- Running
- Stopped

---

## 🖥️ Dashboard Navigation

The sidebar provides access to:

```text
Dashboard
Live Data
Sensors
AI Detection
Alerts
```

Each section presents a different part of the farming monitoring system.

---

## 🛠️ Tech Stack

### Frontend

- **Next.js 16**
- **React**
- **TypeScript**
- **Tailwind CSS**
- **Lucide React**
- **Recharts**

### Development

- Node.js
- npm
- Git
- VS Code

---

## 📁 Project Structure

```text
Vertical-Farming-Dashboard-Mini-Project-
│
├── app/
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
│
├── components/
│   ├── dashboard/
│   │   ├── AIDiseaseDetection.tsx
│   │   ├── KPICard.tsx
│   │   ├── RealTimeChart.tsx
│   │   ├── RecentAlerts.tsx
│   │   └── SensorStatus.tsx
│   │
│   └── layout/
│       ├── Sidebar.tsx
│       └── TopNavbar.tsx
│
├── public/
│   └── leaf.jpg
│
├── package.json
├── next.config.ts
├── tsconfig.json
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/25Pradnyesh/Vertical-Farming-Dashboard-Mini-Project-.git
```

### 2. Enter the project

```bash
cd Vertical-Farming-Dashboard-Mini-Project-
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm run dev
```

### 5. Open the dashboard

Visit:

```text
http://localhost:3000
```

---

## 🧪 Current Development Mode

The current frontend uses **simulated sensor data** rather than a live IoT/Firebase connection.

This allows the complete dashboard interface to be demonstrated locally without requiring:

- ESP32 hardware
- Firebase credentials
- A database
- An external API
- A backend server

The simulated values update automatically to demonstrate the real-time monitoring experience.

---

## 🔮 Future Integration

The frontend architecture can later be connected to a real IoT infrastructure.

A potential production architecture:

```text
Sensors
   │
   ▼
ESP32 / IoT Controller
   │
   ▼
Database / API
   │
   ▼
Backend
   │
   ├───────────────┐
   ▼               ▼
Sensor Data      AI Model
   │               │
   └───────┬───────┘
           ▼
   Vertical Farming
       Dashboard
```

Possible future integrations include:

- ESP32 sensor network
- Firebase Realtime Database
- Real-time IoT telemetry
- Automated irrigation
- Plant disease detection models
- AI-powered recommendations
- Historical sensor analytics
- Authentication
- Multi-farm monitoring

---

## 🎯 Project Goal

The goal of this project is to create a clean and intuitive monitoring interface for smart vertical farming systems.

Instead of requiring farmers or operators to inspect individual sensor readings, the dashboard brings the important information into a single interface that makes environmental conditions, alerts, and system status easy to understand.

---

## 👨‍💻 Built By

**Pradnyesh**

Engineering student & developer building projects across AI, IoT, Web3 and modern web technologies.

### Connect

- GitHub: [@25Pradnyesh](https://github.com/25Pradnyesh)
- X: [@Pradnyesh_25](https://x.com/Pradnyesh_25)

---

## 📄 License

This project is available for educational and demonstration purposes.
