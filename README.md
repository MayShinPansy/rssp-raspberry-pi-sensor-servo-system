# RSSP: Raspberry Pi Sensor and Servo Control System

This project was developed for the **Robotics, Sensors and Signal Processing (RSSP)** module. It demonstrates an embedded system using a Raspberry Pi to integrate multiple sensors and actuators for real-time control and feedback.

---

## 📌 Project Overview

The system combines sensing, signal processing, and actuation to create an interactive control system.

The Raspberry Pi reads input from a potentiometer and ultrasonic sensor, processes the signals, and controls a servo motor and LEDs accordingly.

---

## ⚙️ Features

* 🎚️ Potentiometer controls servo angle
* 📡 Ultrasonic sensor detects distance (obstacle detection)
* 🔴 LED turns ON when object is too close
* 🟢 LEDs indicate servo position range
* 🔁 Limit switch allows system reset/restart
* ⚡ Real-time signal processing using Python

---

## 🧠 System Workflow

1. Potentiometer value is read via MCP3008 (SPI)
2. Value is mapped to servo angle (0–180°)
3. Ultrasonic sensor measures distance
4. If object is too close:

   * Warning LED turns ON
5. LEDs indicate servo angle range
6. Limit switch resets system when pressed

---

## 🧰 Hardware Components

* Raspberry Pi
* Servo Motor
* Ultrasonic Sensor (HC-SR04)
* Potentiometer
* MCP3008 ADC
* LEDs (Red / Green)
* Limit Switch
* Breadboard & Jumper Wires

---

## 💻 Software & Libraries

* Python 3
* RPi.GPIO
* spidev
* NumPy
* asyncio

---

## ▶️ How to Run

1. Enable SPI on Raspberry Pi
2. Install dependencies:

```
pip install numpy spidev
```

3. Run the program:

```
python src/main.py
```

---

## 🎥 Demo Video

Due to GitHub file size limitations, the demo video is hosted externally:

👉 **[Watch Demo Video](https://drive.google.com/file/d/1I8NiMnWdsuQzPf3dEckR7fr4z8Nbkeok/view?usp=sharing)

---

## 📊 Learning Outcomes

* Understanding of sensor integration
* Signal processing in embedded systems
* GPIO control using Python
* Real-time system response design
