# 🧒🏻 Child Safety Wearable Device with IoT System

This project presents a **smart wearable device** designed to ensure **child safety** using GPS tracking, geofencing, and SMS alerts. The system provides real-time monitoring and sends emergency alerts if the child moves beyond a predefined safe zone.

---

## 🎯 Objective

- Ensure **child safety** using GPS-based real-time location tracking.
- Alert parents when a child exits a predefined **geofence zone**.
- Balance between **child independence** and **parental peace of mind**.
- Maintain **privacy and data security** in tracking operations.

---

## 🛠️ Features

- 📍 Real-time GPS location tracking
- 📲 Automatic SMS alerts with Google Maps link
- 📡 GSM module-based message delivery
- 🧭 Geofencing-based safety monitoring (up to 500m)
- 🔋 Battery-powered wearable device
- 🔁 Continuous monitoring with auto alert system

---

## 🧩 Hardware Components

| Component        | Description                            |
|------------------|----------------------------------------|
| Arduino Uno      | Main microcontroller                   |
| GSM Module       | Sends SMS alerts to parents            |
| GPS Module       | Tracks child's location                |
| Battery          | Powers the wearable device             |
| Breadboard       | For circuit connections                |
| Jumper Wires     | For component integration              |

---

## 💻 Software Components

- Arduino IDE
- Default SMS Application (on mobile)
- Embedded C/C++ Code (for Arduino)

---

## 🔁 System Workflow

1. 📶 **Initialization**: Device boots and connects to satellites and GSM network.
2. 🗺 **Geofence Setup**: Safe zone defined via lat/lon coordinates & max radius (default: 30m–500m).
3. 📡 **Location Tracking**: GPS updates location periodically.
4. 🚨 **Boundary Detection**: Compares GPS location with geofence.
5. ✉️ **Alert Generation**: On exit, sends SMS to predefined contact.
6. 🔄 **Continuous Monitoring**: Device loops through tracking logic.

---

## 🧠 Methodology

- GPS tracks live coordinates.
- Arduino processes distance from safe zone.
- GSM module sends an alert SMS like:  
  `"Alert! The Child is outside the fence. http://maps.google.com/maps?q=loc:LAT,LNG"`

---

