# 📘 MS-3.08 — Introduction to Computer-Controlled Experiments (ICCE)

This repository contains the complete experimental and data-analysis workflow for the Introduction to Computer-Controlled Experiments (ICCE) laboratory module.

The experiment investigates the current–voltage (I–V) characteristics of electronic components, using an Arduino-based data acquisition system controlled via Python scripts. The project integrates basic electronics, serial communication, automated data collection, uncertainty analysis, and scientific visualisation.


## 🔬 Experiment Overview
	•	An Arduino microcontroller generates a variable analogue voltage using PWM filtered by an RC network
	•	The voltage is applied to LEDs or a fixed resistor in series with a known sensing resistor
	•	The current is inferred from the measured voltage drop across the sensing resistor
	•	Voltage and current data are acquired automatically via serial (UART) communication
	•	I–V characteristics are analysed and compared across components and conditions

## 🧪 Components Tested
	•	Red LED
	•	Yellow LED
	•	Green LED
	•	Blue LED
	•	White LED
	•	Fixed resistor (ohmic reference)


## 📊 Key Analysis Performed
	•	Automated voltage sweeps (0–5 V)
	•	Repeated measurements to reduce random error
	•	I–V curve plotting and comparison
	•	Linear fitting to validate ohmic behaviour of the resistor
	•	Two-region analysis of LED I–V curves (pre- and post-turn-on)
	•	Extraction of LED turn-on voltages
	•	Semi-log I–V fitting using the Shockley diode model
	•	Qualitative interpretation of semiconductor bandgap effects
	•	Optional numerical differentiation (dI/dV)
	•	Comparison of LED performance at room temperature (RT) and 77 K (liquid nitrogen cooling)

## 🧠 Concepts Covered
	•	UART / serial communication
	•	PWM generation and RC filtering
	•	Ohmic vs non-ohmic behaviour
	•	Semiconductor bandgap and LED turn-on voltage
	•	Ideality factor and model limitations
	•	Measurement uncertainty and reproducibility
	•	Data reuse and automated scientific workflows


## 🛠️ Requirements

### Hardware
	•	Arduino-based DAQ system (as provided in the ICCE laboratory)
	•	Standard electronic components (LEDs, resistors)

### Software
	•	Python 3.x
	•	Required Python packages:
	•	numpy
	•	matplotlib
	•	pyserial
	•	time
	•	datetime
	•	csv

## 👥 Authorship

This project was conducted as part of the ICCE laboratory course in collaboration with:

- **Devan Hu** 

Experimental work and initial data handling were performed jointly.  
Subsequent data analysis, visualisation, and automation scripts were primarily developed by the repository author, with contributions and discussion from the collaborator.
