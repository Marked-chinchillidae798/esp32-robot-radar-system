# 🤖 esp32-robot-radar-system - Real-Time Radar Visualization Tool

[![Download](https://img.shields.io/badge/Download-esp32--robot--radar--system-ff6f61?style=for-the-badge)](https://github.com/Marked-chinchillidae798/esp32-robot-radar-system)

## 📋 About esp32-robot-radar-system

This is an ESP32-based robotic radar system. It uses ultrasonic sensors to detect objects. A servo motor moves the sensor to scan the surrounding area. The data shows up in real-time on a web dashboard using your browser. This lets you see what the radar senses without special software.

The main goal is to offer a simple way to build and use a radar on ESP32 boards. It mixes hardware and software for a clear view of your environment. No advanced skills are needed to get started.

The system works by:
- Sending ultrasonic pulses.
- Measuring the time for echoes to return.
- Moving the sensor with a servo motor to cover an area.
- Showing detected objects on a web page via WiFi.

## 🖥️ What You Need

Before you begin, make sure you have these things:

- A Windows PC with internet access.
- A modern web browser such as Chrome, Firefox, or Edge.
- An ESP32 board connected to the radar hardware (ultrasonic sensor and servo motor).
- WiFi network for the ESP32 to connect to.
- USB cable to connect ESP32 to your PC (used for setup if needed).

The PC must run at least Windows 7 or newer.

## 🔧 Hardware Overview

The system uses:

- **ESP32** microcontroller: handles sensor data and WiFi.
- **Ultrasonic sensor**: measures distance to obstacles.
- **Servo motor**: moves the sensor for scanning.
- **WiFi network**: sends data from the ESP32 to your browser.
- A power supply for the ESP32 board (usually USB).

If you build the hardware, connect everything as per your ESP32 radar project guide. If you already have the hardware, proceed to software setup.

## 🌐 Download and Install the Software

### Step 1: Visit the Download Page

Click the big download badge above or click here to visit the GitHub page where you can get the software:

https://github.com/Marked-chinchillidae798/esp32-robot-radar-system

This page contains all available files, instructions, and updates.

### Step 2: Download the Software

You will find source code and prebuilt files on the GitHub page. For typical users:

- Look for a folder or release marked as "Prebuilt" or "Binary."
- Download the latest `.bin` or `.hex` file for the ESP32.
- If you want to try the web visualization on your PC first, instructions are given on the page.

### Step 3: Install ESP32 Drivers (If Needed)

If Windows does not recognize your ESP32 board when you plug it in, you may need to install drivers.

- Visit this link to get drivers:

  https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers

- Follow the simple installer instructions.

### Step 4: Flash the Software to ESP32

To load the software onto your ESP32, you will need a program called **ESP32 Flash Tool**.

- Download the installer here:

  https://dl.espressif.com/dl/esp-idf-tools-setup-2.3.exe

- Run the installer and open the flashing app.
- Connect your ESP32 board using the USB cable.
- Select the `.bin` file you downloaded from the GitHub repository.
- Click "Flash" or "Start" to upload the software.

The board will restart automatically once flashing finishes.

### Step 5: Connect ESP32 to WiFi

After flashing, the board will create a WiFi hotspot or try to connect to your home network.

- Use your phone or PC to find the ESP32 hotspot named something like `ESP32-Radar`.
- Connect to it.
- Open your browser and go to `192.168.4.1` (default address) to configure your WiFi.
- Enter your home WiFi name and password.
- Save and restart the ESP32.

Now the board will connect to your home WiFi network.

## 🚀 Running the Radar System

### Step 1: Find the ESP32 IP Address

Once connected to your home network, you need the ESP32's IP address.

- Open your router's admin page and look for connected devices.
- Look for a device named similar to `ESP32-Radar`.
- Note the IP address.

### Step 2: Open the Web Dashboard

On your Windows PC, open your preferred web browser.

Type this address in the browser, replacing `xxx.xxx.xxx.xxx` with the IP address you found:

http://xxx.xxx.xxx.xxx

This page shows the radar's live view.

### Step 3: Use the Radar Web View

You will see a graphical display of the scanned area. As the servo moves the sensor, obstacles appear in real-time.

You can:

- Watch objects detected by ultrasonic sensors.
- See their relative position around the radar.
- Refresh or reconnect if needed.

## ⚙️ Adjusting Settings

If you want to change how the radar works, you can edit the configuration files on the ESP32 before flashing, or use the dashboard if enabled.

Typical settings include:

- Scan angles of the servo motor.
- Scan speed (how fast it moves).
- Sensitivity of the ultrasonic sensor.
- WiFi network info.

For most users, default settings will work well.

## 🔗 Repository Topics and Details

This project covers:

- Embedded systems and IoT with ESP32.
- Robotics sensor integration and control.
- Real-time data display on web dashboards.
- Ultrasonic distance measuring.
- Servo motor scanning.
- Using WiFi for hardware communication.

## 🛠️ Troubleshooting

If the system does not work as expected:

- Make sure your ESP32 board is powered and connected.
- Check that you flashed the correct firmware file.
- Confirm the ESP32 connects to your WiFi.
- Ensure your browser accesses the correct IP address.
- Try restarting the ESP32 and your PC.

For help, review the GitHub repository issues section or reach out to community forums.

## 📥 Download Again or Get Updates

You can always return to this page and click the download badge below to get the latest version or updated files:

[![Download](https://img.shields.io/badge/Download-esp32--robot--radar--system-ff6f61?style=for-the-badge)](https://github.com/Marked-chinchillidae798/esp32-robot-radar-system)