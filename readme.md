# The idea
Before I even received my Decent Espresso Machine I was searching for possibilities to integrate the machine with Home Automation systems.

On the diaspora I stubled upon the Web API created by Johanna Schander (https://github.com/decentespresso/de1app/tree/main/de1plus/plugins/web_api) and also the more detailed API by Henrik Pejer (https://github.com/pejer/decentespresso_module_system/tree/modules/modules/pejer_web_api). The second one was integrated directly to the app. So it will break with every update. Since there is a good working plugin system I thought this should be used.

I talked to both and with their "blessing" I combined both ideas and added mine to it.

# What does it do?
* get a simple or detailed state of the machine
* change the state to standby or enable it
* get, display or download shot files
* get, download or upload profiles


# How to use it?
* Copy the files to the plugin folder into a folder called "advanced_rest_api".
* Adjust the plugin settings in the settings file if needed.
* Activate the plugin in the app settings.

## API
There is a documentation about all available API endpoints in the attached json - which is also displayed in the Web UI.

## Web UI
Navigate to http://DECENT-IP:8888 in your preferred browser. The port can be changed in the settings. 8080 should be prevented if it is used with the webcast feature.

## Home Assistant
There is a yaml file available with an example configuration for Home Assistant (https://home-assistant.io).

## Homebridge
As requested I added a Homebridge accessory config.
* install the Homebridge Http Switch Plugin (https://github.com/Supereg/homebridge-http-switch)
* create a new device and add the example configuration


... please contact me for feature requests. 

# Disclaimer
Of course the usage of this is at your own risk. It may break your machine. You are creating a web server with an unencypted connection in your network. Please be cautious.

This is my first work in TCL - please be nice ;-)
