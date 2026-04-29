# RFID Attendance System

This project is an RFID-based attendance system using LPC2148 microcontroller.

## Features
- RFID card detection
- Admin and user modes
- Attendance logging
- UART communication with PC
- CSV-based data storage

## Components Used
- LPC2148
- RFID Reader
- EEPROM (SPI)
- LCD Display
- Keypad
- UART Communication

## Working
1. RFID card is scanned
2. LPC2148 reads data via UART
3. System checks admin or user
4. Data sent to PC
5. PC stores attendance in CSV file
6. LCD displays result

## Project Structure
- LPC_Code → Embedded system code
- PC_Code → PC interface program

## Author
Annaladas Raj Kumar
