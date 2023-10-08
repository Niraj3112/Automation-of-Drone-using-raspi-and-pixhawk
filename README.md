# Autonoumous-of-Drone-using-raspi-and-pixhawk
## Project Overview

This project focuses on making a drone autonomous using a Raspberry Pi and a Pixhawk flight controller. By following the steps outlined below, you will be able to set up your drone for autonomous flight, allowing it to take off, reach a specified altitude, hover, and then land autonomously.

**Hardware Requirements**
- Raspberry Pi (RPi)
- Pixhawk Flight Controller
- Drone (compatible with Pixhawk)
- Laptop/Desktop for development
**Software Requirements**
- Raspberry Pi OS (64-bit)
- Mission Planner (for Pixhawk configuration)
- Automation script for autonomous flight
## Raspberry Pi Setup
1. Install a 64-bit Raspberry Pi OS on a 32GB microSD card using the Raspberry Pi Imager, which can be downloaded from [here](https://www.raspberrypi.com/software/).
2. Configure VNC to connect your Raspberry Pi with your laptop.
3. Install the required libraries on the Raspberry Pi. These libraries are necessary for interfacing with the Pixhawk and implementing autonomous flight features.
   - Python libraries: python3-dev, python3-opencv, python3-wxgtk4.0, python3-pip, python3-matplotlib, python3-lxml, python3-pygame
   - Python packages: PyYAML, mavproxy (user installation), pymavlink, mavproxy, dronekit
4. Enable the Raspberry Pi's serial port and disable serial control
   In the configuration menu, navigate to Interfacing Options > Serial and select "No" to disable serial login and "Yes" to enable the hardware serial interface. Afterward, reboot your Raspberry Pi.

## Mission Planner Configuration

1. Open Mission Planner and configure the baud rate of telemetry2 to 921600.

## Autonomous Operation

With the Raspberry Pi properly configured and connected to Pixhawk, you can now proceed with autonomous operations:
1. Ensure your drone is in Guided mode.
2. Place the provided automation script on your Raspberry Pi.
3. Position your drone in a flyable area.
4. Execute the automation script as instructed.
The provided automation script will initiate autonomous flight, instructing the drone to take off, reach a specified altitude (e.g., 15 meters), hover, and eventually land autonomously.

By following these steps, you'll have successfully set up your drone for autonomous flight using a Raspberry Pi and Pixhawk, making it ready for various applications and missions.
