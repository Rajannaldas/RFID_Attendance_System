# RFID Attendance System

## 📌 Project Overview
This project is an RFID-based attendance system designed using the LPC2148 microcontroller.  
It is used to track employee attendance and working hours in an organization.

The system reads RFID cards, identifies users, logs attendance, and communicates with a PC system to store data.

## Features
- RFID-based user identification  
- Admin and user modes  
- Add / Delete / Edit employee  
- Real-time clock (RTC) display  
- Working hours calculation  
- UART communication with PC  
- CSV-based data storage

## Components Used
- LPC2148 Microcontroller  
- RFID Reader Module  
- RFID Cards  
- EEPROM (SPI based)  
- LCD Display  
- Keypad  
- UART Communication (RS232)  
- PC System  

## Working
1. RFID card is tapped on reader  
2. RFID reader sends data via UART1  
3. LPC2148 receives data using interrupt  
4. System checks whether card is admin or user  
5. Frame is created
6. Data is sent to PC using UART0  
7. PC program processes data and updates CSV file  
8. Response is sent back to LPC2148  
9. LCD displays the result
    
## Admin Functions
- Add new employee  
- Delete employee  
- Edit employee details  
- Change admin card (stored in EEPROM)

## User Functions
- Login (IN time)  
- Logout (OUT time)  
- Working hours calculation  
- Maximum 3 IN/OUT entries  

## Project Structure
- LPC_Code → Embedded system code
- PC_Code → PC interface program
  
## Software Used
- Keil uVision4 (Embedded C development)  
- Flash Magic (Flashing program)  
- Serial Terminal (UART monitoring)  

## Key Concepts Used
- Embedded C Programming  
- UART Communication  
- SPI Communication  
- Interrupt Handling  
- Real-Time Systems  
- File Handling in C
  
## Future Improvements
- Use database instead of CSV  
- Add fingerprint authentication  
- Cloud-based attendance system  
- Multiple admin support  

## Conclusion
This project demonstrates a real-time embedded system integrating hardware and software to automate attendance tracking efficiently.

## Acknowledgement
I would like to thank my faculty for guidance and support in completing this project.


## Author
Annaladas Raj Kumar
