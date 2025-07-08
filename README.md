# ESP32_SNIFFER

A compact handheld ESP32-S3-based wireless sniffer with a 2.8" TFT touchscreen, nRF24L01+ antenna, and onboard SD card logging. Designed to monitor WiFi and Bluetooth MAC addresses and signal strength across channels, with a simple touchscreen UI and self-contained operation.

# FEATURES

- Scan for 2.4GHz WiFi MAC addresses
- Channel hopping and RSSI detection
- Bluetooth device scanning
- Save logs to SD card for later analysis
- Touchscreen GUI with simple navigation
- Fully portable and battery-powered

# COMPONENTS

- ESP32-S3 Dev Board (with dual USB-C)
- 2.8" TFT Capacitive Touch Display
- nRF24L01+ Antenna Module (2.4GHz)
- SD Card Reader (up to 64GB supported)
- Anker Portable Battery (for mobile power)
- 3D Printed Enclosure (optional)
- Supporting components: jumper wires, breadboard, headers

# SOFTWARE

- Developed in Arduino IDE using the following libraries:
  - `TFT_eSPI`
  - `ESP32SPISlave`
  - `SD_MMC`
  - `WiFi`
  - `BluetoothSerial`

The project is fully offline-capable. Data is logged to the SD card and can be analyzed using a separate host system.


<div align="center">
  <img width="500" alt="GUI Screenshot" src="https://github.com/user-attachments/assets/e06d5231-c049-4c7e-b2e3-51d6adc0e85b" />
  <img width="500" alt="ESP32 Sniffer Breadboard" src="https://github.com/user-attachments/assets/70359836-4e6d-46f8-b5ff-962e30f79daa" />
  <img width="500" alt="ESP32 Sniffer Final Build" src="https://github.com/user-attachments/assets/92ad93bb-2bfe-4722-b8ae-84bd190e09df" />
</div>

---
