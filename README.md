# Patio-Heater-Controller
Homebridge based controller for an infrared heater.

## Components

* Raspberry Pi 0W
* [CZH labs](https://chz-labs.com) [DIN mount relay module](relay) (5 x SPST-NO) - relay 1 on GPIO 5 and relay 2 on GPIO 6 are used to control the DPDT relays.
* 2 - DPDT relays (DIN mount)
* Mean Well DIN mount 5V power supply
* Enclosure

## Software Setup (from scratch)

1. Install Raspberry Pi OS (Raspbian)
2. Boot
3. Install Homebridge using the instructions found here: [Install Homebridge on Raspbian](install-hb).
4. After the install completes, connect to the Homebridge UI on port 8581 (e.g., patioheater.local:8581).
   * You'll be prompted to create a Homebridge user and set a password. If you use a random password (e.g., one generated for you by Safari) be sure to save it as Safari (at least) does not recognize that you're setting a password that it should put into your keychain.
6. Check the logs and update Node if necessary.
7. Add [homebridge-rpi](homebridge-rpi) plugin
8. After adding the homebridge-rpi plugin, enable and start the pigpiod service
9. Configure the homebridge-rpi plugin to create a switch Accessory for each heating element.

[relay]: <https://www.czh-labs.com/tmp/madeimg/datasheet/d-1368.pdf>
[install-hb]: <https://github.com/homebridge/homebridge/wiki/Install-Homebridge-on-Raspbian>
[homebridge-rpi]: <https://github.com/ebaauw/homebridge-rpi>
