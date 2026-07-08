# QUADCOPTER-FOR-HOTSPOT-DETECTION-IN-OVERHEAD-POWERLINES

> A low-cost autonomous quadcopter equipped with a thermal camera for real-time hotspot detection in overhead power transmission lines.

<p align="center">
  <img src="assets/images/drone.jpg" width="700">
</p>

---

## 📖 Overview

Power transmission lines are prone to faults caused by overheating, loose connections, corrosion, and mechanical wear. Traditional inspection methods are time-consuming, expensive, and dangerous for maintenance personnel.

This project presents a **drone-based thermal inspection system** that captures real-time thermal images of power transmission lines using an **MLX90640 thermal sensor** integrated with a **Raspberry Pi 4**. The drone is stabilized using a **Pixhawk 2.4.8 flight controller** and monitored through **Mission Planner**.

Unlike AI-based inspection systems, this prototype focuses on **manual real-time thermal monitoring**, making it lightweight, affordable, and suitable for educational and research purposes.

---

# 🎯 Objectives

- Detect thermal hotspots in power transmission lines.
- Reduce manual inspection risks.
- Perform real-time thermal monitoring.
- Build a low-cost UAV inspection platform.
- Demonstrate thermal anomaly detection using embedded systems.

---

# ✨ Features

- 🚁 Quadcopter-based inspection system
- 🌡️ Real-time thermal imaging
- 📡 Pixhawk flight controller
- 📍 GPS-based navigation
- 💻 Raspberry Pi onboard processing
- 📶 Live thermal visualization
- 🔥 Hotspot identification
- ⚡ Lightweight and low-cost design

---

# 🛠 Hardware Components

| Component | Description |
|------------|-------------|
| F450 Frame | Drone Frame |
| Pixhawk 2.4.8 | Flight Controller |
| Raspberry Pi 4 Model B | Companion Computer |
| MLX90640 BAB | Thermal Camera |
| A2212 1000KV BLDC Motors | Propulsion |
| 40A ESC | Motor Controller |
| 1045 Propellers | Lift Generation |
| Neo-M8N GPS | Positioning |
| FlySky FS-i6 | Remote Controller |
| Telemetry Module | Ground Communication |
| 3S LiPo Battery | Power Supply |

---

# 💻 Software Used

- Raspberry Pi OS
- Python
- Mission Planner
- Thonny IDE
- NumPy
- OpenCV
- Matplotlib
- Adafruit CircuitPython MLX90640 Library

---

# 🔌 System Architecture

```
            +----------------------+
            |  FlySky Transmitter  |
            +----------+-----------+
                       |
                       |
                +------+------+
                |  Pixhawk FC |
                +------+------+
                       |
      +----------------+----------------+
      |                                 |
      |                                 |
 GPS Module                     ESC + Motors
      |
      |
 Raspberry Pi 4
      |
      |
 MLX90640 Thermal Camera
      |
      |
 Thermal Image Processing
      |
      |
 Live Thermal Visualization
```

---

# 🔄 Workflow

```
Power ON
    │
    ▼
Initialize Pixhawk
    │
    ▼
GPS Lock
    │
    ▼
Drone Takeoff
    │
    ▼
Capture Thermal Data
    │
    ▼
Raspberry Pi Processing
    │
    ▼
Interpolation
    │
    ▼
Thermal Heatmap
    │
    ▼
Hotspot Detection
```

# 🔗 Sensor Connections

| MLX90640 | Raspberry Pi |
|-----------|--------------|
| VCC | 3.3V |
| GND | GND |
| SDA | GPIO2 (Pin 3) |
| SCL | GPIO3 (Pin 5) |

---

# 🚀 Flight Setup

Before flight:

- Accelerometer Calibration
- Compass Calibration
- ESC Calibration
- Radio Calibration
- Flight Mode Configuration
- GPS Lock (6–8 Satellites)
- Battery Check

---

# 📸 Results

### Thermal Image (Without Interpolation)

<p align="center">
<img src="assets/images/thermal_before.png" width="500">
</p>

---

### Thermal Image (With Interpolation)

<p align="center">
<img src="assets/images/thermal_after.png" width="500">
</p>

---

### Hotspot Detected

<p align="center">
<img src="assets/images/hotspot.png" width="500">
</p>

---

### Final Drone

<p align="center">
<img src="assets/images/drone.jpg" width="600">
</p>

---

# 📈 Future Improvements

- AI-based hotspot detection
- YOLO integration
- Autonomous waypoint inspection
- GPS location tagging
- RGB + Thermal image fusion
- Longer flight endurance
- Cloud-based monitoring dashboard

---

# 📚 References

- Pixhawk Documentation
- Mission Planner Documentation
- Raspberry Pi Documentation
- MLX90640 Datasheet
- ArduPilot Documentation

---

# 👩‍💻 Author

**Sudhiksha K**

Electronics and Communication Engineering

College of Engineering, Guindy

Anna University

---

