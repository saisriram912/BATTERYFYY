# BATTERYFYY
Designed an Arduino-based battery monitoring system that evaluates Li-ion battery condition through voltage and current measurements. It performs load testing, estimates internal resistance using voltage drop, and displays battery parameters and condition on a 16×2 LCD.
# Arduino-Based Battery Voltage and Condition Monitoring System

## Project Overview
This project is designed to monitor the condition of a 3.7V Li-ion battery using an Arduino UNO. It measures battery voltage and load current, performs controlled load testing, and estimates internal resistance based on the voltage drop under load. An LM358 operational amplifier is used for current-sensing signal amplification, while an IRF540N MOSFET controls the load. The measured parameters and estimated battery condition are displayed on a 16×2 I2C LCD.

The system provides a simple approach to identifying possible battery degradation through voltage and internal resistance monitoring.

## Key Features
- Battery voltage measurement using a voltage divider.
- Load current measurement using a shunt resistor and LM358.
- MOSFET-controlled load testing.
- Internal resistance estimation.
- Real-time parameter display on an LCD.

## Technologies Used
- Arduino UNO
- LM358 Operational Amplifier
- IRF540N MOSFET
- 16×2 I2C LCD
- Voltage Divider
- Shunt Resistor
- 4.7Ω Load Resistor
- Embedded C / Arduino IDE

## Working Principle
The Arduino first measures the battery's no-load voltage. It then activates a load through the MOSFET and measures the loaded voltage and current. By comparing the voltage readings, the system estimates the battery's internal resistance and displays the results on the LCD.

**Note:** This prototype estimates battery condition; it does not directly measure actual battery capacity or provide a certified State of Health (SoH) percentage.

## Applications
- Basic Li-ion battery monitoring.
- Educational electronics projects.
- Battery condition assessment prototypes.
- Embedded systems and sensor-based monitoring.

## Project Status
Prototype development and testing.
