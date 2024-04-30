# Hardware Infrastructure: (images are to be provided later)
==========================
## Vision:
----------
To be able to provide a solid hardware infrastructure with relative ease.
## Mission:
-----------
In the end of the project, the infrastructure is designed to be:
1. Sourced locally.
2. Modular.
3. Open-Source.

## Robot Infrastucture
-------------------------
The main goals of the robot infrastructure is for the robot to be able to:
1. Travese based on user input or robot-made decisions.
2. Sense changes in position as it moves.
3. Receive information from implemented infrastructure in the environment thorugh VLC.
4. Operate on 12V Battery Pack with battery management capabilities.
   
### A - Power Board:
1. Multiple Outputs for Power Distribution.
2. 5V conversion, for powering the used SBC.
3. Reverse Polarity and Overcurrent Protection.

### B - Sensor Board:
Provides feedback regarding robot position using:
1. IMU : MPU6050
2. Ultrasonic sensors for (For obstacle avoidance).
The recorded data is sent to the SBC for processing.

### C - Motion Board:
* Receives commands from the SBC to control 4 independent DC motors, each one driving an omni-directional wheel.
* Each motor has a built-in magnetic rotary encoder, whose signal is processed by the on-board controller and sent to the SBC for recording travelled distance.

### D - Actuators' Board:
* Capable of controlling up to 10 servo motors independently.

### E - Battery Management System:
* Protection Features:
	1. Overvoltage
	2. Undervoltage
	3. Overcurrent
	4. Short Circuit.
* Monitoring Features:
	1. Voltage of each module.
	2. Total Current of the pack
	3. Temperature.
### F - VLC [Receiver]:
* Uses BPW34 Micro solar cell for Detection.
* Structure:
	1. Transimpedance Amplifier.
	2. Voltage Amplifier.
	3. Decision making.
### G - VLC [Transmitter]:
* A code is assigned to each region.
* Each transmitter sends said code by controlling a 220VAC LED.
* Each Bit corresponds to a certain intensity to be detected by the receiver.


## Images:
![Overall_Block_Diagram](https://github.com/meh-land/Dr_Reports/assets/93788514/64f159fb-e910-4954-b8a0-c9498935b370)
![BPW34 Light Sensor (VLC Receiver)](https://github.com/meh-land/Dr_Reports/assets/93788514/0047d68e-7e48-4e5f-8dfa-95b1a3795d08)
![MPU_6050 (Sensor)](https://github.com/meh-land/Dr_Reports/assets/93788514/6dae199f-0dc0-43ba-b974-01c0cda4055d)
![DC Motor with Magnetic Encoder (Motion)](https://github.com/meh-land/Dr_Reports/assets/93788514/d242dec3-982e-48e1-9e79-91760286c1df)
![Servo Motor(Actuators)](https://github.com/meh-land/Dr_Reports/assets/93788514/2cd571ee-818a-4d4b-88f4-140d0f84d8dd)


