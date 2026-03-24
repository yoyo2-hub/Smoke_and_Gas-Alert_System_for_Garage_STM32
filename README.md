# Smoke/Gas Alert System for Garage Using STM32
Hardware used: STM32F401 Nucleo, MQ-2 gas sensor, flame sensor, buzzer, relay module, red LED, Dupont wires.

Description: Inspired by home automation projects using DHT11, LDR, and MQ-2 sensors,this project implements a fire and gas alert system for garages.

The Nucleo reads the MQ-2 voltage via ADC and receives digital signals from the flame detector.

When a hazard is detected, a buzzer sounds, the red LED flashes, and a relay cuts power to equipment (e.g., charger or extractor) to reduce risk.

The system features periodic monitoring with an analog watchdog, configurable thresholds, and hysteresis to prevent false alarms. Serial communication can send alert messages to a PC.

The solution respects real-time and low-power constraints.
