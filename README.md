# HomeAssistant configuration baseline

First stab at a homeassistant configuration.
Note that this uses MQTT components quite heavily as I've bridged Samsung's smartthings with MQTT, all the samsung "things" therefore appear as MQTT devices/sensors.
Also, so do the hue tap devices I've got; there's a python poller on my network for Hue tap which makes them appear as MQTT devices.

A lot of the automations are for turning lights on and off in time with the sun's elevation.

