# NerdMiner CYD web installer

Installs the NerdMiner CYD firmware (lite edition) on an ESP32-2432S028 board from Chrome or Edge over USB:
https://sfttech2000.github.io/nerdminer-cyd-flasher/

Only the installer page and firmware images live here. boot.bin goes to 0x0 and the app image to 0xe000;
NVS (Wi-Fi and settings) is kept unless Erase is ticked.

Uses ESP Web Tools 10.4.0 (Apache-2.0), vendored in esp-web-tools/ with its licence.
