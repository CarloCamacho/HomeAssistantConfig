
<p align="center">
<img src="https://www.home-assistant.io/images/home-assistant-logo.svg" width="150">
</p>

### Note: Configuration files have changed over time but I have kept the repo in its old state as a record.  Integrations these days means there is less reliance on config files, but i'll update some key ones that have required some work. Eg. Sensors

These are the [Home Assistant](https://home-assistant.io/) configuration files used in my Home Assistant (HA) setup. 
I'm new to the home automation game and have found hopefully this repository will help someone else who is getting started. 

HomeAssistant is currently running on a Raspberry PI 4 in Docker, with a local instance of Zigbee2Mqtt handling the Zigbee devices. 

# Editing the Configuration Files:
I edit the majority of the HA configuration files via Samba share on a Windows 10 workstation using [Visual Studio Code](https://code.visualstudio.com/).
Management of the Pi and Linux backend are done via [Putty](https://www.putty.org/).

# Connected Devices:

## Cloud Resources:
* __[Australian Bureau of Meteorology](http://www.bom.gov.au)__
* __[Teslafi - Vehicle Stats & Tracking](https://www.teslafi.com)__
* __[PV Output - Solar performance tracking](https://pvoutput.org/)__


## Wifi Connected Devices
* __[LIFX Lights](https://www.lifx.com.au/)__ 
* __[Shelly 1 Plus - Garage Door Control](https://shelly.cloud/shelly-plus-1)__
* __[Sonos Music](https://www.sonos.com/en-au/home)__
* __[Konnected - Home Security](https://konnected.io)__
* __[Tuya Lightbulbs - Lamps](https://www.tuya.com)__
* __[Google Home - Voice Control](https://store.google.com/au/product/google_home_mini)__
* __[ChromeCast Audio](https://store.google.com/us/product/chromecast_audio)__
* __[TP-Link HS110 Power Switch](https://www.tp-link.com/au/products/details/cat-5258_HS110.html)__
* __[Xiaomi Smart WiFi Socket](https://xiaomipedia.com/en/p/mijia-smart-wifi-socket-2/)__

## Zigbee Devices
* __[Slaesh CC2652RB Stick w/ Zigbee2Mqtt](https://slae.sh/projects/cc2652)__
* __[Xiaomi Smart Bluetooth Switch](https://www.gearbest.com/smart-light-bulb/pp_257679.html)__
* __[Xiaomi Temperature and Humidity Sensor](https://www.gearbest.com/access-control/pp_626702.html)__
* __[Philips Hue Dimmer Switch](https://www.philips-hue.com/en-us/p/hue-dimmer-switch--latest-model-/046677562779)__

## Hardwired Devices and Services
* __[Cisco SG300-28p Switch](https://www.cisco.com/c/en/us/support/switches/sg300-28pp-28-port-gigabit-poe-plus-managed-switch/model.html)__
* __[Synology DS412+ ](https://www.synology.com/en-us/support/download/DS412+#utilities)__
* __[pfSense Router w/ pfBLockerNG](https://www.pfsense.org/)__
* __[Vivotek PD8136 Pan/Tilt Dome Cameras ](https://www.vivotek.com/website/pd8136/)__
* __[TP-Link Tapo C100 Camera ](https://www.tapo.com/au/product/smart-camera/tapo-c100/)__
* __[TP-Link Tapo C200 Pan/Tilt Dome ](https://www.tapo.com/au/product/smart-camera/tapo-c200/)__
* __[Fronius Symo 8.2-3-M](https://www.solargain.com.au/solar-inverters/fronius/fronius-symo)__
* __[Frigate NVR](https://frigate.video/)__
* __[AdvantageAir - Air Conditioning Control](https://www.advantageair.com.au/myplace)__
* __[Hydrwise Reticulation](https://www.hydrawise.com/)__




## What's New
- New Lovelace interface -  
I'm in a fairly good place with the interface right now. It works well both on in a browser and on phones, and so far the wife has been fine interacting with it.
I've recently integrated the Frigate NVR video feeds and have found it to work really well. 
I've also just added a bit of logic around the kettle to highlight whether its ready to be turned on or not - essentially before going to be I make sure its filled and then turn it off at the wall/smartplug. 
This is detected by home assistant and flags that the kettle is ready. In a groggy state in the morning, we can see if the kettle is ready and turn it on from our phones.
Of course we could also set a timer and have it ready, but i've its better to do it on demand as its a fairly basic kettle with no "keep warm" type functions, so if it boils and we don't use it, we'll have to run it again manually anyways. 

<img src="https://github.com/CarloCamacho/HomeAssistantConfig/blob/master/Stock%20Photos/lovelace.JPG">
