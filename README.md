# Punch Impact Estimator Using Piezoelectric Sensor

## Overview
This project measures relative punch impact intensity using a piezoelectric sensor and Arduino-based signal processing. The goal was to design a low-cost embedded system capable of detecting and comparing strike forces while dealing with noisy, high-speed impact signals.

---

## Objectives
- Detect punch impacts reliably
- Extract meaningful signal features
- Compare strike intensity
- Maintain low cost (< £30)

---

## System Architecture
Impact → Piezo Sensor → Protection Circuit → Arduino ADC → Signal Processing → Output

---

## Hardware Design

Components:
- Arduino Uno
- Piezoelectric disc sensor
- 1MΩ resistor
- Protection diode

Design considerations:
- Piezo sensors produce high-voltage spikes
- Protection circuitry required to prevent ADC damage
- Sensor placement affects repeatability

---

## Software Design

Processing steps:
1. Sample analog signal
2. Detect impact threshold
3. Capture signal peak
4. Log peak value

Key engineering challenge:
Filtering noise while preserving fast transient signals.

---

## Testing & Results

Tests performed:
- Light punch
- Medium punch
- Hard punch

Results:
- Clear voltage amplitude differences observed
- Repeatability improved with consistent mounting

Limitations:
- Cannot measure absolute force
- Sensitive to placement

---

## Improvements

Future upgrades could include:
- Higher-resolution ADC
- Multiple sensors
- Machine learning classification
- Wireless data transmission

---

## Skills Demonstrated

- Embedded systems
- Analog signal acquisition
- Sensor interfacing
- Signal processing
- Experimental testing

---

## Images

(Insert build photos here)

---

## Conclusion

This project demonstrated that low-cost sensing hardware can be used to extract meaningful impact data when combined with proper signal conditioning and analysis.
