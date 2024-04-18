# Progress Report

## Server
During the past weeks, development on the server side has moved forward in terms of research as well as development of the actual infrastructure, here is a summary of these developments.

### Infrastructure
* Simple website used for testing the robot's motion.

* Integrating the website's backend with ROS (Noetic).

* Setup the website on a virtual server (virtual machine) and adjust the machine's networking such that it is accessible from any device throughout the network.

* Setup another virtual server to emulate video streaming.

### Research
* Researched docker and docker-compose with the goal of migrating the previously mentioned infrastructure to a docker base, the purpose is portability and flexibility.

* Researched ROS (Humble and Noetic), the docker infrastructure associated with ROS Humble was in progress when the decision was made to switch to ROS Noetic due to some libraries and functionalities that are available for Noetic and not Humble (despite Humble being the most up-to-date  version).

* Currently researching the various components of the (LAMP) infrastructure which consists of:

    * Laravel framework

    * Apache web server

    * MySQL database

    * PHP language for backend

    These components are being studied in order to deploy the main website on a virtual server of its own and later on can be migrated to a docker base.


### Future plans
* Work with embedded team to deploy video streaming software on the SBC.

* Work with embedded team to establish reliable communication between the server and SBC using ROS.

* Integrate main website with docker infrastructure.

* Write python and bash scripts to facilitate deployment of various parts of the system, as well as improve upon the already existing scripts.

<!--************************************************************************************-->
## Web Application

### Used Technologies:
**React.js Framework with TypeScript template.**

