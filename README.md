# Thermal Management System

Dual-microcontroller embedded thermal management system using an STM32 
Nucleo F030R8 as the control node and an ESP32 WROVER as the UI node.

The STM32 runs a three-state finite state machine (MONITORING, COOLING, 
FAULT) with hysteresis-based control logic, driving a PWM-actuated fan 
in response to live temperature and humidity sensor data. System 
telemetry is transmitted over UART to the ESP32, which renders 
real-time system state on an I2C LCD display.
