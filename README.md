# 01-Connect Arduino IDE to Home Assistant by using WiFi and MQTT
This project demonstrates how to connect an ESP8266 board to Home Assistant using Wi-Fi and MQTT and update it over the Air. This setup allows you to monitor and control your devices in real-time, making your smart home more versatile and efficient.

See also : <a href="https://youtu.be/vI8LN8mpi_4" target="_blank"> My YouTube Tutorial</a> for the OTA (Over The Air Update) addon.


## Overview
The video guide walks you through the steps to:
- Set up the Arduino IDE to program the ESP8266.
- Write and upload code to connect the ESP8266 to your Wi-Fi network, MQTT broker and OTA (over the air) update.
- Configure Home Assistant to receive and display data from the ESP8266.

## Requirements
- An ESP8266 board (e.g., Wemos D1 Mini)
- USB cable for programming the ESP8266
- Home Assistant installed on your system
- MQTT broker set up within Home Assistant
- Arduino IDE installed on your computer

## Installation

### Arduino IDE Setup
1. **Download and Install Arduino IDE**: [Arduino IDE Download](https://www.arduino.cc/en/software)
2. **Add ESP8266 Board to Arduino IDE**:
   - Go to `File > Preferences`.
   - In the "Additional Board Manager URLs" field, add the following URL:
     ```
     http://arduino.esp8266.com/stable/package_esp8266com_index.json
     ```
   - Go to `Tools > Board > Boards Manager` and search for `ESP8266`. Install the package.

### Libraries Required
You will need the following libraries installed in the Arduino IDE:
- `ESP8266WiFi`
- `PubSubClient`
- `ESP8266mDNS.h`
- `WiFiUdp.h`
- `ArduinoOTA.h`

