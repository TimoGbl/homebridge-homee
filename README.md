# Homebridge-Homee

[![Package Quality](http://npm.packagequality.com/shield/homebridge-homee.svg)](http://packagequality.com/#?package=homebridge-homee)

Homee platform plugin for homebridge: https://github.com/nfarina/homebridge

## Installation
Follow the instruction in [NPM](https://www.npmjs.com/package/homebridge) for the homebridge server installation. The plugin is published through [NPM](https://www.npmjs.com/package/homebridge-homee) and should be installed "globally" by typing:

    sudo npm install -g homebridge-homee

## Configuration

config.json

Example:

    {
        "bridge": {
            "name": "Homebridge",
            "username": "CC:22:3D:E3:CE:51",
            "port": 51826,
            "pin": "031-45-154"
        },
        "description": "This is an example configuration file for the homebridge-homee plugin",
        "hint": "Always paste into jsonlint.com validation page before starting your homebridge, saves a lot of frustration",
        "platforms": [
            {
                "platform": "Homee",
                "name": "Homee",
                "host": "192.168.178.1",
                "user": "your-username",
                "pass": "your-password",
                "debug": true //optional, enable debug mode
            }
        ]
    }

## Exclude nodes
This plugin integrates all (known) devices to homebridge by default. You can create a group named 'Homebridge' in Homee and add all the devices you want to use with homebridge. Other devices are then ignored.

## Tested devices
- Danfoss Living connect Thermostat
- Devolo Door/Window Sensor
- Devolo Motion Sensor
- Devolo Heizkörperthermostate
- Devolo Smart Metering Plug
- Fibaro Door/Window Sensor
- Fibaro Motion Sensor
- Fibaro Smoke Sensor 2
- Fibaro Wall Plug
- Greenwave Powernode
- Philips Hue White and Color Ambiance
- Philips Hue White
- Popp Rauchwarnmelder mit Sirene
