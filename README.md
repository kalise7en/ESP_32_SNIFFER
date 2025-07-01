# ESP_32_SNIFFER
A small handheld device inspired by the ESP Maurader that has 2.4ghz capabilities along with Wifi and Bluetooth scanning. Using an Esp-32-S3 alongside a TFT 2.8 screen and a nrf24 module, the Sniffer can create logs of local scans and save them to a sd card for later use. 

Using Arduino for the IDE and flashing the build to the S3 model a grid of icons will appear. The WIFI and BLUETOOTH icons do general scans that include SSID, RSSI, CHANNEL for Wifi and MAC, RSSI for Bluetooth. The SD card logo allows you to initialize the card and see saved files to confirm. The last icon is for a spectrum scanner that I will be improving on as it's scanning process isn't terribly accurate. 

The whole project has took a year on an off hitting roadbocks through the process. Please check out justcallmekoko/ESP32Marauder his work is amazing.


PRODUCTS

ESP32-S3 Development board
nrf24l01 + pa + lna (radio peripheral)
ILI9341 2.8" SPI TFT LCD
Anker A1645 nano power bank (I used this one but you can power it with anything that can supply 5v/3A)
Case STL file in main.
