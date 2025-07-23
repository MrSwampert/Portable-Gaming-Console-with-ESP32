# ArcadESP - The Open-Source Retro Gaming Handheld
Portable Gaming Console with ESP32-WROVER, TFT Display, and MicroSD Storage.

# Summary

ArcadESP is an open-source, portable, retro video game console. Its main utility is to emulate games from classic consoles (such as the NES) using an ESP32 microcontroller, which is a very cheap and powerful chip. The main goal of the project is to leave it as a development board, which allows programming it for more functions.

# Description:
The circuit is centered on an ESP32-WROVER-IE microcontroller. The main power supply for the system is 3.3V.
The design integrates several key peripherals for operation. It includes a TFT screen for graphics display, managed through multiple GPIO connections of the microcontroller. For user input, the system features a series of buttons, including direction controls (up, down, left, right), action buttons (Start, Select, A, B, L, R), and menu buttons, which connect to a PCF8574 I/O port expander.
Data storage is handled through a MicroSD card slot with push-out functionality, allowing the reading and writing of information. Additionally, the circuit incorporates an auto-reset section for the microcontroller. Test points (TP1, TP2, TP3, TP4) are also included for monitoring key voltages such as V_USB, V_BATT and 3.3V.

# Features:
**Processing Core:** **ESP32-WROVER-IE** module with a dual-core CPU, Wi-Fi, Bluetooth, and integrated PSRAM.

**Connectivity & Power:** **USB-B port** for power and programming via an onboard **CH340 USB-to-UART** controller.

**Power Management:** Includes an **LTC4054** Li-Ion battery charger and an **MIC5219 LDO regulator** for a stable 3.3V supply.

**Audio Subsystem:** Features an I2S Stereo DAC (**UDA1334ATS**), a **PAM8403 Class-D amplifier**, and a **3.5mm audio jack** output.

**User Interface:** **TFT color display** for visual output, accompanied by user input buttons and a status LED.

**External Storage:** **Micro SD card slot** for expandable data and media storage.

**I/O Expansion:** **PCF8574 I/O expander** to provide additional digital pins over the I2C bus.

# Applications: 
-	Retro Emulation Console (Main Application)
-	Portable Media Player
-	IoT Device and Control Tool
-	Development and Learning Platform (All in One)

**Entertainment:** Play classic video games on a device you built yourself.
 
**Education:** It's a fantastic tool for learning about electronics, microcontroller programming (in the Arduino IDE), and how software emulation works.
 
**Personal Project (DIY):** It offers the satisfaction of building a functional gadget from scratch, with a very low cost (less than $20, according to similar projects).

# In Terms of Gaming:

Releases are here **https://github.com/retro-esp32/RetroESP32/releases**

It includes 11, YES eleven emulators.

 - Nintendo Entertainment System
 - Nintendo Game Boy
 - Nintendo Game Boy Color
 - Sega Master System
 - Sega Game Gear
 - Colecovision
 - Sinclair Zx Spectrum 48k
 - Atari 2600
 - Atari 7800
 - Atari Lynx
 - PC Engine

# Sector Focus:
The project is clearly focused on the maker or DIY sector. The target audience are:
 
**Students and Electronics Hobbyists:** People who want to put their hardware and software knowledge into practice.

**Retro Gaming Enthusiasts:** Nostalgic gamers who would enjoy not only playing, but also building their own console.
 
**Programmers and Developers:** Those interested in developing software for embedded systems and optimizing code for hardware with limited resources. (For example, **PICO-8** is a virtual machine that emulates a video game console. While it is impossible to replicate with **ESP32**, there are alternatives such as **Fake-8**, which is the best open source way to run **PICO-8** games on unsupported platforms).

This is not a product for the end consumer looking for an **“out-of-the-box”** console, but for someone who values the process of creation and customization.

The differential value of ArcadESP is its low cost, the use of the versatile ESP32 and its open-source nature, which invites a community to modify, improve and share their own versions.


# Power Budget:
<img width="3634" height="1969" alt="Power Budget" src="https://github.com/user-attachments/assets/ab43c390-9d30-4ec4-90c7-0904e69b9eae" />


# Block Diagram:
![Block Diagram](https://github.com/user-attachments/assets/a2732f13-642e-495d-99c7-92f5d1fba33b)


# Schematic
![Schematic_v1_page-0001](https://github.com/user-attachments/assets/21245f79-7f60-4261-9b1f-8e48e182f1de)


![Schematic_v1_page-0002](https://github.com/user-attachments/assets/f9dc21a0-e96c-4544-b652-97c719ce0494)


# 3D Model:
<img width="993" height="508" alt="image" src="https://github.com/user-attachments/assets/94d55f6d-f18f-4131-ae3e-d24e379275e0" />


<img width="993" height="508" alt="image" src="https://github.com/user-attachments/assets/fda1bbd3-08d8-44e4-8f9b-b54431d6933b" />


# References:

Pebri, “GitHub - pebri86/esplay_micro_hardware: Micro version of esplay hardware, ESP32 based gaming console,” GitHub. **https://github.com/pebri86/esplay_micro_hardware**

“ESPLay Micro V2,” Handheld ESP32 Game Console | Makerfabs. **https://www.makerfabs.com/esplay-micro-v2.html** 

Pebri, “GitHub - pebri86/esplay-retro-emulation: Retro Emulation Collection for ESPlay Hardware, an ESP32 based game console,” GitHub. **https://github.com/pebri86/esplay-retro-emulation**

Pebri, “GitHub - pebri86/esplay-micro-firmware-collections: Firmware files collections (*.fw) for ESPlay Micro,” GitHub. **https://github.com/pebri86/esplay-micro-firmware-collections**

Jtothebell, “GitHub - jtothebell/fake-08: A Pico-8 player/emulator for console homebrew,” GitHub. **https://github.com/jtothebell/fake-08**
