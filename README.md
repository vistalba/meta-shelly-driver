# meta-shelly-driver

## General
This driver is to control some Shelly devices from your Neeo with help of meta2 (https://github.com/jac459/meta).
As this driver is new, it's beta stage. Please be aware that everything can change.

## Requirements
- Neeo
- propper and working installation of meta2 (https://github.com/jac459/meta)
- supported Shelly device
- shelly with fixed ip-address
- shelly device name set
- shelly username/password set (not tested without user/pass until now!)

## Supported devices
- Shelly 1 (Light)
- Shelly 1PM (Light)
- Shelly 1L (Light)
- Shelly Dimmer 1 (Light)
- Shelly Dimmer 2 (Light)
- Shelly 2.5 (Roller Shutter mode only!)

Please select the right driver above for your device.

## Shelly 1 / 1PM / 1L
Driver is supporting ON/OFF and TOGGLE command.
Important: After adding the device to Neeo you have to edit the recipe. Add "POWER ON" to the "Power on" and "POWER OFF" to the "Power Off" recipe. Otherwise pooling of the device will not work.

## Shelly Dimmer 1 / Dimmer 2
Driver is supporting ON/OFF/TOGGLE and Brightness with a slider.
Important: After adding the device to Neeo you have to edit the recipe. Add "POWER ON" to the "Power on" and "POWER OFF" to the "Power Off" recipe. Otherwise pooling of the device will not work.

## Shelly 2.5 (Roller Shutter mode)
Driver is supporting OPEN/CLOSE/STOP and setting a desired position by slider.
Futhermore you can tilt the cover blinds by push the cursor LEFT (close) or RIGHT (open) which will run the motor for 250ms.
Important: After adding the device to Neeo you have to make the recipe visible in recipe menu of Neeo. Otherwiese it will not shown on the room.

## Installation instructions

- Add Device on Neeo
- Search driver (Shelly)
- Select the propper driver for your Shelly device type!
- Enter URI for Shelly device (format example: username:password@192.168.178.55:80 | [username]:[password]@[ip-address]:[port])
  Important: If you are using special characters in your username/password you have to encode it as described in RFC1738 (https://datatracker.ietf.org/doc/html/rfc1738#section-3.1 | not tested) 
- Device name will be discovered. Select the propper device by your naming.
- Select a room which the device should be added.


