📦 LPG Monitoring System (IoT-Based Gas Level & Leak Detection)

🎯 Project Objectives

Monitor gas leakage and instantly alert the customer

Help the customer know when to replace the cylinder

Provide continuous gas level updates using IoT (no SIM card needed)

🧩 Problem Statement

Traditional LPG cylinders do not show remaining fuel level.
Existing solutions depend on GSM modules (require SIM cards) or manual checking.

This project provides an accurate, continuous, low-cost IoT solution using NodeMCU.

💡 Proposed Solution

A NodeMCU ESP8266 based IoT system that:

Detects LPG leaks using MQ-6

Measures weight using Load Cell + HX711

Displays information on LCD

Alerts with buzzer

Sends data to app/website (IoT)


Advantages

Accurate

Fast & reliable

No SIM required

Cost efficient

🧱 System Architecture (Block Diagram)

NodeMCU → Load Cell (HX711)
NodeMCU → MQ-6 Sensor
NodeMCU → Buzzer
NodeMCU → LCD Display
NodeMCU → Mobile/Web App


🔌 Circuit Implementation

Hardware used:

NodeMCU

Load Cell

HX711 Amplifier

MQ-6 Sensor

16×2 LCD

Buzzer


(Photos from the presentation can be added later)


---

📏 Load Cell Specifications

Range: 0–40 kg

Rated Output: 1.0 ± 0.1 mV/V

Non-linearity: 0.03%

Repeatability: 0.03%

Cable length: 18 cm



---

🧪 MQ-6 Specifications

Voltage: 5V

Detection: 100–10,000 ppm

High sensitivity to LPG/Propane



---

🛠️ Hardware Build

Prototype includes:

Mounted load cell

LPG sensor

LCD

NodeMCU

Calibration setup

Assembled circuit



---

🚀 Results

LPG detection working

Load cell successfully calibrated

Real-time LCD display

Fully functional prototype



⚠️ Limitations

Weight data affected by vibrations

Needs stable mounting

Internet required for IoT features



---

📚 References

(Include the research papers listed in your PPT)
