## Progress Report #1
- Date: 16 - 12 - 23
### Intro
- The main goal for the previous hardware design phase is to provide a suitable infrastructure to operate the cargo-bot, until more sophisticated systems are established in the near future.
- Currently, three boards were designed and tested: One Power Board, One Motor Board, and One Motor Evaluation Board.
### A- Power Board:
- Version: MK-I
- Objective: Provide power from battery pack to motors and control units.
- Features:
  * Protection Features (Fuses on 12V and 5V rails,  Reverse Polartiy on Battery Connectors)
  * 5V source from an efficient buck converter.
  * Multiple Connectors for multiple access of voltages.
- Images:
- <img src="https://github.com/meh-land/Dr_Reports/assets/93788514/3a836798-9459-4715-b97e-4c5b9fabe13e" width="40%" height="40%">
- <img src="https://github.com/meh-land/Dr_Reports/assets/93788514/eb5f9a61-bf00-48d7-8d9d-69b583f1aaf0" width="40%" height="40%">
- <img src="https://github.com/meh-land/Dr_Reports/assets/93788514/dda18dc0-d786-4d25-bde0-d4b7afc05aad" width="50%" height="50%">

### B- Motor Board:
- Version: MK-I
- Objective: Driving the used DC Motors, in order to test motion cababilities of the cargo-bot.
- Features:
  * The used controller is STM32 Blue Pill.
  * Controlling up to 4 DC motors using external motor drivers.
  * Monitoring the motion of the 4 motors using attached magnetic encoders with the motors.
![image]()

- Images:
- <img src="https://github.com/meh-land/Dr_Reports/assets/93788514/df2a69bc-a13a-43d5-81f6-953d9059f44b" width="40%" height="40%">
- <img src="https://github.com/meh-land/Dr_Reports/assets/93788514/cbf71202-07b3-4cfd-ace0-1d44fd7cdb5e" width="40%" height="40%">
- <img src="https://github.com/meh-land/Dr_Reports/assets/93788514/d9cc9f73-fb4b-45c8-9f0c-03138d9c4418" width="40%" height="40%">


### C- Motor Driver Evaluation Board:
- Version: MK-I
- Objectives:
  * Testing the newly found TB67H450FNG motor driver IC and its features.
  * Preparing a test rig for any suggested DC motor.
  * Monitoring the I-V Characteristics of DC motor.
  
- Features:
  * Simple interfacing with the board.
  * Selectable source of *Vref* for the current limit feature of the driver.
  * Test points on boards for measuring voltages (Vref, Vout)
  * Shunt resistor for monitoring current waveform using an oscilloscope.
- Images:
- <img src="https://github.com/meh-land/Dr_Reports/assets/93788514/716bf3e9-33b5-447a-915d-037e3bfb60d0" width="40%" height="40%">
- <img src="https://github.com/meh-land/Dr_Reports/assets/93788514/4ee7737b-2da3-4c63-a81d-b704bd11efed" width="40%" height="40%">
- <img src="https://github.com/meh-land/Dr_Reports/assets/93788514/c02a5534-ae0f-42dd-9254-0e98bef5ceff" width="40%" height="40%">

### In progress:
- Building a board, based on the famous STM32 Blue Pill, to communicate with the _Single Board Computer_ (SBC) via CAN, to control up to 10 Servo Motors.
- Studying how to monitor cells' _State of Health_ (SOH) and _State of Charge_ (SOC).
### Near Future Plans:
- Designing power system MK-II with cell monitoring features.
- Designing a compact system, based on STM32 Blue Pill, to control 4 DC motors based on the communcations with the SBR.

