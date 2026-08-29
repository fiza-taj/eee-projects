# ⚡ SCR Turn-On Circuit using Synchronized UJT Relaxation Oscillator

*Mini Project — Batch A4, Section A*

A power electronics mini project on synchronized triggering of a Silicon Controlled Rectifier (SCR) using a UJT (Unijunction Transistor) relaxation oscillator, guided by **Deepa B** (Project Guide), **Mr. Elia Sundram** and **Mr. Gangadhar J** (Project Co-ordinators), under **Dr. S Kotresh**, HOD, Dept. of EEE.

**Status:** ✅ Completed

---

## 📋 Overview

An SCR is turned on by applying a suitable gate pulse and stays conducting until current falls below its holding value. This project builds a **synchronized UJT relaxation oscillator** circuit to generate sharp, consistent gate pulses in sync with the AC supply — enabling precise firing-angle control and smooth regulation of power delivered to a load.

---

## 🎯 Objective

- Achieve precise SCR triggering synchronized with the AC waveform
- Control the turn-on timing of the SCR for power regulation

---

## ⚙️ Components & Specifications

| Component | Purpose | Specification |
|---|---|---|
| **SCR** (Silicon Controlled Rectifier) | Main power control device; conducts when triggered | 400V, I_T = 4A |
| **UJT** (Unijunction Transistor) | Relaxation oscillator generating trigger pulses | V_B2B1 = 10–20V |
| **Capacitor** | Charges/discharges to control UJT triggering time | 0.1µF – 0.47µF, 100V |
| **Resistor** | Adjusts capacitor charging rate; controls firing angle | 100kΩ potentiometer |
| **Zener Diode** | Regulates DC supply to UJT circuit; stable reference voltage | 12V, 0.5W |

---

## 🔬 Working

When AC supply is applied, part of it is rectified and regulated by the Zener diode to supply the UJT relaxation oscillator. The capacitor charges through the variable resistor; once it reaches the UJT's peak-point voltage, the UJT switches ON and the capacitor discharges rapidly through the pulse transformer's primary winding. This induces a sharp triggering pulse in the secondary winding, applied to the SCR's gate, turning it ON.

Adjusting the resistor varies the capacitor's charging time — and therefore the SCR's firing angle (α). This repeats every half cycle, producing gate pulses synchronized with the AC supply, allowing smooth power control to loads such as lamps, heaters, or motors.

---

## 🖼️ Hardware Model

![Hardware Model](./scr_project_images/hardware_model.jpg)

---

## 📈 Results — Output Waveforms

**Half-wave output at firing angle = 0°**
![Output waveform at angle 0](./scr_project_images/output_waveform_angle_0.jpg)

**Load waveform at firing angle = 90°**
![Output waveform at angle 90](./scr_project_images/output_waveform_angle_90.jpg)

**Waveform across load (V_load / V_SCR)**
![Waveform across load](./scr_project_images/output_waveform_load.jpg)

The synchronized UJT oscillator successfully generated sharp, consistent gate pulses across varying firing angles, confirming reliable SCR turn-on and controllable phase delay.

---

## 🛠️ Tech / Components Used

`SCR` `UJT Relaxation Oscillator` `Zener Diode` `Power Electronics` `Circuit Analysis`

---

## 🌍 Applications

- Speed control of AC and DC motors
- Light dimming and heating control
- Controlled rectifiers
- Automatic power switching
- Pulse generators
- Sawtooth wave generators
- Switch-mode power supplies (SMPS)

---

## ✅ Advantages

- Precise and stable triggering
- Accurate phase control
- Sharp, fast-rising pulses with efficient, robust triggering
- Minimizes power dissipation
- Circuit simplicity and cost-effectiveness

---

## 📝 Conclusion

The SCR turn-on circuit using a synchronized UJT relaxation oscillator proved an efficient and reliable method for controlling SCR firing angle in AC circuits. Adjusting the resistor and capacitor values in the timing network allowed precise control of output power, resulting in smooth, stable operation — making this method widely applicable in light dimmers, controlled rectifiers, and motor speed control systems.

---

## 📚 References

1. Md. Moyeed Abrar (2018), *International Journal of Advanced Technology and Engineering Exploration* — synchronized UJT trigger circuit for SCR turn-on, improved phase-controlled stability.
2. M. H. Rashid (2017), *Power Electronics: Circuits, Devices and Applications*, Pearson Education — UJT relaxation oscillator working and SCR triggering method.
3. M. D. Singh & K. B. Khanchandani (2011), *Power Electronics*, Tata McGraw-Hill — synchronized UJT oscillator firing circuit and phase control in AC rectifiers.

---

## 👥 Team

| Name | USN |
|---|---|
| Afrin Sadaf S K | 3VC23EE003 |
| D Ghousiya Taskeen | 3VC23EE018 |
| Fiza Taj | 3VC23EE021 |
| Naseema P | 3VC23EE037 |

*Electrical and Electronics Engineering Students, RBYMEC*
