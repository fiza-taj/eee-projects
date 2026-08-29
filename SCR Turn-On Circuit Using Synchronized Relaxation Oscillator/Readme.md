# SCR Turn-On Circuit using Synchronized UJT Relaxation Oscillator

**Mini Project**

**Status:** Completed

---

## Overview

A power electronics mini project on synchronized triggering of a Silicon Controlled Rectifier (SCR) using a UJT (Unijunction Transistor) relaxation oscillator. The circuit generates gate pulses synchronized with the AC supply, enabling precise firing-angle control and regulation of power delivered to a load.

## Objective

- Achieve precise SCR triggering synchronized with the AC waveform
- Control the turn-on timing of the SCR for power regulation

## Components & Specifications

| Component | Purpose | Specification |
|---|---|---|
| SCR | Main power control device; conducts when triggered | 400V, I_T = 4A |
| UJT | Relaxation oscillator generating trigger pulses | V_B2B1 = 10–20V |
| Capacitor | Controls UJT triggering time | 0.1µF – 0.47µF, 100V |
| Resistor | Adjusts capacitor charging rate; controls firing angle | 100kΩ potentiometer |
| Zener Diode | Regulates DC supply to UJT circuit | 12V, 0.5W |

## Working

The AC supply is rectified and regulated by the Zener diode to power the UJT relaxation oscillator. The capacitor charges through the variable resistor until it reaches the UJT's peak-point voltage, at which the UJT switches ON and discharges the capacitor through the pulse transformer's primary winding. This induces a sharp triggering pulse in the secondary winding, applied to the SCR's gate, turning it ON.

Varying the resistor changes the capacitor's charging time, and therefore the SCR's firing angle. This repeats every half cycle, producing gate pulses synchronized with the AC supply for controlled power delivery.

## Hardware Model

![Hardware Model](./scr_project_images/hardware_model.jpg)

## Results

**Output waveform at firing angle = 0 degrees**
![Output waveform at angle 0](./scr_project_images/output_waveform_angle_0.jpg)

**Output waveform at firing angle = 90 degrees**
![Output waveform at angle 90](./scr_project_images/output_waveform_angle_90.jpg)

**Waveform across load**
![Waveform across load](./scr_project_images/output_waveform_load.jpg)

The circuit successfully generated synchronized gate pulses across varying firing angles, confirming reliable SCR turn-on and controllable phase delay.

## Tech Used

`SCR` `UJT Relaxation Oscillator` `Zener Diode` `Power Electronics` `Circuit Analysis`

## Applications

- Motor speed control (AC/DC)
- Light dimming and heating control
- Controlled rectifiers
- Switch-mode power supplies (SMPS)

## Conclusion

The synchronized UJT relaxation oscillator proved an efficient method for controlling SCR firing angle, enabling precise, stable power regulation. This makes it applicable to light dimmers, controlled rectifiers, and motor speed control systems.

## Team

| Name | USN |
|---|---|
| Afrin Sadaf S K | 3VC23EE003 |
| D Ghousiya Taskeen | 3VC23EE018 |
| Fiza Taj | 3VC23EE021 |
| Naseema P | 3VC23EE037 |

Electrical and Electronics Engineering, RBYMEC
