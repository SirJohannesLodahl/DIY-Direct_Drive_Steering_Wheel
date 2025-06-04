# DIY-Direct_Drive_Steering_Wheel
Building My Own Force Feedback Steering Wheel with FFbeast – A DIY Journey

This is a full deep dive into my DIY force feedback steering wheel project, powered by the open-source firmware FFbeast. 

My goal is to create a clean, responsive, fully 3d printable and modular setup that feels like a professional direct-drive system – but built entirely by myself, with full control over both hardware and software. From CAD modeling and 3D printing, to programming low-power wireless communication protocols on the ESP32 – I’m documenting every step.



This project is meant to be as open and educational as possible. If you’re working on a similar setup, struggling with FFbeast configuration, or trying to build your own wireless button system – feel free to contact me! I’m happy to share what I’ve learned and would love to hear about your builds as well.

You can open an issue, start a discussion, or reach out directly via 
Instagram [@johannes.ldhl](https://www.instagram.com/johannes.ldhl/#)
Youtube [@Johannes Lodahl](https://www.youtube.com/@johanneslodahl7738)
Discord @sirjolo_6090
Feel free to reach out!

Let’s dive right in.



## 🧰 Step-by-Step Guide

A complete walkthrough from hardware to firmware.

---

### ✅ 1. Prepare Your Workspace

* Clear a safe, static-free workbench
* Gather tools (screwdrivers, soldering iron, multimeter, etc.)
* Install required software (see [Tools](#tools))

---

### ⚙️ 2. Assemble the Hardware

* Mount the motor and baseplate
* Connect the motor to the driver board
* Install the power supply and fuse
* Wire encoder and signal cables
* Optional: Add cooling or fan control

---

### 🚰 3. Build the Wheel Rim

* 3D print or assemble the wheel structure
* Mount buttons and shifters
* Install ESP32 and battery
* Wire buttons to GPIO pins
* Test charging setup (USB or wireless)

---

### 🔌 4. Flash the Firmware

#### FFbeast (Motor Controller)

* Download the latest FFbeast release
* Flash firmware to your controller (e.g. STM32, G431, ODrive...)
* Configure basic parameters (via USB or serial)

#### ESP32 (Wireless Rim)

* Clone this repo
* Open `/rim-fw` in PlatformIO or Arduino IDE
* Flash to your ESP32
* Test Bluetooth connection to PC

---

### ⚖️ 5. Configuration & Tuning

* Connect to FFbeast UI (via USB)
* Set motor type, encoder, and FFB strength
* Assign button mappings (if applicable)
* Fine-tune PID and filtering
* Save and back up config

---

### 🎮 6. Testing & Integration

* Connect system via USB to your PC
* Open a sim racing game (e.g. Assetto Corsa)
* Check for force feedback, button input, etc.
* Adjust firmware or game settings as needed
* Celebrate your first lap!

---

### 🧪 7. Troubleshooting

If things don't work:

* Re-check all power and ground connections
* Look at serial logs from FFbeast / ESP32
* Test each subsystem (motor, rim, buttons) separately
* Open an [Issue](https://github.com/...) or check the [Discussion](#)

---

### ⚒ Tools

| Tool               | Description                    | Link                                                          |
| ------------------ | ------------------------------ | ------------------------------------------------------------- |
| PlatformIO         | ESP32 development              | [https://platformio.org](https://platformio.org)              |
| FFbeast Config UI  | Tuning & flashing              | [https://github.com/FFbeast/](https://github.com/FFbeast/)... |
| KiCad / Fusion 360 | (If you modify PCB or housing) | -                                                             |


# Tools
Tool	Description	Link
PlatformIO	ESP32 development	https://platformio.org
FFbeast Config UI	Tuning & flashing	https://github.com/FFbeast/...
KiCad / Fusion 360	(If you modify PCB or housing)	-
