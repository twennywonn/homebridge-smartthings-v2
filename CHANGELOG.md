
## v2.1.0
- [UPDATE] Refactored the device service and characteristic logic so it's cleaner, more modular, and easier to maintain.
- [NEW] Device services and characteristics are now cleaned up when they are no longer used.
- [FIX] Lot's of fixes for device state updates and device commands.
- [FIX] Button events should now work again.
- [FIX] Updated the Hoobs config file (Plugin will be undergoing review by Hoobs to be certified soon) (@mkellsy)
- [FIX] Added support for AirPurifier & AirQuality (@danielskowronski)
- [FIX] Delays on device event updates resolved. (@devarshi) #33 #40
- [FIX] Thermostat Mode fixes (@torandreroland)
- [FIX] Dozens of other minor bugfixes and tweaks.

## v2.0.5 - v2.0.10
- [FIX] Fixed thermostat temp unit error.
- [FIX] removed token/id validation by default to prevent error with mismatched access_token | app_id.
- [FIX] Other minor bugfixes and tweaks.

## v2.0.4
- [FIX] Fixed AlarmStatus updates not being shown in the Home app when changed from ST side.
- [FIX] Fixed issues with local_commands option.
- [FIX] Fix for Celcius temperature conversions.
- [NEW] Added support for new 'temperature_unit' config option using either the smartapp or config.json file.
- [FIX] Other minor bugfixes and tweaks.

## v2.0.1
- [NEW] Completely rewrote the entire plugin using modern javascript structure.
- [NEW] The code is now much cleaner,  easier to update/maintain, and easier for others to follow.
- [NEW] This translates into a  faster/leaner and way more stable plugin than previous versions.
- [NEW] The plugin now uses the Homebridge Dynamic platform API, meaning it no longer requires a restart of the Homebridge service for device changes to occur.
- [NEW] The plugin now utilizes the device cache on service restart to prevent losing all of your devices when the plugin fails to start for an extended period of time.
- [NEW] It will now remove devices no longer selected under SmartThings.
- [NEW] Introduced an all-new logging system to provide more insight into issues and status, as well as write them to a file.
- [NEW] I used all of the issues from my existing plugin to repair this new version.
- [NEW] Many, many other bug fixes for devices, commands and many other items.
- [NEW] ***Important NOTICE:***
**Due to the changes in the plugin API you can not directly update the plugin, you will need to add as a new accessory and setup your devices/automations/scenes again.
On a positive note, you can use the same SmartApp instance though as long as you update to the latest code.**
