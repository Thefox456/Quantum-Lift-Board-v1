# Quantum-Lift-Board-v1
Elevator Control Board (9 Floors + Automatic Doors) – Full Design
System Overview:
Control Logic
74HC/CD4000 Series Logic Gates for sequencing and control
7-segment display driver for floor indication
Call request buttons for each floor + emergency stop
Flip-flops & Counters to track floor levels

Motor Control
380V DC Elevator Motor (controlled via relays + MOSFET drivers)
DC Motor for Doors (controlled by H-bridge driver)
Limit switches for floor positioning & door operation

Safety Features
Emergency Braking System (Relay cutoff in emergencies)
Overload Detection (Current sensor)
Door Interlock Mechanism (Ensures the door stays closed while moving)

Microcontroller-Based Logic Control (PIC16F877A)
-Handles floor selection logic
-Controls 7-segment display for floor indication
-Manages motor control relays & safety interlocks
Function-------------------------------------------PIC16F877A Pin
Floor Buttons Input	-------------------------------PORTB (RB0-RB7)
7-Segment Display	PORTD ---------------------------(D0-D7)
Motor Control Relays--------------------------------RC0, RC1
Door Motor PWM--------------------------------------CCP1 (RC2)
Limit Switches--------------------------------------RA0, RA1
Overload Sensor-------------------------------------RA2 (ADC)
