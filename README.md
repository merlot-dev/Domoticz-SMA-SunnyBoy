# Domoticz-SMA-SunnyBoy
Domoticz plugin to get SMA Sunny Boy 1.5/TriPower information

ONLY TESTED FOR Raspberry Pi

With Python version 3.7.3 & Domoticz version 2020.2

## Prerequisites

The Serial ID of the sunny power. But if you do not know it, just enter a fake value. Upon the first call the log will
tell you which Serial ID Domotics got back.

## Installation

Assuming that domoticz directory is installed in your home directory.

```bash
cd ~/domoticz/plugins
git clone https://github.com/fvdoorn1970/Domoticz-SMA-SunnyBoy.git
# restart domoticz:
sudo systemctl restart domoticz.service
```
In the web UI, navigate to the Hardware page. In the hardware dropdown there will be an entry called "SMA Sunny Boy".

## Known issues

## Updating

Like other plugins, in the Domoticz-SMA-SunnyBoy directory:
```bash
git pull
sudo /etc/init.d/domoticz.sh restart
```

## Parameters

| Parameter | Value |
| :--- | :--- |
| **IP address** | IP of the SMA Sunny Boy eg. 192.168.1.231 |
| **Password** | password for the User Group, not the Installer one |
| **Serial ID** | serial ID of the Sunny Boy |
| **Debug** | default is True, use this the first time if you do not know the serial ID |

## Acknowledgements

Forked from:
https://github.com/merlot-dev/Domoticz-SMA-SunnyBoy
Which was based on the script found here
https://community.openhab.org/t/example-on-how-to-access-data-of-a-sunny-boy-sma-solar-inverter/50963/19


