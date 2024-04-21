# System Outline

<!--PUT STACK OVERVIEW HERE-->

# Server
- Currently the server is able to run the dashboard and send data reliably to the robot using ROS scripts
<!--PUT SCREENSHOT OF DASHBOARD SENDING ROS MESSAGES HERE-->

<!--PUT DOCKER PHOTO HERE-->
- We are working on dockerizing the entire stack:
    - Frontend: done
    - Backend: done
    - Database: In progress
# PI
- Currently Raspberry pi runs the backend of the Dashboard, this is done to increase reliability, the tradeoff is performance.

- All ROS scripts run on the PI to circumvent dealing with UDP.

# Misc Infrastructure
Working on WiFi Localization.

<!--PUT FIGURE OF WIFI LOCALIZATION HERE-->