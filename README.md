# POWERGUARD
## Project Overview
The Voltage and Earth Monitoring System is an Arduino-based safety and monitoring solution designed to continuously monitor phase voltage, earth continuity, and ground fault conditions in electrical systems. The system detects abnormal conditions such as loss of supply, earth failure, and ground faults, and immediately alerts the user through a mobile application while also isolating the load for safety.

This project is especially useful in industrial, residential, and institutional electrical installations where proper earthing and voltage availability are critical for safety and equipment protection.

## Objectives
Monitor the availability of phase voltage in real time  
Detect earth failure and ground fault conditions  
Automatically disconnect the load during unsafe conditions  
Send real-time alerts to a mobile application via Bluetooth  
Allow manual reactivation of the load after fault clearance  

## System Description
The system uses an Arduino microcontroller as the core processing unit. Voltage divider circuits are used to safely sense phase and earth voltages. Based on the sensed conditions, the Arduino controls a relay module to disconnect or reconnect the load.

A Bluetooth module (HC-05) is used to communicate system status messages to a mobile application developed using MIT App Inventor.

## Hardware Components
Arduino UNO, Voltage Divider Circuits, 5V Power Supply / Charger (230V to 5V), Relay Module, Bluetooth Module (HC-05), Resistors, Diodes, LEDs, Load (Bulb for demonstration)

## Working Principle
The system continuously monitors the phase voltage using a voltage divider.  
Another sensing circuit monitors earth continuity and ground fault conditions.  
If phase voltage is lost, the system sends a "NO CURRENT" alert to the mobile app.  
If an earth fault or ground fault is detected, the system sends a "GROUND FAULT" alert.  
During unsafe conditions, the relay disconnects the load automatically.  
Once the fault is cleared, the user can manually turn ON the relay using the mobile app.  

## Mobile App Features
Displays real-time system status  
Shows fault messages such as:  
NO CURRENT  
GROUND FAULT  
Manual relay ON control after fault rectification  
Simple and user-friendly interface  

<p align="center">
  <img src="Images/APP Screen shot.png" width="400">
</p>
