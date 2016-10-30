# homebridge-mqtt-smoke-alarm
An homebridge plugin that creates an HomeKit smoke alarm accessory mapped on a MQTT topic.

# Installation
Follow the instruction in [homebridge](https://www.npmjs.com/package/homebridge) for the homebridge server installation.
The plugin is published through [NPM](https://www.npmjs.com/package/homebridge-mqtt-power-consumption) and should be installed "globally" by typing:

    npm install -g homebridge-mqtt-smoke-alarm

# Configuration
Remember to configure the plugin in config.json in your home directory inside the .homebridge directory. Configuration parameters:
```javascript
{
  "accessory": "mqtt-smoke-alarm",
  "name": "<name>",
  "url": "<url of the broker>", // i.e. "http://mosquitto.org:1883"
  "username": "<username>",
  "password": "<password>",
  "topic": "<topic to get the alarm state>"
}
```
