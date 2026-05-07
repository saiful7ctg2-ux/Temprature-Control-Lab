# 🌡️ Real-Time Temperature Control & Monitoring System

A PI-based temperature control system with OPC UA communication and a real-time Node-RED monitoring dashboard, built on an ApMonitor-based temperature control lab.

---

## 📌 Project Overview

This project implements a closed-loop **PI control system** for real-time temperature regulation. The system integrates industrial communication protocols and a live monitoring interface, simulating a real Industry 4.0 automation environment.

---

## 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| Control Design | MATLAB / Simulink |
| Process Simulation | ApMonitor Temperature Control Lab (TCLab) |
| Industrial Communication | OPC UA (UaModeler, UaExpert) |
| Monitoring Dashboard | Node-RED |
| Programming | MATLAB |

---

## ⚙️ System Architecture

```
[TCLab Plant]
     │
     ▼
[MATLAB/Simulink - PI Controller]
     │
     ▼
[OPC UA Server - UaModeler]
     │
     ▼
[Node-RED Dashboard - Real-Time Monitoring]
```

---

## 🔬 Key Features

- ✅ **PI Controller** designed and tuned in MATLAB/Simulink for stable temperature regulation
- ✅ **OPC UA Integration** for standardized, secure industrial data communication
- ✅ **Real-Time Dashboard** built in Node-RED displaying live temperature, setpoint, and control output
- ✅ **ApMonitor TCLab** used as the physical/simulated plant for realistic process behavior
- ✅ Fully aligned with **Industry 4.0** automation and IIoT standards

---


## 🚀 Getting Started

### Prerequisites

- MATLAB / Simulink installed
- [TCLab Python package](https://apmonitor.com/pdc/index.php/Main/ArduinoTemperatureControl) installed:
  ```bash
  pip install tclab
  ```
- [UaModeler](https://www.unified-automation.com/products/development-tools/uamodeler.html) for OPC UA server
- [Node-RED](https://nodered.org/) installed:
  ```bash
  npm install -g --unsafe-perm node-red
  ```

### Running the Project

1. **Start the OPC UA server** using UaModeler with the provided config
2. **Run the MATLAB script** or open the Simulink model and start simulation
3. **Launch Node-RED** and import the `dashboard_flow.json` file
4. Open the dashboard at `http://localhost:1880/ui`

---

## 📊 Results

- Achieved stable temperature tracking with minimal steady-state error
- Real-time data visible on the Node-RED dashboard with < 1s latency via OPC UA
- System successfully demonstrates closed-loop control in an IIoT-compatible architecture

---



## 📄 License

This project is for academic and portfolio purposes.
