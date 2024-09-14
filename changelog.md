# Changelog

### [v1.1.0]

#### New Features:
- OTA Firmware update
- Get FirmwareVersion

#### Improvements:
- 

#### Bug Fixes:
- NA

#### Known Issues:
- Handling missed ON schedules while the device was offline
- If ON & OFF schedule are given for the same time device will turn ON & OFF repeatedly.
- Device doesn't try reconnect to Wifi if failed in first attempt, stays in AP Mode

---

### [v1.0.0]

#### New Features:
- Added support for **new PCB version 1.0** with fan speed control circuitry.
- Scheduling functionality 
- Web Server for Wifi Config
- Added schedule_disabled
- Added getFanSpeed, getFilterTime, getLedTime
- Added resetFilterTime & resetLedTime
- Added Publish AQI index after time interval

#### Improvements:
- Restructured payload message to JSON format
- Migrated from CloudMQTT to
- List of update payloads Refer: [VioletC MQTT Payload Structure]([URL_TO_PAYLOAD_STRUCTURE])
- Improved get_schedule format
- Fixed schedules getting reset after device restart
- Maintaining the last known fan & UVS state after a restart
- Fixed, disable_schedule doesn't reset the schedule [I]
- Fixed, getFanSpeed command not fetching speed level from NVM

#### Bug Fixes:
- NA

#### Known Issues:
- NA

---

### [v0.1.0]

#### New Features:
- Basic hardware test
- MQTT integration 

#### Improvements:
- NA

#### Bug Fixes:
- NA

#### Known Issues:
- Fan speed control not working



[VioletC MQTT Payload Structure]: [https://github.com/olivierlacan/keep-a-changelog/compare/v1.1.0...v1.1.1](https://docs.google.com/document/d/1pG3jhv8G_tFZMPh7XMVLRTqPksyWVIKNnsxpRhT-Wag/edit?usp=sharing)
