# tallyarbiter-esp8266-listener
ESP8266 / neopixel Tally Arbiter listener,  works with hardware setup of [vtally](https://wifi-tally.github.io/index.html)

## Flash
I've had issues flashing with the arduino IDE.  
I recommend using [nodeMCU-pyflasher](https://github.com/marcelstoer/nodemcu-pyflasher/releases)

## Setup

### Arduino board
On the additional boards manager URLs add http://arduino.esp8266.com/stable/package_esp8266com_index.json

### Arduino Libraries

- WebSockets by Markus Sattler
- Arduino_JSON by Arduino (BETA)
- Adafruit NeoPixel by Adafruit
- Preferences by Volodymyr Shymanskyy
- WiFiManager by tzapu

### Flashing

- Flash firmware with nodemcu-pyflasher
- Reboot the device
- Device will start an AP wifi, connect to it
- Captive portal lets you setup tallyarbiter server IP / port / device label
- Select wifi network and enter password
- Device will reboot and connect to network / tallyarbiter server

## Change wifi / TA information
- You'll have to reflash the device clearing all data
