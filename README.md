# HubConnect Custom Drivers
A collection of custom drivers to use with HubConnect

## Using these Custom Drivers with HubConnect
1. Install and save the desired Custom Driver in the **Drivers** section of your HubConnect Server, and on any HubConnect Remote Client that you want to use the (reflected) device on. *Note that some drivers will not work on SmartThings Hubs*
2. On the HubConnect Server:
  * Open the `HubConnect Server for Hubitat` application
  * Click on `Manage Custom Drivers`
  * Click on `Add A Driver`
  * Fill in the `Attribute Class Name` and `Device Driver Name` as shown below for the driver you installed in step 1.
  * Select the `Attribute 1/18` type from the options list, as shown below
  * Fill in the remainder of the Attributes as shown below
3. 
### HubConnect EchoSpeaks
#### Works With [Echo Speaks by tonesto7](https://github.com/tonesto7/echo-speaks)
* Hubitat webSockets-only, as HubConnect limits the number of attributes that can be reflected via http
#### HubConnect Configuration
* **Attribute Class Name:** `EchoSpeaks`
* **Device Driver Name:** `HubConnect EchoSpeaks`
* **Attribute 1/18:** `speechSynthesis`
* **Attribute 2/18:** `mute`
* **Attribute 3/18:** `level`
* **Attribute 4/18:** `volume`
* **Attribute 5/18:** `alarmVolume`
* **Attribute 6/18:** `doNotDisturb`
* **Attribute 7/18:** `alexaWakeWord`
* **Attribute 8/18:** `currentAlbum`
* **Attribute 9/18:** `currentStation`
* **Attribute 10/18:** `wasLastSpokenToDevice`
* **Attribute 11/18:** `status`
* **Attribute 12/18:** `deviceStatus`
* **Attribute 13/18:** `onlineStatus`
* **Attribute 14/18:** `followUpMode`
* **Attribute 15/18:** `nediaSource`
* **Attribute 16/18:** `lastUpdated`
* **Attribute 17/18:** `alexaPlaylists`
* **Attribute 18/18:** `alexaGuardStatus`

### HubConnect EcoVent
#### Works With [Econet EV100 Vent for Hubitat (my custom version)](https://github.com/SANdood/Hubitat-Stuff/blob/master/Econet-EV100-Vent.groovy)
* Tested for use reflecting Hubitat-based EcoVents to SmartThings Remote Hub
#### HubConnect Configuration
* **Attribute Class Name:** `EcoVent`
* **Device Driver Name:** `HubConnect EcoVent`
* **Attribute 1/18:** `switchLevel`
* **Attribute 2/18:** `switch`
* **Attribute 3/18:** `battery`
* **Attribute 4/18:** `contactSensor`

### HubConnect Illuminance Sensor
#### Works With all Illuminance Sensors
* Useful to reflect `illuminance` only from multi-sensor devices
#### HubConnect Configuration
* **Attribute Class Name:** `Lux`
* **Device Driver Name:** `HubConnect Illuminance Sensor`
* **Attribute 1/18:** `illuminanceMeasurement`

### HubConnect MyQ Garage Door Opener
#### Works With Brian Beaird's MyQ Lite Garage Door Opener
#### HubConnect Configuration
* **Attribute Class Name:** `MyQGarageDoor`
* **Device Driver Name:** `HubConnect MyQ Garage Door Opener`
* **Attribute 1/18:** `garageDoorControl`
* **Attribute 2/18:** `contactSensor`
* **Attribute 3/18:** `acceleration`
* **Attribute 4/18:** `doorSensor`
* **Attribute 5/18:** `lastActivity`
* **Attribute 6/18:** `switch`
* **Attribute 7/18:** `myQDeviceId`

### HubConnect Relative Humidity Sensor
#### Works With all Relative Humidity Sensors
* Useful to reflect 'humidity' only from multi-sensor devices
* Probably works with moisture sensors as well
#### HubConnect Configuration
* **Attribute Class Name:** `Humidistat`
* **Device Driver Name:** `HubConnect Relative Humidity Sensor`
* **Attribute 1/18:** `relativeHumidityMeasurement`

### HubConnect Temperature Sensor
#### Works With all Temperature Sensors
* Useful to reflect `temperature` only from multi-sensor devices
#### HubConnect Configuration
* **Attribute Class Name:** `Thermometer`
* **Device Driver Name:** `HubConnect Temperature Sensor`
* **Attribute 1/18:** `temperatureMeasurement`
