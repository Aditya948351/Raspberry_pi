# Raspberry_pi

<p>Train your Raspberry Pi to recognize you and others.</p>


<h2>What You’ll Need for Raspberry Pi Facial Recognition</h2>
 - Raspberry Pi 3 or 4. (Raspberry Pi Zero W is not recommended for this project.) </p>
 - You will need to install Bullseye OS for this (need python 3.9)
    - 64 bit : https://downloads.raspberrypi.com/raspios_oldstable_arm64/images/raspios_oldstable_arm64-2024-10-28/2024-10-22-raspios-bullseye-arm64.img.xz
    - 32 bit : https://downloads.raspberrypi.com/rpd_x86/images/rpd_x86-2022-07-04/2022-07-01-raspios-bullseye-i386.iso
 - Power supply/microSD/Keyboard/Mouse/Monitor/HDMI Cable (for your Raspberry Pi) </p>
 - Raspberry pi Camera</p>

 1.open a Terminal. </p>
 2. Install OpenCV by running the following commands in your Terminal.
 <li>
    Copy and paste each command into your Pi’s terminal, press Enter, and allow it to finish before moving onto the next command. <li>
    If prompted, “Do you want to continue? (y/n)” press y and then the Enter key.

  
# Terminal Commands and Execution Times

|                         | Terminal Command                                                                                     | Length of Time to Run   |
|-------------------------|-----------------------------------------------------------------------------------------------------|-------------------------|
| 1                       | `sudo apt install cmake build-essential pkg-config git`                                             | A few seconds           |
| 2                       | `sudo apt install libjpeg-dev libtiff-dev libjasper-dev libpng-dev libwebp-dev libopenexr-dev`      | A few seconds           |
| 3                       | `sudo apt install libavcodec-dev libavformat-dev libswscale-dev libv4l-dev libxvidcore-dev libx264-dev libdc1394-22-dev libgstreamer-plugins-base1.0-dev libgstreamer1.0-dev` | 4 minutes               |
| 4                       | `sudo apt install libgtk-3-dev libqtgui4 libqtwebkit4 libqt4-test python3-pyqt5`                   | 4.5 minutes             |
| 5                       | `sudo apt install libatlas-base-dev liblapacke-dev gfortran`                                       | 1 minute                |
| 6                       | `sudo apt install libhdf5-dev libhdf5-103`                                                         | 1 minute                |
| 7                       | `sudo apt install python3-dev python3-pip python3-numpy`                                           | A few seconds           |




