# HubConnect Custom Drivers
A collection of custom drivers to use with HubConnect

## Using these Custom Drivers with HubConnect

#### Install and Configure Custom Driver on your HubConnect Server (master)
1. Install and save the desired Custom Driver in the **Drivers** section of your HubConnect Server.
2. On the HubConnect Server:
   * Open the **HubConnect Server for Hubitat** application
   * Click on **Manage Custom Drivers**
   * Click on **Add A Driver**
   * Fill in the **Attribute Class Name** and **Device Driver Name** as shown below for the driver you installed in step 1.
   * Select the **Attribute 1/18** type from the options list, as shown below
   * Fill in the remainder of the Attributes as shown below
3. Click **Save**
4. Click **Done**
5. Click **Home** (or **Next**)

#### Install Custom Driver on any HubConnect Remote Clients
This is only necessary if you want to reflect a Custom Device as a device on your Remote Client. If the device is physically installed on your Remote Client, you do not need to install the Custom Device (but it doesn't hurt anything if you do).
1. Install and save the desired Custom Driver in the **Drivers** section of the HubConnect Remote Client that you want to use the (reflected) device on. *Note that some drivers will not work on SmartThings Hubs*

#### Reflect a Custom Device from your HubConnect Server
1. Open the appropriate **HubConnect Server Instance** application for the target Remote Client
2. Click on **Connect local devices to Remote Hub**
3. Click on **Custom Devices**
4. Click on the desired Custom Driver definition
5. Select the desired local devices that you want to reflect using this driver. ***Be sure that the Custom Driver is already installed on the Remote Client!***
6. When finished, click Done/Next all the way back to the main menu

#### Reflect a Custom Device from a HubConnect Remote Client
1. Open **HubConnect Remote Client** application on the Remote Hub
2. Click on **Select devices to synchronize to Server hub**
3. Click on **Custom Devices**. Here you should see the list of Custom Drivers that you Installed & Configured in the very first step above. 
4. Click on the desired Custom Driver definition
5. Select the desired local devices that you want to reflect using this driver. ***Be sure that the Custom Driver is already installed on the Remote Client!***
6. When finished, click Done/Next all the way back to the main menu

### HubConnect EchoSpeaks
**importUrl:** https://raw.githubusercontent.com/SANdood/HubConnect-Custom-Drivers/master/HubConnect%20EchoSpeaks

#### Works With [Echo Speaks by Anthony Santilli (@tonesto7)](https://github.com/tonesto7/echo-speaks)
* Hubitat webSockets-only, as HubConnect limits the number of attributes that can be reflected via http. Cannt be used with SmartThings-hosted Echo Speaks, nor to reflect Hubitat-hosted Echo Speaks to a SmartThings hub.
#### HubConnect Configuration
* **Attribute Class Name:** `EchoSpeaks`
* **Device Driver Name:** `HubConnect Echo Speaks Device`
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

### HubConnect Ecobee Suite Sensor
**importUrl:**
* Designed for reflecting SmartThings-based Ecobee Suite Sensors to Hubitat, or Hubitat to Hubitat. Will not save as a SmartThings DTH

#### HubConnect Configuration
* **Attribute Class Name:** `ESSensor`
* **Device Driver Name:** `HubConnect Ecobee Suite Sensor`
* **Attribute 1/18: ** `temperatureMeasurement`
* **Attribute 2/18: ** `motion`
* **Attribute 3/18: ** `Awake`    // Sensor used in Awake Program? off = no, on = yes
* **Attribute 4/18: ** `Away`     // Sensor used in Away Program?
* **Attribute 5/18: ** `Home`     // Sensor used in Home Program?
* **Attribute 6/18: ** `Sleep`    // Sensor used in Sleep Program?
* **Attribute 7/18: ** `Fan Only`
* **Attribute 8/18: ** `programsList`
* **Attribute 9/18: ** `SmartRoom`
* **Attribute 10/18: ** `Wakeup`  // Sensor used in Wakeup Program?
* **Attribute 11/18: ** `currentProgramName`
* **Attribute 12/18: ** `doors`
* **Attribute 13/18: ** `humidity`
* **Attribute 14/18: ** `thermostatId`
* **Attribute 15/18: ** `windows`
* **Attribute 16/18: ** `vents`

### HubConnect Ecobee Suite Thermostat
**importUrl:**
* Designed for reflecting SmartThings-based Ecobee Suite Thermostats to Hubitat, or Hubitat to Hubitat. Will not save as a SmartThings DTH.
* ***IMPORTANT NOTE: Ecobee Suite Helpers are NOT supported by this reflected device!***

#### HubConnect Configuration
* **Attribute Class Name:** `ESThermostat`
* **Device Driver Name:** `HubConnect Ecobee Suite Thermostat`
* **Attribute 1/18: ** ``
* **Attribute 2/18: ** ``
* **Attribute 3/18: ** ``
* **Attribute 4/18: ** ``
* **Attribute 5/18: ** ``
* **Attribute 6/18: ** ``
* **Attribute 7/18: ** ``
* **Attribute 8/18: ** ``
* **Attribute 9/18: ** ``
* **Attribute 10/18: ** ``
* **Attribute 11/18: ** ``
* **Attribute 12/18: ** ``
* **Attribute 13/18: ** ``
* **Attribute 14/18: ** ``
* **Attribute 15/18: ** ``
* **Attribute 16/18: ** ``
* **Attribute 17/18: ** ``
* **Attribute 18/18: ** ``

### HubConnect EcoVent
**importUrl:** https://raw.githubusercontent.com/SANdood/HubConnect-Custom-Drivers/master/HubConnect%20EcoVent

#### Works With [Econet EV100 Vent for Hubitat (my custom version)](https://github.com/SANdood/Hubitat-Stuff/blob/master/Econet-EV100-Vent.groovy)
* Tested for use reflecting Hubitat-based EcoVents to SmartThings Remote Hub
#### HubConnect Configuration
* **Attribute Class Name:** `EcoVent`
* **Device Driver Name:** `HubConnect EcoVent`
* **Attribute 1/18:** `switchLevel`
* **Attribute 2/18:** `switch`
* **Attribute 3/18:** `battery`
* **Attribute 4/18:** `contact`

### HubConnect Illuminance Sensor
**importUrl:** https://raw.githubusercontent.com/SANdood/HubConnect-Custom-Drivers/master/HubConnect%20Illuminance%20Sensor

#### Works With all Illuminance Sensors
* Useful to reflect `illuminance` only from multi-sensor devices
#### HubConnect Configuration
* **Attribute Class Name:** `Lux`
* **Device Driver Name:** `HubConnect Illuminance Sensor`
* **Attribute 1/18:** `illuminanceMeasurement`

### HubConnect MyQ Garage Door Opener
**importUrl:** https://raw.githubusercontent.com/SANdood/HubConnect-Custom-Drivers/master/HubConnect%20MyQ%20Garage%20Door%20Opener

#### Works With Brian Beaird's MyQ Lite Garage Door Opener
#### HubConnect Configuration
* **Attribute Class Name:** `MyQGarageDoor`
* **Device Driver Name:** `HubConnect MyQ Garage Door Opener`
* **Attribute 1/18:** `garageDoorControl`
* **Attribute 2/18:** `contact`
* **Attribute 3/18:** `acceleration`
* **Attribute 4/18:** `doorSensor`
* **Attribute 5/18:** `lastActivity`
* **Attribute 6/18:** `switch`
* **Attribute 7/18:** `myQDeviceId`
* **Attribute 8/18:** `CloseButton`
* **Attribute 9/18:** `OpenButton`

### HubConnect Relative Humidity Sensor
**importUrl:** https://raw.githubusercontent.com/SANdood/HubConnect-Custom-Drivers/master/HubConnect%20Relative%20Humidity%20Sensor

#### Works With all Relative Humidity Sensors
* Useful to reflect 'humidity' only from multi-sensor devices
* Probably works with moisture sensors as well
#### HubConnect Configuration
* **Attribute Class Name:** `Humidistat`
* **Device Driver Name:** `HubConnect Relative Humidity Sensor`
* **Attribute 1/18:** `relativeHumidityMeasurement`

### HubConnect Temperature Sensor
**importUrl:** https://raw.githubusercontent.com/SANdood/HubConnect-Custom-Drivers/master/HubConnect%20Temperature%20Sensor

#### Works With all Temperature Sensors
* Useful to reflect `temperature` only from multi-sensor devices
#### HubConnect Configuration
* **Attribute Class Name:** `Thermometer`
* **Device Driver Name:** `HubConnect Temperature Sensor`
* **Attribute 1/18:** `temperatureMeasurement`
