# MS-3.08-Introduction-to-computer-controlled-experiments (ICCE)

This repository contains the complete workflow for the *Introduction to Computer-Controlled Experiments* laboratory, which investigates current–voltage (I–V) characteristics of electronic components using an Arduino-based data acquisition system and Python control scripts.

The experiment combines basic electronics, serial communication, data acquisition, uncertainty analysis, and scientific visualisation.

---


## 🔬 Experiment Overview

- Arduino generates a variable analogue voltage using PWM filtered by an RC network.
- Voltage is applied to LEDs and a resistor in series with a known sensing resistor.
- Current is inferred from the voltage drop across the series resistor.
- Voltage and current are recorded automatically via serial communication.
- I–V characteristics are analysed and compared across components.

---

## 🧪 Components Tested

- Red LED  
- Yellow LED  
- Green LED  
- Blue LED  
- Fixed resistor (ohmic reference)

---

## 📊 Key Analysis Performed

- Automated voltage sweeps (0–5 V)
- Repeated measurements to reduce random error
- I–V curve plotting and comparison
- Linear fitting for resistor validation
- Two-region fitting for LEDs (pre- and post-turn-on)
- Qualitative interpretation of band-gap effects
- Optional numerical differentiation (dI/dV)

---

## 🧠 Concepts Covered

- UART / serial communication
- PWM and RC filtering
- Ohmic vs non-ohmic behaviour
- Semiconductor band gap and LED turn-on voltage
- Measurement uncertainty propagation
- Data reproducibility and reuse

---

## 🛠️ Requirements

- Arduino-based DAQ system (as provided in the lab)
- Python 3.x
- Required Python packages:
  ```bash
  numpy
  matplotlib
  pyserial
  time
  datetime
  csv
