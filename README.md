<!--# FPGA_controlling_APP
這是一個用Android studio以及java開發的APP，並以藍芽模組HC-05與UART技術控制FPGA

# Features
APP介面如下：<br> 

![](https://github.com/rrrjjj2019/FPGA_controlling_APP/raw/master/readme_img/app.png)<br>
Button有以下幾種:<br>
  - Auto: 車子自動前行，前方有障礙物時，後退、左轉、再前行。<br>
  - Manual: 於手機控制上、下、左、右(default mode)。<br> 
  - Bluetooth On / Off: 開啟/關閉手機藍芽。<br>
  - Discover new devices: 搜尋附近藍芽裝置。<br>
  - Show paired devices: 秀出已被對裝置。<br>
  - UP/DOWN/LEFT/RIGHT/STOP: 控制車子的前進/後退/左轉/右轉/煞車。<br>
-->

# FPGA Controlling App 📱🔗

This Android application serves as a **wireless controller for an FPGA-based car** via Bluetooth (HC-05) and UART communication.  
It was developed using **Android Studio (Java)** as part of an integrated project combining **mobile software development, embedded systems, and digital hardware design**.

---

## 🎯 Project Goals
- Provide a **user-friendly smartphone interface** to control FPGA hardware.  
- Implement **manual driving** and **autonomous navigation trigger** modes.  
- Enable robust Bluetooth communication for real-time control.  
- Demonstrate cross-domain integration of **mobile software** and **FPGA hardware**.

---

## 🖼️ App Interface
The control interface is shown below:  

![App Screenshot](https://github.com/rrrjjj2019/FPGA_controlling_APP/raw/master/readme_img/app.png)

---

## 🔧 Features
- **Manual Mode**: Control FPGA car with UP / DOWN / LEFT / RIGHT / STOP buttons.  
- **Auto Mode**: Activate FPGA’s autonomous driving (IR-based obstacle avoidance).  
- **Bluetooth On / Off**: Toggle smartphone Bluetooth module.  
- **Discover New Devices**: Scan for nearby Bluetooth devices.  
- **Show Paired Devices**: Display already paired devices.  

---

## 🚀 Technical Overview
- **Frontend**: Android Studio, Java-based UI with onClick event handling.  
- **Backend**: Bluetooth serial communication via HC-05 module.  
- **Protocol**: Encodes button presses into predefined command strings, which are decoded by FPGA (Verilog UART receiver).  
- **Integration**: Commands map to FPGA states that control stepper motor direction and enable signals.  

---

## ⚡ Key Contributions
- Designed a **lightweight communication protocol** between Android and FPGA.  
- Implemented a **real-time Bluetooth control system** with minimal latency.  
- Bridged **software-hardware co-design**, showcasing ability to integrate mobile applications with embedded digital systems.  

---

## 📚 Future Improvements
- Expand to multi-platform support (iOS + Android).  
- Add **sensor feedback visualization** (e.g., IR detection status displayed in app).  
- Upgrade to BLE (Bluetooth Low Energy) for better efficiency.  