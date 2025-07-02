# ESP_32_SNIFFER

A compact handheld device inspired by the ESP32 Marauder, equipped with 2.4GHz capabilities for Wi-Fi and Bluetooth scanning. Built using an **ESP32-S3**, a **2.8" TFT display**, and an **nRF24 module**, this sniffer can perform real-time scans and log data to an SD card for later review.

---

## 🔍 Features

- **Wi-Fi Scanner**  
  Detects SSID, RSSI, and Channel

- **Bluetooth Scanner**  
  Scans for MAC addresses and RSSI

- **SD Card Logger**  
  Initialize SD card and view saved log files

- **2.4GHz Spectrum Scanner**  
  (Currently under refinement for improved accuracy)

---

## 🧰 Hardware Used

- **ESP32-S3 Development Board**
- **nRF24L01+ PA + LNA** (radio peripheral)
- **2.8" ILI9341 SPI TFT LCD**
- **Anker A1645 Nano Power Bank** (or any 5V/3A power source)
- **3D-Printed Case** (STL file included in repo)

---

## ⚙️ Software

- **IDE**: Arduino
- **Flashing Target**: ESP32-S3
- **Libraries Used**:
  - `Adafruit_GFX`
  - `Adafruit_ILI9341`
  - `WiFi.h`, `BluetoothSerial.h`
  - `SD.h`, `SPI.h`
  - And others bundled via the Arduino Library Manager

---

## 📸 UI Overview

Upon boot, the device presents a grid of icons:

- 📶 Wi-Fi Scan
- 📱 Bluetooth Scan
- 💾 SD Card Access
- 📡 Spectrum Scanner

> *More features and improvements are planned.*

---

## 📚 Acknowledgments

This project was inspired by [justcallmekoko/ESP32Marauder](https://github.com/justcallmekoko/ESP32Marauder). Check out his repository—it's a fantastic resource for similar tools and concepts.

---

## 🚧 Notes

- The spectrum scanner is functional but still being improved.
- Logging is reliable, but parsing tools for logs will be added soon.
- This project has been a long-term effort across a year with learning curves and roadblocks—feedback is welcome!

---

## 🖨️ STL File

The STL file for the 3D-printable case is included in the repo.

---

## License

MIT License (or your preferred one)
