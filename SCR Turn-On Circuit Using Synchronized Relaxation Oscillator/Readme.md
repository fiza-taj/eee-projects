# SCR Turn-On Circuit using Synchronized UJT Relaxation Oscillator

Mini Project
Status: Completed

## Overview

A power electronics mini project on synchronized triggering of a Silicon Controlled Rectifier (SCR) using a UJT relaxation oscillator. The circuit generates gate pulses synchronized with the AC supply, enabling precise firing-angle control and regulation of power delivered to a load.

## Components & Specifications

| Component | Purpose | Specification |
|---|---|---|
| SCR | Main power control device | 400V, I_T = 4A |
| UJT | Generates trigger pulses | V_B2B1 = 10-20V |
| Capacitor | Controls UJT triggering time | 0.1uF - 0.47uF, 100V |
| Resistor | Controls firing angle | 100kOhm potentiometer |
| Zener Diode | Regulates DC supply | 12V, 0.5W |

## Working

The AC supply is rectified and regulated by the Zener diode to power the UJT relaxation oscillator. The capacitor charges through the variable resistor until it reaches the UJT's peak-point voltage, causing the UJT to switch ON and discharge through the pulse transformer's primary winding. This induces a sharp triggering pulse applied to the SCR's gate, turning it ON. Varying the resistor changes the firing angle, producing gate pulses synchronized with the AC supply.

## Results

The circuit successfully generated synchronized gate pulses across varying firing angles (tested at 0 degrees and 90 degrees), confirming reliable SCR turn-on and controllable phase delay. Hardware model and waveform images are included in this repository.

## Tech Used

SCR, UJT Relaxation Oscillator, Zener Diode, Power Electronics, Circuit Analysis

## Applications

- Motor speed control (AC/DC)
- Light dimming and heating control
- Controlled rectifiers
- Switch-mode power supplies (SMPS)

## Team

| Name | USN |
|---|---|
| Afrin Sadaf S K | 3VC23EE003 |
| D Ghousiya Taskeen | 3VC23EE018 |
| Fiza Taj | 3VC23EE021 |
| Naseema P | 3VC23EE037 |

Electrical and Electronics Engineering, RBYMEC