> #### TypeScript is used instead of Javascript:
> ![image](https://github.com/meh-land/Dr_Reports/assets/79084467/f528c640-7ed3-42ea-84aa-d5006c01413e)

> TypeScript is often considered better than JavaScript for several reasons, especially in the context of large-scale or complex applications.
>
> Here are some key advantages of TypeScript over JavaScript:
> -----------------------------------------------------------
> * **Optional Static Typing:**
>
> JavaScript is a dynamically typed language, meaning that the software will not treat type differences as errors up until runtime.
> This often resulted in a lot of bugs and frustration. However, TypeScript offers optional static typing. Once static typing is declared,
> a variable does not change its type and can only take in certain values. The compiler alert developers of any type-related errors
> which results in early bug detection.
>
> * **Early Bug Detection:**
>
> With the compiler checking our code, warnings and errors caught for us at the time of development, decreasing the chances of bugs and
> unexpected behavior at runtime. Checking type correctness at compile time also helps with refactoring code quickly with confidence.
> Overall, this feature helps avoid accidental mistakes that developers otherwise would have to comb through manually in JavaScript.
>
> * **Improved Readability:**
>
> Defined types and clear categories for variable declarations not only improve readability, but the stability of the code overall.


### Done Features:
#### 1.  **Membership [Registeration / Login]:**
  ![image](https://github.com/meh-land/Dr_Reports/assets/79084467/9f321577-600d-4ae2-9b02-166456ab0269)
![image](https://github.com/meh-land/Dr_Reports/assets/79084467/6120d821-154b-4768-958a-da9849f1e850)

> ***Cookies are used such that whenever user checks **Remember me** checkbox, they don't have to login everytime they visit the website.***
>
>  ![image](https://github.com/meh-land/Dr_Reports/assets/79084467/124af93b-cfed-4d16-88f5-5a7140791619)


#### 2. **User Profile:**
   ![image](https://github.com/meh-land/Dr_Reports/assets/79084467/6f90dd14-6dbb-417c-83a9-b5fc38d55b93)
   ![image](https://github.com/meh-land/Dr_Reports/assets/79084467/23669768-9f21-4dee-91fe-298c1ded847b)
   ![image](https://github.com/meh-land/Dr_Reports/assets/79084467/7bce86f2-d8a0-477d-b3d4-46ea877fd790)
> ***Sweetalert2 library is used to provide feedback whether edits are done successfully or warning in case of error.***
   ![image](https://github.com/meh-land/Dr_Reports/assets/79084467/4fd01f71-bd97-410a-9d7c-77969a898eac)



<!--************************************************************************************-->

## Mobile Application

### Used Technologies:
* **React Native**
  > React Native is a React JS-based framework to design mobile apps with reusable components.

* **EXPO**
  > Simplified Development Experience Expo is a framework and platform for building React Native applications.
  > It aims to provide a simplified development experience by abstracting away some of the complexities involved in setting up and
  > configuring a React Native project.
  >
  > Advantages of Expo:
  > ------------------
  > **1. Quick Start:**
  >
  >    Expo allows you to quickly start developing your app without worrying about device-specific setup or native code dependencies.
  >
  > **2. Over-the-Air Updates:**
  >
  >    With Expo, you can deploy updates to your app directly to user devices without requiring them to download a new version from the app store.
  >
  > **3. Access to Pre-built Libraries:**
  >   
  >    Expo provides a wide range of pre-built libraries and APIs, making it easy to add features like push notifications, in-app purchases, and maps to your app.
  >
  > **4. Simplified Build Process:**
  >
  >    Expo handles the build process for you, abstracting away the need to configure build tools and deal with native code compilation.
  >
  > **5. Native Physical Device:**
  >
  >    With Expo, you can have the Expo Go app installed in your mobile and connect over the same network and get your app tested on any physical device [both Android and iOS].

### Done Features:
#### 1.  **Membership [Registeration / Login]:**
![image](https://github.com/meh-land/Dr_Reports/assets/79084467/8459a415-4ff1-4090-91c1-282b3c87df55)
![image](https://github.com/meh-land/Dr_Reports/assets/79084467/224d7d6e-2c6b-407b-bf44-e86411b18691)
![image](https://github.com/meh-land/Dr_Reports/assets/79084467/4dcdec30-4234-47a5-b202-e5c7d73529fd)

#### 2. **User Profile:**
![image](https://github.com/meh-land/Dr_Reports/assets/79084467/efa751b2-5214-41ab-905d-a11c7ae34137)
![image](https://github.com/meh-land/Dr_Reports/assets/79084467/82bdc35e-a7ac-40ba-a8ad-b2fcd3e64521)
![image](https://github.com/meh-land/Dr_Reports/assets/79084467/2e292109-9957-45e4-b52f-6010369af636)
![image](https://github.com/meh-land/Dr_Reports/assets/79084467/b1603515-25ea-4a05-bd65-6510f506c30a)
![image](https://github.com/meh-land/Dr_Reports/assets/79084467/c15d9b2b-dbb4-4bd7-afaa-a804a6a0a573)

<!--************************************************************************************-->

## Backend

### Used Technology:
* ***PHP***
* ***MYSQL "DataBase"***

### Done Features:

* Create, View, Edit, Delete User.

<!--************************************************************************************-->
## Pi_LinuxROS_Ubuntu
This repository contains step-by-step instructions to set an Ubuntu Server 20.04 LTS running ROS 1 Noetic on the Raspberry Pi 4.


### RPI Imager
1. Choose Ubuntu Server 20.04 LTS.
2. DO NOT SET A DEFAULT WIFI NETWORK.
3. Set Hostname as raspberrypi.
4. Enable SSH - Use password authentication.
5. Username: pi - Password: 123
6. Set locale settings - Time zone: Africa/Cairo - Keyboard layout: us


### PuTTY - Serial Communication with Pi
1. Choose 'Serial' as the connection type.
2. In serial line, write COMx - Check the device manager to see which COM port you are using.
3. Speed: 115200.
4. Press `Open` and power up the Pi.


### Pi - on boot (MUST DO)
1. Disable unattended updates completely. 
   ```
   sudo apt remove unattended-upgrades
   ```
2. Connect an Ethernet cable to the Pi to have access to the internet.
3. Install nmcli to connect to wifi. 
   ```
   sudo apt install network-manager
   ```
4. Run these commands to connect to ESP network.
   ```
   nmcli radio wifi
   sudo nmcli dev wifi connect ourESP password ourESP123
   ```
5. Update and upgrade all packages.
   ```
   sudo apt update && sudo apt upgrade -y
   ```


### Pi - SSH Through PC
1. Since the Pi is connected on the ESP network, make sure your PC is also connected to it.
2. Open cmd on Windows or terminal on Linux.
3. Enter the following command:
   ```
   ssh pi@raspberrypi
   ```
4. You will be prompted to enter the password.
5. Voila!


### Pi - ROS 1 Noetic Setup (METHOD 1)
1. Setup the Pi to accept software from packages.ros.org
   ```
   sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
   ```
2. Set up your keys. Make sure `curl` is installed.
   ```
   curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
   ```
3. Run:
   ```
   sudo apt update
   ```
4. Install ROS-Desktop-Full.
   ```
   sudo apt install ros-noetic-desktop-full
   ```
5. Run this script to use ROS.
   ```
   source /opt/ros/noetic/setup.bash
   ```
6. OPTIONAL: Source the previous script on startup using `.bashrc`.
   ```
   echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
   source ~/.bashrc
   ```


### Pi - ROS 1 Noetic Setup (METHOD 2)
1. Run this single line command to install ROS 1 Noetic *BRUH!*
   ```
   wget -c https://raw.githubusercontent.com/qboticslabs/ros_install_noetic/master/ros_install_noetic.sh && chmod +x ./ros_install_noetic.sh && ./ros_install_noetic.sh
   ```
2. Run this single line command to uninstall ROS 1 Noetic.
   ```
   wget -c https://raw.githubusercontent.com/qboticslabs/ros_install_noetic/master/ros_uninstall_noetic.sh && chmod +x ./ros_uninstall_noetic.sh && ./ros_uninstall_noetic.sh
   ```

<!--************************************************************************************-->

## Embedded
In the past weeks we’ve been searching for controlling our robot’s motors with ROS as it’s more compatible with the rest of the layers we’re dealing with. 
### PWM controlling :-
First, we’re controlling speed of the DC motor of the prototype with PWM (Pulse Width Modulation) which its main idea is that it turns the digital signal into an analog signal by changing the timing of how long it stayed ON and OFF which measured by “duty cycle” parameter that used to describe the percentage of how long it stayed ON compared to how long it stayed OFF.

On a small scale for our prototype, it could be used for many reasons:
1. Speed control:
   - With PWM mode, the motor will have a much higher torque that helps in moving in the specified speed even with more load.
1. Power efficiency:
   * Transistors of PWM mode has low impedance and therefore, low voltage drop and low power dissipation.
1. Control circuit (MCU):
   + Easy to switch ON/OFF.
### PID controller :-
As a future plan, we want to control the motors with PID (Proportional – Integral – Derivative) controller, it’s the most common control algorithm and advanced over PWM.

The idea behind the PID controller is to read a sensor and continuously calculating the error value as the difference between the desired setpoint and the measured process variable and calculate the proportional, integral, and derivative responses and summing those 3 components (P, I and D) to compute the actuator output.

It’s used for closed loop systems – that’s our case – as it’s a process of reading sensors to provide constant feedback and calculating the desired actuator output.

<img width="545" alt="Screenshot 2023-12-16 224513" src="https://github.com/meh-land/Dr_Reports/assets/145927508/a60aa30a-f30c-45e5-8f96-83c5da53152c">

<!--************************************************************************************-->
## Hardware
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

<!--************************************************************************************-->

## Localization

### Introduction:
During the last sprint, the task of researching available localization methods emerged.
After checking available resources one interesting way was using ultrasonic waves to implement a GPS-inspired localization.

### What was done:
- Matlab audible communication was implemented and tested by recording on the phone then decoding on Matlab (SNR wasn't good enough)
- Ultrasonic wave generation using an avr-based controller

### What to do:
- Ultrasonic receiver using an arm-based controller to verify sender frequencies
- Implement the communication protocol over ultrasound and amplify the sender till the receiver can understand the data
- Use time division multiplexing between senders and unique signatures to determine TOF hence the distance between each beacon
- Find the best estimation of position based on available distances
  - Handle initial estimation of beacon positions  
  - Handle Non Coherent distances (due to varying sound speed)
