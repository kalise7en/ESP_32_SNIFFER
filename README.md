# ESP_32_SNIFFER

The ESP_32_SNIFFER is a self‑contained handheld platform for 2.4 GHz monitoring.  
Built around an ESP32‑S3 microcontroller, an ILI9341‑based 2.8‑inch TFT display, and an nRF24L01+ PA / LNA transceiver, the device can scan Wi‑Fi and Bluetooth environments and record the resulting data to a microSD card.

---

## Features

| Function                | Output fields                                       |
|-------------------------|-----------------------------------------------------|
| Wi‑Fi scanner           | Service set identifier (SSID), received‑signal strength indicator (RSSI), channel |
| Bluetooth scanner       | Media‑access‑control (MAC) address, RSSI            |
| SD‑card logging         | Initialise card, browse and verify saved log files  |
| 2.4 GHz spectrum scan   | Experimental; accuracy improvements in progress     |

A graphical start screen presents four touch‑selectable icons corresponding to the functions above.

---

## Hardware

- ESP32‑S3 development board  
- nRF24L01+ PA / LNA transceiver module  
- ILI9341 2.8‑inch SPI TFT LCD  
- 5 V / 3 A power source (tested with an Anker A1645 Nano power bank)  
- Weather‑resistant printed enclosure (STL file supplied)

---

## Software

- Development environment: **Arduino IDE**  
- Core libraries:  

  | Library | Purpose |
  |---------|---------|
  | `Adafruit_GFX` / `Adafruit_ILI9341` | Display graphics |
  | `WiFi.h` | Wi‑Fi interface |
  | `BluetoothSerial.h` | Classic Bluetooth scanning |
  | `SD.h`, `SPI.h` | File system and SPI bus |
  | Additional support libraries via Arduino Library Manager |

Compile the sketch for the **ESP32‑S3** target, then flash via USB.

---

## Project Status

Development has been conducted intermittently over the past year.  
Current priorities:

1. Refinement of the spectrum‑scanner algorithm  
2. Addition of parsing and visualisation tools for saved log files  
3. General code refactoring and documentation

Contributions and issue reports are welcome.

---

## Acknowledgements

The project is inspired by, and makes reference to, the work in  
*justcallmekoko/ESP32Marauder* (GitHub).  
That repository remains an excellent reference for ESP32‑based wireless assessment.

---

## Licence

This project is released under the MIT Licence unless otherwise stated.

