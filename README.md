# Raspberry Pi Facial Recognition Setup Guide

## What You’ll Need

- **Raspberry Pi 3 or 4** (Raspberry Pi Zero W is not recommended).
- **Operating System:** Install Bullseye OS (Python 3.9 is required):
  - [32-bit Download](https://downloads.raspberrypi.com/rpd_x86/images/rpd_x86-2022-07-04/2022-07-01-raspios-bullseye-i386.iso)
- **Hardware:**
  - Power supply
  - MicroSD card
  - Keyboard and mouse
  - Monitor
  - HDMI cable
  - Raspberry Pi Camera

## Steps to Install OpenCV on Raspberry Pi

### Step 1: Open a Terminal
Run the following commands sequentially in the terminal. For each command:

1. Copy and paste it into the terminal.
2. Press **Enter** to execute.
3. If prompted with “Do you want to continue? (y/n),” type **y** and press **Enter**.

  
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



## Modifying Swap Memory

To expand the swapfile, follow these steps:

1. Open the `dphys-swapfile` for editing:
   ```bash
   sudo nano /etc/dphys-swapfile
<p></p>
<div style="text-align: center;">
    <img src="https://github.com/Aditya948351/Raspberry_pi/blob/main/step4.png?raw=true" alt="Step 4 Image" width="600">
</div>

Press Ctrl-X, Y and then Enter to save your changes to dsudo phys-swapfile.

### Setup Script for Face Recognition

Copy and Paste this script in your command promt this may take around 20 minutes:

<h2>Step 1: Restart the swapfile</h2>
    <pre><code>sudo systemctl restart dphys-swapfile</code></pre>
    
<h2>  Step 2: Install face_recognition (this may take around 19 minutes)</h1>  
    <pre><code>pip install --no-cache-dir face-recognition</code></pre>
    
<h2>Step 3: Install imutils</h2>
    <pre><code>pip install imutils</code></pre>


<h2>Step 4: Enable Camera from your Raspberry Pi configuration follow below steps:</h2> 

1. Open the Raspberry Pi configuration menu by running the following command in the terminal:
   ```bash
   sudo raspi-config

1. Open the Raspberry Pi configuration menu:
   ```bash
   sudo raspi-config
2. Navigate to Interface Options.

3. To enable the Legacy Camera: </li>
      Advanced Options > Legacy Camera > Enable

4. Exit and reboot your Raspberry Pi using:
'''bash
sudo reboot


<h2>Step 5: Install Picamera</h2>
    <pre><code>pip install picamera[array]</code></pre>


https://youtu.be/DUGZC-tNm2w?si=eRe6BMFwn5BSEV5c


follow this yt tutorial: https://youtu.be/QzVYnG-WaM4?si=UrQi-QILrg8s3LyJ
    
