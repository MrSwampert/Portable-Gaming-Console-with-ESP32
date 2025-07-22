# ArcadESP - The Open-Source Retro Gaming Handheld
Portable Gaming Console with ESP32-WROVER, TFT Display, and MicroSD Storage


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

# Power Budget:
<img width="3634" height="1969" alt="Power Budget" src="https://github.com/user-attachments/assets/ab43c390-9d30-4ec4-90c7-0904e69b9eae" />


# Block Diagram:
![Block Diagram](https://github.com/user-attachments/assets/a2732f13-642e-495d-99c7-92f5d1fba33b)

# 3D Model:
<img width="993" height="508" alt="image" src="https://github.com/user-attachments/assets/94d55f6d-f18f-4131-ae3e-d24e379275e0" />


<img width="993" height="508" alt="image" src="https://github.com/user-attachments/assets/fda1bbd3-08d8-44e4-8f9b-b54431d6933b" />


# References:

Pebri, “GitHub - pebri86/esplay_micro_hardware: Micro version of esplay hardware, ESP32 based gaming console,” GitHub. **https://github.com/pebri86/esplay_micro_hardware**

“ESPLay Micro V2,” Handheld ESP32 Game Console | Makerfabs. **https://www.makerfabs.com/esplay-micro-v2.html** 

Pebri, “GitHub - pebri86/esplay-retro-emulation: Retro Emulation Collection for ESPlay Hardware, an ESP32 based game console,” GitHub. **https://github.com/pebri86/esplay-retro-emulation**

Pebri, “GitHub - pebri86/esplay-micro-firmware-collections: Firmware files collections (*.fw) for ESPlay Micro,” GitHub. **https://github.com/pebri86/esplay-micro-firmware-collections**

