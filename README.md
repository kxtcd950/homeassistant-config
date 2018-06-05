# HomeAssistant configuration baseline

First stab at a homeassistant configuration.
Note that this uses MQTT components quite heavily as I've bridged Samsung's smartthings with MQTT, all the samsung "things" therefore appear as MQTT devices/sensors.
Also, so do the hue tap devices I've got; there's a python poller on my network for Hue tap which makes them appear as MQTT devices.

A lot of the automations are for turning lights on and off in time with the sun's elevation.

Added an input boolean to toggle the tortoise lights switching on at sunrise instead of a fixed 6:00am, this is to give the tortoises more seasonal variation, but allow for summer (where sunrise is obscenely early) to give them a little more down-time.

Added a scene and new automation for Fridays (when instead of going to bed, I sit downstairs and play PS4 games) so that I'm not bathed in darkness at 22:20.  There's a switchoff for gaming nights which acts as an alarm clock for me to finally go to bed (without this, sometimes I forget).

Repurposed the Hallway hue tap ("Hallway tap") as it wasn't being used.  It's now used to control the tortoise environmental lighting instead of the automation system being overridden manually because it's too hard to use the homeassistant app to turn the tortoise lights on and off on an ad-hoc basis.  This setup, I am assured, will allow the lights' states in the frontend to reflect reality as the physical switches won't be used anymore.
