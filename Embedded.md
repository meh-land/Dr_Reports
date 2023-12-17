# Overview
In the past weeks we’ve been searching for controlling our robot’s motors with ROS as it’s more compatible with the rest of the layers we’re dealing with. 
## PWM controlling
First, we’re controlling speed of the DC motor of the prototype with PWM (Pulse Width Modulation) which its main idea is that it turns the digital signal into an analog signal by changing the timing of how long it stayed ON and OFF which measured by “duty cycle” parameter that used to describe the percentage of how long it stayed ON compared to how long it stayed OFF.

On a small scale for our prototype, it could be used for many reasons:
1. Speed control:
   - With PWM mode, the motor will have a much higher torque that helps in moving in the specified speed even with more load.
1. Power efficiency:
   * Transistors of PWM mode has low impedance and therefore, low voltage drop and low power dissipation.
1. Control circuit (MCU):
   + Easy to switch ON/OFF.
## PID controller
As a future plan, we want to control the motors with PID (Proportional – Integral – Derivative) controller, it’s the most common control algorithm and advanced over PWM.

The idea behind the PID controller is to read a sensor and continuously calculating the error value as the difference between the desired setpoint and the measured process variable and calculate the proportional, integral, and derivative responses and summing those 3 components (P, I and D) to compute the actuator output.

It’s used for closed loop systems – that’s our case – as it’s a process of reading sensors to provide constant feedback and calculating the desired actuator output.

<img width="545" alt="Screenshot 2023-12-16 224513" src="https://github.com/meh-land/Dr_Reports/assets/145927508/a60aa30a-f30c-45e5-8f96-83c5da53152c">
