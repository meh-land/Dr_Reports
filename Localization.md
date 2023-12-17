Progress Update
17/12/2023

# Introduction:
During the last sprint, the task of researching available localization methods emerged.
After checking available resources one interesting way was using ultrasonic waves to implement a GPS-inspired localization.

# What was done:
- Matlab audible communication was implemented and tested by recording on the phone then decoding on Matlab (SNR wasn't good enough)
- Ultrasonic wave generation using an avr-based controller

# What to do:
- Ultrasonic receiver using an arm-based controller to verify sender frequencies
- Implement the communication protocol over ultrasound and amplify the sender till the receiver can understand the data
- Use time division multiplexing between senders and unique signatures to determine TOF hence the distance between each beacon
- Find the best estimation of position based on available distances
  - Handle initial estimation of beacon positions  
  - Handle Non Coherent distances (due to varying sound speed)
