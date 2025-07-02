# CYBER_DECK

The Cyber_Deck is a portable, customizable computing system housed in a weatherproof case. It is built around a Raspberry Pi 5 and designed for independent security auditing and wireless experimentation. The system includes a 10-inch touchscreen, 2TB NVMe SSD for storage, and a 65,000mAh power bank. Running Kali Linux, it supports Wi-Fi and SDR-based testing and monitoring.

---

## Hardware Components

- Raspberry Pi 5 (8GB RAM)
- Official Raspberry Pi 5 Active Cooler with aluminum heatsink and blower
- 10.1" IPS LCD Touchscreen Display (1024x600 resolution)
- 2TB Crucial P3 NVMe SSD in a Dockteck USB 3.2 tool-free enclosure
- 65,000mAh power bank with USB Power Delivery (22.5W)
- MEIJIA all-weather waterproof protective case (15.98" x 12.99" x 6.85")
- Panel-mounted and short cables:
  - Micro HDMI to HDMI (90° angled)
  - USB 3.0 male to female extensions
  - USB-C male to female extension
  - RJ45 Ethernet extension (panel mount)
  - 3.5mm stereo audio extension

---

## Wireless and Radio Adapters

- NooElec Smart V5 SDR for radio frequency analysis
- Panda Wireless PAU0F AXE3000 WiFi 6E adapter (supports monitor mode)

Note: Various online tutorials are available for configuring these adapters with GQRX, GNU Radio, and Airmon-ng.

---

## Power Management Considerations

- The Raspberry Pi 5 requires ~27W during boot. To ensure smooth operation without manual intervention, set `max_current_enable=1` in `config.txt`.
- USB PD-compatible power banks are recommended to handle high current demand.
- If using a power bank without a hardware switch, a kill switch can be added inline between the battery and PCB. Only perform such modifications if properly trained, as lithium-ion batteries can be hazardous.

---

## Software and Offline Tools

- **Kiwix** for offline access to large information repositories such as Wikipedia (via ZIM files)
- **Ollama** for running lightweight local LLMs through the terminal
- **Kali Linux** full penetration testing suite

Be sure to update your system before disconnecting from the internet:

```bash
sudo apt update && sudo apt upgrade -y
