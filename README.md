# homeassistant-control4
These custom components for Home Assistant (https://www.home-assistant.io) allow you to integrate Control4 systems into Home Assistant. Currently, lights, thermostats, alarm systems, and media room volume control are supported. 

How to use:
-------------
- Install the Web2Way driver into your Control4 project using Composer Pro (2.9+ recommended): https://github.com/itsfrosty/control4-2way-web-driver (You may need your dealer to do this if you don't have access to the Control4 Composer Pro program)
- Copy the custom_components into your ~/.homeassistant/ folder
- Find the `proxy_id` of each Control4 device you want to integrate inside Composer Pro, and include them in your `configuration.yaml`

Sample Home Assistant `configuration.yaml` entries:
-------
~~~~
base_url: The IP address of your Control4 controller. (You should assign a static IP to your controller on your router)
proxy_id: The proxy ID of the Control4 device, found inside Composer Pro by hovering over the device in the project tree view.
name: The name that Home Assistant will use to identify the device.
scan_interval: How often to query the Control4 controller about the state of the device, in seconds.
~~~~

Lights:
~~~~


