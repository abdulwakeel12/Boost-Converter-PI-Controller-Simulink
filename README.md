
# ⚡ Closed Loop Boost Converter using PI Controller – Simulink Model

🎓 **6th Semester Project**  
📅 **Duration:** January 2023 – June 2023  
🏛 **Institution:** Sukkur IBA University  
🏢 **Department:** Electrical Engineering  
📘 **Course:** ELE-321: Control Systems (Spring 2023)  
👨‍🏫 **Instructor:** Dr.-Ing. Kashif Hussain

---

## 👤 Group Member

- **Wakeel Ahmed**  
  CMS ID: 033-19-0026

---

## 📖 Project Introduction

This project focuses on designing and simulating a **Closed Loop Boost Converter** using a **PI controller** in **MATLAB Simulink**. The boost converter steps up a DC input voltage to a higher level and is essential in battery systems, solar panels, and electric vehicles. A PI (Proportional-Integral) controller improves voltage regulation and efficiency.

---

## ⚙️ Boost Converter Design

### 🔌 Circuit Components

- Input Voltage Source
- MOSFET (Power Switch)
- Inductor
- Diode
- Output Capacitor
- PI Controller

---

## 🧠 Control Strategy

A PI controller is implemented to:
- Regulate the PWM signal duty cycle
- Compare desired vs. actual output voltage
- Reduce error through control logic

---

## 🛠 MATLAB Simulink Model

### 🧩 Main Blocks Used:

- **Pulse Generator**  
- **MOSFET Switch**
- **Inductor**
- **Capacitor**
- **Gain Block**
- **PI Controller**
- **Scope**

These are connected to simulate a working Boost Converter system.

---

## 📐 Parameter Calculations

| Parameter     | Value    |
|---------------|----------|
| Vin           | 12 V     |
| Vout          | 20 V     |
| Frequency (f) | 25 kHz   |
| Duty Cycle (D)| 0.625    |
| Iout          | 1 A      |
| ΔIL           | 0.2 A    |
| ΔV            | 0.1 V    |
| Inductor (L)  | 3.6 μH   |
| Capacitor (C) | 0.2 μF   |
| Load (RL)     | 4 Ω      |

---

## 🧪 PI Controller Tuning (Ziegler-Nichols Method)

1. Set **P** and **I** to zero
2. Increase **P** until the output oscillates
3. Measure oscillation period (**Tu**) and ultimate gain (**Ku**)
4. Calculate:

```
P = 0.6 × Ku  
I = 1.2 × Ku / Tu  
```

Adjust gains iteratively for:
- Better stability
- Faster settling time
- Less overshoot

---

## 📊 Simulation Analysis

- ✅ **Voltage Regulation**: Maintains stable Vout under load
- ⚙️ **Efficiency**:  
  `Efficiency (%) = (Pout / Pin) × 100`
- 📉 **Performance Metrics**:  
  - Settling Time  
  - Overshoot  
  - Steady-state Error

---

## 📈 Output Observations

Figures include:
- 🔁 Circuit Diagram
- 📉 Output Voltage Waveform
- 📊 Output Values
- 📈 Current Waveform
- 🔢 Current Values

> (Note: Please upload simulation images/screenshots in the `images/` folder and embed them like:  
> `![Figure 1: Boost Converter Circuit](images/boost-circuit.png)`)

---

## ✅ Conclusion

This project successfully demonstrates the modeling and control of a **Boost Converter** using a **PI Controller** in **MATLAB Simulink**. The PI controller greatly enhances voltage regulation, enabling better stability under variable input and load conditions.

---

## 📚 References

- [Tutorials Point - DC Motor Control](https://www.tutorialspoint.com/arduino/arduino_dc_motor.htm)
- [Slideshare - Speed Control of DC Motor](https://www.slideshare.net/mafazahmed/speed-control-of-dc-motor)
- [ElectronicsHub - Boost Converter with PI](https://www.electronicshub.org/speed-and-direction-control-of-dc-motor-using-arduino/)

---

© 2023 Wakeel Ahmed, Sukkur IBA University  
All Rights Reserved
