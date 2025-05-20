# dhamalavirus

most important kura chai k ho vhane ni when you flash the payload it automatically starts on your computer so to prevent that i have mentioned below but but but when it is flashed and if we want another project to do you have to use the file name flash_nuke.uf2 (this file is for formating or wiping eintire pi pico and make fresh) 

 flash_nuke.uf2 this file is in our list so search for it and simply press bootsel button and connect to a pc and just daragg and dropp the file into it. thats it. 
# if you want a reverse 
there is a payload and powershell script above payload.ps1 copy and make a folder inside  linux machine in /var/www/html and make a file name payload.ps1 using nano. now you have to start server of python in 80 port and listen to the port using netcat using -lvp port 
# DhamalaVirusDucky
Build a Budget-Friendly but Powerful USB Rubber Ducky Using a Raspberry Pi Pico

# Quick Start Guide
Get your DhamalaVirusDucky up and running in under 5 minutes!

# Step 1: Download and Plug In
Go to the Releases page and download the latest version.

Connect your Raspberry Pi Pico (or variant) to your computer while holding the BOOTSEL button.

It will appear as a removable drive named RPI-RP2.

# Step 2: Install CircuitPython
Depending on your board, copy the appropriate .uf2 file to RPI-RP2:

For Raspberry Pi Pico:
adafruit-circuitpython-raspberry_pi_pico-en_US-9.2.1.uf2

For Pico W:
adafruit-circuitpython-raspberry_pi_pico_w-en_US-9.2.1.uf2

For Pico 2:
adafruit-circuitpython-raspberry_pi_pico2-en_US-9.2.1.uf2

For Pico 2W:
adafruit-circuitpython-raspberry_pi_pico2_w-en_US-9.2.1.uf2

After copying, the device will reboot and reappear as CIRCUITPY.

# Step 3: File Setup on CIRCUITPY
Copy the entire lib folder to the root of CIRCUITPY.

Copy all *.py script files to the root of CIRCUITPY.

Follow the instructions in the README.md to complete setup.

Place your payload file as payload.dd in the root directory.

# Step 4: Activate DhamalaVirusDucky
Disconnect your Pico from the USB port.

Remove the setup jumper (if used).

Plug it into your target machine. The DhamalaVirusDucky will now execute the payload automatically.

Setup Mode (Safe Editing Mode)
To prevent the DhamalaVirusDucky from running payloads on your own system during development:

Bridge pin 1 (GP0) and pin 3 (GND) using a jumper wire. or mera vhai baini ho tya aauta (Bootsel) vhanne button huna sakxa tesma dabawo. 

This enters setup mode, which disables payload execution and allows safe editing.

This is the easiest and safest way to modify your payloads without accidental execution.
