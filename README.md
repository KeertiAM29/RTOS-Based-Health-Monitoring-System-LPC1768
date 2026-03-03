# 🤖 RTOS-Based Health Monitoring & Fall Detection System using LPC1768

This project implements a real-time health monitoring and fall detection system using the ARM Cortex-M3 based LPC1768 microcontroller with CMSIS-RTOS. The system simulates heart rate monitoring and detects bed-fall conditions using IR sensors.

## 📌 Problem Statement

Continuous monitoring of patients in hospitals is required to detect abnormal heart rate conditions and fall incidents. Manual monitoring can cause delayed response. This project demonstrates an RTOS-based embedded solution for concurrent monitoring tasks.

## 🎯 Objectives

- Simulate heart rate (BPM) monitoring  
- Indicate abnormal BPM using LED  
- Detect bed-fall events using IR sensors  
- Trigger buzzer alert during fall condition  
- Display system status on 16x2 LCD  
- Implement multitasking using RTOS  

## 🛠️ Technologies Used

- Microcontroller: LPC1768 (ARM Cortex-M3)  
- Programming Language: Embedded C  
- RTOS: CMSIS-RTOS  
- Development Tool: Keil µVision  
- Components: 16x2 LCD, IR Sensors (2), Buzzer, LED
## 🎥 Project Demo

[Watch / Download Demo Video](https://raw.githubusercontent.com/KeertiAM29/RTOS-Based-Health-Monitoring-System-LPC1768/main/working%20video.mp4)

 

## ⚙️ RTOS Implementation

Three concurrent threads were implemented using CMSIS-RTOS:

```c
IR_Task();    // Monitors IR sensors for bed-fall detection
BPM_Task();   // Simulates heart rate and updates LCD
ALERT_Task();// Handles buzzer alert and LCD lock during fall
