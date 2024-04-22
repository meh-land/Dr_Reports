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
1. IMU
2. Ultrasonic sensors for (For obstacle avoidance).
The recorded data is sent to the SBC for processing.

### C - Motion Board:
* Receives commands from the SBC to control 4 independent DC motors, each one driving an omni-directional wheel.
* Each motor has a built-in magnetic rotary encoder, whose signal is processed by the on-board controller and sent to the SBC for recording travelled distance.
