
<p align="center">
<img src="https://www.home-assistant.io/images/home-assistant-logo.svg" width="150">
</p>

### Note: Configuration files have changed over time but I have kept the repo in its old state as a record.  Integrations these days means there is less reliance on config files, but i'll update some key ones that have required some work. Eg. Sensors

These are the [Home Assistant](https://home-assistant.io/) configuration files used in my Home Assistant (HA) setup. 
I'm new to the home automation game and have found hopefully this repository will help someone else who is getting started. 

HomeAssistant is currently running on a Raspberry PI 4 in Docker with a SQL backend, and telemetry storage via [InfluxDB](https://www.influxdata.com/time-series-platform/influxdb/), infrastructure data gathered by [Telegraf](https://www.influxdata.com/time-series-platform/telegraf), visualisation with [Grafana](https://grafana.com/), and various tasks that I prefer to run under linux. Eg. Docker, Crontab 

A fantastic resource for combing all of the above products is Phil Hawthorne's blog: https://philhawthorne.com/getting-started-with-grafana-influxdb-for-home-assistant/
He also has a great Docker image for InfluxDB & Grafana that greatly simplifies the setup process:  https://github.com/philhawthorne

# Editing the Configuration Files:
I edit the majority of the HA configuration files via Samba share on a Windows 10 workstation using [Visual Studio Code](https://code.visualstudio.com/).
Management of the Pi and Linux backend are done via [Putty](https://www.putty.org/).

# Connected Devices:

## Cloud Resources:
* __[Australian Bureau of Meteorology](http://www.bom.gov.au)__
* __[SpeedTest-cli](https://github.com/sivel/speedtest-cli)__
* __[Teslafi - Vehicle Stats & Tracking](https://www.teslafi.com)__

## Wifi Connected Devices
* __[LIFX Lights](https://www.lifx.com.au/)__ 
* __[Shelly 1 Plus - Garage Door Control](https://shelly.cloud/shelly-plus-1)__
* __[Sonos Music](https://www.sonos.com/en-au/home)__
* __[Konnected - Home Security](https://konnected.io)__
* __[Broadlink RM Mini 3](https://www.amazon.com/BroadLink-Control-Universal-Remote-RMMINI3-EN/dp/B01FK2SDOC/ref=sr_1_2?ie=UTF8&qid=1499475366&sr=8-2&keywords=broadlink+mini3)__
* __[Google Home - Voice Control](https://store.google.com/au/product/google_home_mini)__
* __[ChromeCast Audio](https://store.google.com/us/product/chromecast_audio)__
* __[TP-Link HS110 Power Switch](https://www.tp-link.com/au/products/details/cat-5258_HS110.html)__


## Zigbee Devices
* __[Slaesh CC2652RB Stick w/ Zigbee2Mqtt](https://slae.sh/projects/cc2652)__
* __[Xiaomi Smart Bluetooth Switch](https://www.gearbest.com/smart-light-bulb/pp_257679.html)__
* __[Xiaomi Temperature and Humidity Sensor](https://www.gearbest.com/access-control/pp_626702.html)__

## Hardwired Devices
* __[Cisco SG300-28p Switch](https://www.cisco.com/c/en/us/support/switches/sg300-28pp-28-port-gigabit-poe-plus-managed-switch/model.html)__
* __[Synology DS412+ ](https://www.synology.com/en-us/support/download/DS412+#utilities)__
* __[Mikrotik hEX Router ](https://mikrotik.com/product/RB750Gr3)__ 
* __[Mikrotik hAP ac lite Wireless AP](https://mikrotik.com/product/RB952Ui-5ac2nD)__
* __[Vivotek PD8136 Pan/Tilt Dome Cameras ](https://www.vivotek.com/website/pd8136/)__
* __[Enviro PHAT Sensors](https://shop.pimoroni.com/products/enviro-phat)__
* __[Pi-Hole](https://pi-hole.net/)__

   
## What's Next
