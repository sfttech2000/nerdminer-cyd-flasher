# NerdMiner CYD web installer

Installs the NerdMiner CYD firmware (lite edition) on an ESP32-2432S028 board from a browser over USB:
computers with Chrome or Edge (Web Serial), Android phones with Chrome and an OTG cable (WebUSB):
https://sfttech2000.github.io/nerdminer-cyd-flasher/

Only the installer page and firmware images live here. boot.bin goes to 0x0 and the app image to 0xe000;
NVS (Wi-Fi and settings) is kept unless Erase is ticked.

Uses esptool-js 0.6.1 (Apache-2.0), vendored in mobile/esptool-js/ with its licence, and a small
CH340 driver over WebUSB (mobile/ch340-webusb.js) for Android, where Chrome's Web Serial lists
only Bluetooth devices.
