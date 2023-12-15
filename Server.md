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