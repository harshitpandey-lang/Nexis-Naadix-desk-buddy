
# Nexis
<img width="1366" height="410" alt="model_nexis_2026-Jun-03_01-21-36AM-000_CustomizedView11682904690_png" src="https://github.com/user-attachments/assets/e82a30d5-a7dc-404a-8ee1-78e78ddcec3c" />

Nexis is a dual AI powered desk automation bot which uses raspberry pi to run a local llm and also uses a cloud deployed ai agent to do the tasks given to it in small chunks. We can give instructions through the interactive touch screen and also through the micophone. 
It uses esp32 to give commands to the device connected through the USB. 

## Overview

Nexis is a desk buddy which can do all sort of works upon good training and customisation. It uses a raspberry pi and open source AI model to break works into smaller steps. It uses the the local llm to generte the HID code respective to every step given uses python to asses if the work is performed then goes ahed with next step till all are completed. 
It uses esp32 to give HID code to the PC connected to make it do or perform a particular task. It can communicate or given instructionthrough the Touchscreen and Microphone.

## Project Goals

- Automate all the lame tasks and can be worked through while sleeping like a human would do.
- It will work as an ultimate assistant if customised and trained it can peroform any kind of work from editing 3d cad designing , coding and many more tasks.
- It can Interact to any computer or pc through the USB and work smoothly. So one can use a system with this assitant make make it do all their jobs.
- It can also be used to educate and elevate and it can work as jarvis in future.

---
## Specifications

| Parameters | Value |
| Code | Python|
| Hardware | Raspberry pi model B |
| Design | 3d printed and rubber keys|

### Hardware

* Raspberry Pi 4 Model B
* Official Raspberry Pi Display
* ESP32-S3
* INMP441 Microphone
* MAX98357A Amplifier
* Speaker
* Rotary Encoder
* Push Buttons
* LiPo Battery (Optional)

See BOM.md for the complete list.

---

## Software

### Raspberry Pi

Install:

* Raspberry Pi OS
* Python
* Git
* Required libraries

### ESP32

Install:

* Arduino IDE or PlatformIO
* ESP32 Board Package

---

# Step 1 — Clone Repositories

Clone:

```bash
git clone <oai-repository>
```

Clone:

```bash
git clone <nexis-repository>
```

---

# Step 2 — Prepare Raspberry Pi

Flash Raspberry Pi OS.

Connect:

* Display
* Keyboard
* Mouse

Perform:

```bash
sudo apt update
sudo apt upgrade
```

Install project dependencies.

---

# Step 3 — Configure OAI

Create environment file.

Add:

```text
API_KEY=
MQTT_SERVER=
```

Run test commands.

Verify OAI returns valid plans.

---

# Step 4 — Flash ESP32

Open:

```text
firmware/
```

Compile firmware.

Upload to ESP32-S3.

Verify:

* WiFi connection
* HID connection

---

# Step 5 — Manufacture PCB

Open:

```text
pcb/
```

Generate:

* Gerbers
* Drill Files
* BOM

Submit to PCB manufacturer.

---

# Step 6 — Assemble Hardware

Install:

* Raspberry Pi
* Display
* PCB
* Speaker
* Buttons
* Encoder

Complete wiring.

Verify power rails.

---

# Step 7 — System Test

Test:

### Audio

* Microphone
* Speaker

### Input

* Touchscreen
* Buttons
* Encoder

### Communication

* Pi ↔ ESP32

### HID

* Keyboard
* Mouse

---

# Step 8 — Final Validation

Test example commands:

```text
Open YouTube

Open Calculator

Search Google

Upload File
```

Verify:

* OAI response
* Approval screen
* HID execution

---

# Manufacturing Notes

The PCB included in this repository is an early revision.

Future revisions may change:

* Component placement
* Routing
* Connector locations

Always verify the latest schematic before ordering boards.

---

# Current Project State

Completed:

* OAI
* CAD Design
* PCB Design
* Documentation

In Progress:

* Firmware
* PCB Validation
* Physical Assembly

Planned:

* Manufacturing
* Testing
* Final Enclosure Revision

The repository represents the current development state and will continue evolving as physical prototypes are produced and tested.

---
<img width="874" height="1240" alt="WhatsApp Image 2026-06-04 at 8 46 59 AM" src="https://github.com/user-attachments/assets/b5e7b2c2-8e9a-4f77-adbe-37a7350d4056" />

---
