# ESP32 Back EMF Detector

Detecting back EMF from an inductor or a small DC motor using an ESP32’s ADC input.

---

## 📌 Overview
When the current through an inductive load (motor or inductor) is suddenly interrupted, a **voltage spike (back EMF)** occurs.  
This project uses the **ESP32’s analog-to-digital converter (ADC)** to measure that spike and print the values to the Serial Monitor.

---

## 🛠️ Components
- ESP32 development board  
- Small DC motor or inductor  
- 9V battery + pushbutton  
- Voltage divider resistors  
- Diode (for protection)  
- Breadboard + jumper wires  

---

## 🔌 Circuit
- Motor/Inductor powered by 9V through a pushbutton.  
- Voltage output tapped via a voltage divider into ESP32 **GPIO 35**.  
- Diode across the motor/inductor for back EMF protection.  

*(Insert circuit diagram image here if you have one.)*

---

## 💻 Code
See [`back_emf_detector.ino`](back_emf_detector.ino).  

The sketch reads ADC values from GPIO 35 and prints a message if back EMF is detected above a thr

