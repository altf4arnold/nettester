# nettester

This is a simple python script that has for only purpose to test the UrLab network when it crashes.
It was designed to run on a raspberry pi 3 B+.

## dependencies :
* RPi.GPIO
* python 3
* nslookup

## How to run :
Assuming that you have the permissions to access the raspberry pi's GPIO with your user :
```
virtualenv -p python3 ve3
source ve3/bin/activate
pip install -r requirements.txt
python nettester.py
```

## GPIO pins layout :
![alt text](gpio-numbers-pi2.png "Raspi GPIO")

* pin 2 : input
* pin 3 : reset
* pin 4 : DNS
* pin 14 : LAN
* pin 15 : DHCP
* pin 18 : not our fault
* pin 17 : wifi
