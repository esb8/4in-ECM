# Engine Control Module

## Overview  
The **Engine Control Module (ECM)** is a **control and data acquisition (DAQ) system** designed for liquid rocket engine testing. It integrates sensor measurement, actuation control, and data logging into a compact embedded system suitable for ground testing and development.  

The system is capable of:  
- Monitoring **up to 4 pressure transducers**  
- Reading multiple **thermocouples** for temperature measurement  
- Controlling **1 solenoid valve** (on/off flow control)  
- Driving **2 servo motors** (valve actuation or gimbal control)  
- Logging sensor data for analysis and verification  

---

## Features  
- **Data Acquisition**  
  - 4 analog channels for high-accuracy pressure transducers  
  - Integrated thermocouple interface for combustion chamber and feed line monitoring  
  - Real-time sampling and logging  

- **Actuation**  
  - Solenoid driver with high-side switching capability  
  - Dual servo motor outputs (PWM control)  
  - Configurable control logic for sequencing and automation  

- **System Control**  
  - Embedded microcontroller (e.g., STM32/Arduino/FPGA – specify)  
  - USB/UART interface for PC communication  
  - Safety interlocks and emergency shutdown support  

- **Software**  
  - Firmware for DAQ, control, and communications  
  - Logging utility for test data collection  
  - Configurable sampling rates and actuation sequences  

---

## Applications  
- Small-scale **liquid rocket engine testing**  
- **Valve and feed system automation**  
- **Sensor data acquisition** for propulsion research  
- **Ground support equipment** integration  

---

## Getting Started  
1. **Hardware Setup**  
   - Connect pressure transducers to the analog input ports (0–5 V or 0–10 V).  
   - Connect thermocouples to the thermocouple inputs.  
   - Wire solenoid to the high-side driver output.  
   - Connect servos to PWM headers.  

2. **Software Setup**  
   - Flash firmware using the provided source code.  
   - Install the DAQ/logging software on your PC.  
   - Configure serial port and sampling rate.  

3. **Operation**  
   - Power on the ECM.  
   - Verify sensor calibration.  
   - Execute control sequences via PC interface or onboard logic.  

---

## Safety Notes  
⚠️ This module is intended for **research and experimental use only**.  
- Always follow proper test stand safety procedures.  
- Use protective enclosures and remote operation where possible.  
- Ensure solenoid and servo actuation logic is validated before hot-fire testing.  
