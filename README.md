# Petrol Theft Detection System

## Overview
A security system designed to detect petrol theft, battery theft, two-wheeler theft, and intrusions using an LPC2138 microcontroller interfaced with multiple sensors. When an abnormal event is detected, the system activates a buzzer and sends SMS alerts via a GSM module. The entire system is simulated in Proteus for verification.

## Team Members
- Komal Pradip War (UEC2021267)
- Rakhi Sitaram Kasbe (UEC2022013)
- Harshali Sambhaji Borhade (UEC2022016)

## Features
- Real-time event detection using Flex, Vibration, Gas, and PIR sensors.
- SMS alerts sent instantly via GSM module.
- Audible alarm triggered during suspicious activity.
- Simulated in Proteus before real-world deployment.

## Components Used
- **LPC2138 Microcontroller** (ARM7TDMI-S core)
- **GSM Module** (for sending SMS alerts)
- **Flex Sensor** (detects bending)
- **Vibration Sensor** (detects tampering/vibration)
- **Gas Sensor (MQ-6)** (detects petrol vapors)
- **PIR Sensor** (detects human movement)
- **Buzzer** (for audible alerts)

## Working Principle
1. Sensors monitor continuously and send data to the LPC2138 microcontroller.
2. The microcontroller detects abnormal sensor readings based on predefined conditions.
3. Upon detection:
   - Buzzer is activated for local alert.
   - SMS alert is sent via GSM module to a predefined number.
4. System ensures proactive security by real-time detection and notification.

## Simulation
- **Platform:** Proteus Simulation Environment
- Virtual models of the microcontroller, GSM module, and sensors are created.
- Sensor behavior is emulated to validate event detection and communication flow.

## Code Overview
- **UART Initialization** for GSM communication.
- **GPIO Configuration** for sensor input and buzzer output.
- **Main Loop:**
  - Continuously check sensor status.
  - If an event is detected, send an SMS and activate the buzzer.
- **Delay Function:**
  - Simple software delay used for timing operations.

## Project Setup Instructions
1. Setup the virtual hardware (LPC2138, GSM, Sensors) in Proteus.
2. Flash the provided code to the LPC2138 microcontroller.
3. Connect the GSM module using UART.
4. Simulate different events like bending, vibration, gas leaks, or movement.
5. Verify SMS alerts and buzzer activation.

## Conclusion
This project provides an effective and reliable method for real-time detection of theft or intrusion. Through strategic sensor placement and robust communication, it ensures comprehensive security monitoring. Simulation results validate the design, making it suitable for practical deployment.

## References
1. N. Kaushik et al., "Anti-theft vehicle security system", International Journal for Scientific Research and Development, 2014.
2. S. S. Pethakar et al., "RFID, GPS and GSM based vehicle tracing and employee security system", IJARCSSE, 2012.
3. B. G. Nagaraja et al., "Design and development of a GSM based vehicle theft control system", International Conference on Advanced Computer Control, 2009.
4. M. A. Khedher, "Hybrid GPS-GSM localization of automobile tracking system", International Journal of Computer Science and Technology, 2011.

---

*This project is developed as part of the Open Ended Assignment at MKSSS's Cummins College of Engineering for Women, Pune.*
