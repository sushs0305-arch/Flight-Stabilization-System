
# Arduino Nano Based Flight Stabilization System

A 2-axis flight stabilization system developed using **Arduino Nano**, **MPU6050**, **BMP280**, **SG90 Servo Motors**, and an **Active Buzzer**. The system measures orientation and altitude, computes stabilization angles, and drives servo motors to demonstrate basic flight stabilization.

---

##  Project Overview

This project demonstrates the working principles of a basic flight stabilization controller. The MPU6050 sensor measures the roll, pitch, and gyroscope-based yaw values, while the BMP280 measures atmospheric pressure to estimate altitude. Based on the measured orientation, servo motors are commanded to simulate stabilization, and a buzzer provides an alert when excessive tilt is detected.

---

##  Features

- Roll angle estimation
- Pitch angle estimation
- Gyroscope-based yaw estimation
- Altitude measurement using BMP280
- Two-axis servo stabilization
- Active buzzer warning
- Real-time Serial Monitor output
- Compact PCB-based hardware implementation

---

##  Hardware Components

- Arduino Nano
- MPU6050 (Accelerometer + Gyroscope)
- BMP280 (Pressure & Altitude Sensor)
- 2 × SG90 Servo Motors
- Active Buzzer
- PCB
- USB Cable
- Jumper Wires

---

##  Circuit Connections

| Component | Arduino Nano |
|-----------|--------------|
| MPU6050 SDA | A4 |
| MPU6050 SCL | A5 |
| BMP280 SDA | A4 |
| BMP280 SCL | A5 |
| Servo 1 Signal | D9 |
| Servo 2 Signal | D10 |
| Active Buzzer | D8 |
| VCC | 5V |
| GND | GND |

---

##  Working Principle

1. MPU6050 continuously measures acceleration and angular velocity.
2. Roll, pitch, and yaw values are calculated.
3. BMP280 estimates altitude from atmospheric pressure.
4. Servo motor positions are calculated from the measured orientation.
5. Servo motors simulate stabilization.
6. The buzzer activates when the tilt exceeds the predefined threshold.
7. All sensor values and servo positions are displayed on the Serial Monitor.

---

##  Project Images

## 📷 Project Gallery

<table>
<tr>
<td align="center">
<img src="images/pcb.jpeg" width="420"><br>
<b>PCB Assembly</b>
</td>

<td align="center">
<img src="images/flight_controller.jpg" width="420"><br>
<b>Working Model</b>
</td>
</tr>

<tr>
<td colspan="2" align="center">
<img src="images/controller.png" width="850"><br>
<b>Serial Monitor Output</b>
</td>
</tr>
</table>

##  Output

```text
Roll : -8.80°
Pitch : 15.83°
Yaw : 359.96°
Altitude : 749.25 m
Servo1 : 117°
Servo2 : 41°
```

---

##  Software Used

- Arduino IDE 2.x
- Embedded C++
- Wire Library
- MPU6050 Library
- Adafruit BMP280 Library
- Servo Library

---

##  Future Improvements

- GPS Integration
- Magnetometer for accurate yaw estimation
- PID tuning optimization
- ESC and Brushless Motor Control
- Wireless telemetry
- Battery monitoring
- OLED/LCD display

---

