# XPlaneEnhancement

## About XPlaneEnhancement repository

This repository contains tuning scripts for my X-Plane 11-aircraft "Quest Kodiak". The scripts are written in Lua or FlyWithLua. 


## Files and folders

### Overview
* *writeKodiakPrefs.lua*: App to set some Kodiak preferences which are always overwritten with default values (workaround for Kodiak-issue)
* *Example Quest_Kodiak-LR_G1000_prefs.txt*: copy of the preferences file in the aircraft folder.
* *FlywithLua*: Alle FlyWithLua scripts lay here
  * *Kodiak_commands.lua*: A script that defines additional X-Plane 11-commands for the **Thranda Quest Kodiak** to be used by joysticks or keys
  * *IXEG733_commands.lua*: A script that defines additional X-Plane 11-commands for the **IXEG 737-300** to be used by joysticks or keys

### writeKodiakPrefs.lua, Example Quest_Kodiak-LR_G1000_prefs.txt

Workaround for the Thranda Quest Kodiak V2.3 which always overwrites it's prefs-file with
default data when unloading the aircraft in the X-Plane 11-simulator.  
Disclaimer: Use this app on your own risk.

!! Make sure to have a backup of your preferences file before using this app the first time. !!

This FlyWithLua-script overwrites the following preferences:
```
  _track_up_0,     _track_up_1,     _track_up_2
  _data_fields_0,  _data_fields_1,  _data_fields_2
  _ils_cdi_auto_0, _ils_cdi_auto_1, _ils_cdi_auto_2
  _filter_rnp_0,   _filter_rnp_1,   _filter_rnp_2
  _baro_unit_0,    _baro_unit_1,    _baro_unit_2
  _wind_display_0, _wind_display_1, _wind_display_2
  _inset_map_0,    _inset_map_1,    _inset_map_2
```
For development purposes I included an example preferences file out of my X-Plane Kodiak-aircraft folder "`Example Quest_Kodiak-LR_G1000_prefs.txt
Version: 1.0`".

### Kodiak_commands.lua

A script that provides additional X-Plane 11-commands to be used by joysticks or keys. Based on the script by Popeye_swe.

### IXEG733_commands.lua

A script that provides additional X-Plane 11-commands to be used by joysticks or keys.

-- * Set field of view so that all instruments are visible for the captain's side
* Create 4 commands to be used for hardware fuel cutoff levers:
  * Set lever 1 to on
  * Set lever 1 to off
  * Set lever 2 to on
  * Set lever 2 to off
* Create 2 commands to set all landing lights on/off
* Create 2 commands to set the taxi light and the runway turnoff lights on/off

The new commands can be found under *FlyWithLua/ixeg/...*

All created commands are logged in the x-plane log.txt file.
