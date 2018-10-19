
<p align="center">
  <img src="https://github.com/home-assistant/home-assistant-assets/blob/master/loading-screen.gif">
</p>

These are the [Home Assistant](https://home-assistant.io/) configuration files used in my Home Assistant (HA) setup. 
I'm new to the home automation game and have found Hopefully this repository will help someone else who is getting started. 

HomeAssistant is currently running on a Raspberry PI 3 Model B+.  I am running [Hassbian](https://www.home-assistant.io/docs/installation/hassbian/installation/) because I am comfortable with the Debian architecture it runs on and like the freedom it provides. I also have a seprate headless Debian Stretch server that handles data storage via [InfluxDB](https://www.influxdata.com/time-series-platform/influxdb/), infrastructure data gathered by [Telegraf](https://www.influxdata.com/time-series-platform/telegraf), visualisation with [Grafana](https://grafana.com/), and various tasks that I prefer to run under linux. Eg. Docker, Crontab    

A fantastic resource for combing all of the above products is Phil Hawthorne's blog: https://philhawthorne.com/getting-started-with-grafana-influxdb-for-home-assistant/
He also has a great Docker image for InfluxDB & Grafana that greatly simplifies the setup process:  https://github.com/philhawthorne

# Editing the Configuration Files:
I edit the majority of the HA configuration files via Samba share on a Windows 10 workstation using [Visual Studio Code](https://code.visualstudio.com/).
Management of the Pi and Linux backend are done via [Putty](https://www.putty.org/).

# Connected Devices:

## Cloud Resources:
* __[Australian Bureau of Meteorology](http://www.bom.gov.au)__
* __[IFTTT](https://ifttt.com)__
* __[Life360](https://www.life360.com/)__
* __[DuckDNS](https://www.duckdns.org/)__
* __[SpeedTest-cli](https://github.com/sivel/speedtest-cli)__

## Wifi Connected Devices
* __[LIFX Lights](https://www.lifx.com.au/)__ 
* __[Broadlink RM Mini 3](https://www.amazon.com/BroadLink-Control-Universal-Remote-RMMINI3-EN/dp/B01FK2SDOC/ref=sr_1_2?ie=UTF8&qid=1499475366&sr=8-2&keywords=broadlink+mini3)__*
* __[Google Home Mini](https://store.google.com/au/product/google_home_mini)__
* __[ChromeCast Audio (x2)](https://store.google.com/us/product/chromecast_audio)__
* __[Xiaomi Mi Box (x2)](https://www.mi.com/en/mibox/)__
* __[TP-Link HS110 Power Switch (x2)](https://www.tp-link.com/au/products/details/cat-5258_HS110.html)__

## Zwave / Zigbee Devices (Not Integrated Yet)
* __[Vera3 Controller](http://getvera.com/controllers/vera3/)__
* __[Aeotec Door Sensor](https://aeotec.com/z-wave-door-window-sensor)__
* __[Xiaomi Multifunction Gateway](https://www.gearbest.com/living-appliances/pp_344667.html)__
* __[Xiaomi Smart Bluetooth Switch](https://www.gearbest.com/smart-light-bulb/pp_257679.html)__
* __[Xiaomi Temperature and Humidity Sensor](https://www.gearbest.com/access-control/pp_626702.html)__

## Hardwired Devices
* __[Cisco SG300-28p Switch](https://www.cisco.com/c/en/us/support/switches/sg300-28pp-28-port-gigabit-poe-plus-managed-switch/model.html)__
* __[Synology DS412+ ](https://www.synology.com/en-us/support/download/DS412+#utilities)__
* __[Mikrotik hEX Router ](https://mikrotik.com/product/RB750Gr3)__ 
* __[Mikrotik hAP ac lite Wireless AP](https://mikrotik.com/product/RB952Ui-5ac2nD)__
* __[Vivotek PD8136 Pan/Tilt Dome Camera ](https://www.vivotek.com/website/pd8136/)__
* __[Enviro PHAT Sensors](https://shop.pimoroni.com/products/enviro-phat)__
* __[Pi-Hole](https://pi-hole.net/)__

   
## What's Next

### Z-Wave & Zigee Gear:  
* I am waiting on my Xiaomi gear to arrive and once it has i'll integrate it into HA with a bunch of old Z-Wave bits and pieces I have too. Contemplating whether to keep the Vera3, or purchase a USB Z-Wave dongle for the Pi to simplify the setup a bit... One less hub is always better in my books.
### Stats & Figures:  
* I've been capturing a bunch of data with Telgraf and want to expand on that a bit.  I also have a scheduled SpeedTest capturing data into InfluxDB. I want to start adding these in as sensors and displaying them.
~~### Interface:~~
~~* I want to set up a lovelace interface, but i'll probably wait until I have the rest of my sensors inplace.~~
### Automation:  
* Not doing alot of automation just yet, but will explore it more soon now that i've got some good data coming in and more control over devices.