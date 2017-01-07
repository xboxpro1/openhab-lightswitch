# OpenHAB light switch

This repository encapsulates Cadsoft's Eagle files and firmware for OpenHAB light switch using ESP8266-01 module. For powering module can be used any 5V/ >=800mA power supply such as USB charger for phone.

Schematic is very simple. GPIO0 of ESP8266 is used for driving relay and GPIO2 for observation of original switch. Light can be turned on / off using original switch or OpenHAB admin screen.

For uploading code to ESP8266 is needed Arduino. In source code is needed to specify WIFI AP parameters, network parameters, OpenHAB item name as well as address where OpenHAB server listens. After module started is in his IP address available HTTP server where some parameters can be redefined. It's useful in case for example changing WIFI password.


###Schematic:
![alt](/eagle/lightswitchx1_sch.png?raw=true)



###PCB:
PCB is realized as single-sided with some wire jumpers. ESP8266 is mounted as always in socket to enable firmware update.

![alt](/eagle/lightswitchx1_brd.png?raw=true)

##Some project images:

### Module with power supply
![alt](/images/2017-01-02%2021.51.43.jpg?raw=true)

### Already mounted on its place
![alt](/images/2017-01-07%2013.30.43.jpg?raw=true)
![alt](/images/2017-01-07%2014.20.36.jpg?raw=true)
