AWARE Plugin: YOUR PLUGIN
==========================

This plugin measures tone of keyboard data for every hour.

# Settings
Parameters adjustable on the dashboard and client:
- **status_plugin_template**: (boolean) activate/deactivate plugin

# Broadcasts
**ACTION_AWARE_PLUGIN_TEMPLATE**
Broadcast ..., with the following extras:
- **value_1**: (double) amount of time turned off (milliseconds)

# Providers
##  Template Data
> content://com.aware.plugin.tone_analyser.provider.tone_analyser

Field | Type | Description
----- | ---- | -----------
_id | INTEGER | primary key auto-incremented
timestamp | REAL | unix timestamp in milliseconds of sample
device_id | TEXT | AWARE device ID
tone      | TEXT | Tone analysed for previous hour
