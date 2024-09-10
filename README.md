# Motor Control System with Keypad and LCD Interface

This project implements a motor control system using a microcontroller, keypad input, and an LCD for displaying feedback. The system allows users to input a password, which controls access to the motor functions.

## Features

- **Password Verification**: A 4-digit password is required to control the motor. Users are prompted to enter the password via a keypad. The entered digits are masked with `*` on the LCD.
  
- **Access Control**:
  - Correct password entry grants access to control the motor.
  - If the password is incorrect but close (1 digit wrong), a message is displayed indicating proximity to the correct password.
  - After three incorrect attempts, the system locks.

- **Motor Control**: Once access is granted, users can:
  - Turn the motor **ON** (`key 5`)
  - Turn the motor **OFF** (`key 6`)
  - Reverse the motor's direction (`key 4`)

- **Password Reset**: If the system is locked after multiple incorrect attempts, users can reset the password by pressing a specific key (`key 4`). The system will prompt for a new password.

- **LCD Display**: Provides real-time feedback, displaying messages like `WELCOME`, `ACCESS GRANTED`, `ACCESS DENIED`, and motor control instructions.

## Code Overview

- Pin assignments for LCD, motor, and keypad are defined at the beginning of the code.
- Password logic is implemented with storage and verification processes.
- Motor control is managed through simple commands based on user input via the keypad.
- The system includes subroutines for handling the keypad input, password comparison, and LCD display management.

