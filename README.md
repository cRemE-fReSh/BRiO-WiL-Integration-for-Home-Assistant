# BRiO WiL Integration for Home Assistant

## Notice

This is not an official integration of the manufacturer of the device. Also, I am neither in touch nor in contact with the manufacturer.

Please review the license before usage.

## Info

This solution integrates the CCEI BRiO WiL into Home Assistant using TCP commands via Node-RED. BRiO WiL is used to control pool underwater spotlights via WiFi and Bluetooth using the App of the manufacturer.

Trying this out, you should already be firm in using Node-RED.

Please understand that some wording within the integration is in German language, especially all texts that are visible in the Home Assistant dashboards. Any translator helps ;-)

## Integration

The integration consists of two elements: Node-RED flow and a few inputs, that have to be added to the configuration.yaml.

### Prerequisite

The BRiO WiL device must be connected to the same network (LAN/WiFi) as Node-RED and therefore reachable from the Node-RED host.

### Node-RED

You can import the flow from folder Node-RED in this repository.

Please ensure that you change the IP adress within **ALL** TCP requests within the flow to the IP adress of your own device.

### Home Assistant

You have to create four new inputs of type input_select and one of input_boolean.

All required code can be retrieved from the file within folder "Home Assistant".

After restarting HA, you can add the inputs to your dashboards.

![alt text](https://github.com/cRemE-fReSh/BRiO-WiL-Integration-for-Home-Assistant/blob/main/Screenshot_HASS.png)?raw=true)

Have fun!
