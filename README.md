# Patio-Heater-Controller
Homebridge based controller for an infrared heater.

## Components

* Raspberry Pi 0W
* [CZH labs](https://chz-labs.com) [DIN mount relay module](relay) (5 x SPST-NO)

## Software Setup (from scratch)

1. Install Raspberry Pi OS (Raspbian)
2. Boot
3. Install Homebridge using the instructions found here: [Install Homebridge on Raspbian](install-hb).
4. After the install completes, connect to the Homebridge UI on port 8581 (e.g., patioheater.local:8581).

[relay]: <https://www.czh-labs.com/tmp/madeimg/datasheet/d-1368.pdf>
[install-hb]: <https://github.com/homebridge/homebridge/wiki/Install-Homebridge-on-Raspbian>
