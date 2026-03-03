# 🤖 RTOS-Based Health Monitoring & Fall Detection System using LPC1768

This project implements a real-time health monitoring and fall detection system using the ARM Cortex-M3 based LPC1768 microcontroller with CMSIS-RTOS. The system simulates heart rate monitoring and detects bed-fall conditions using IR sensors, triggering alerts accordingly.

## 📌 Problem Statement

In hospital environments, continuous patient monitoring is required to track heart rate and detect fall incidents in real time. Manual supervision can lead to delays. This project demonstrates an RTOS-based embedded solution capable of handling multiple monitoring tasks concurrently.

## 🎯 Objectives

- Simulate heart rate (BPM) monitoring  
- Indicate abnormal BPM using LED  
- Detect fall events using dual IR sensors  
- Trigger buzzer alert during fall condition  
- Display real-time status on 16x2 LCD  
- Implement multitasking using CMSIS-RTOS  

## 🛠️ Technologies Used

- Microcontroller: LPC1768 (ARM Cortex-M3)  
- Programming: Embedded C  
- RTOS: CMSIS-RTOS  
- Development Tool: Keil µVision  
- Components: 16x2 LCD, IR Sensors (x2), Buzzer, LED  
