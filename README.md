# Domoticz-SMA-SunnyBoy
Domoticz plugin to get SMA Sunny Boy 1.5 information

ONLY TESTED FOR Raspberry Pi

With Python version 3.5 & Domoticz version 4.10717 (stable)

## Prerequisites

If the ID's in the script doesn't get the expected information, you have to find them out by using packetcapture while accesing the  SMA Sunny Boy with your browser

## Installation

Assuming that domoticz directory is installed in your home directory.

```bash
cd ~/domoticz/plugins
git clone https://github.com/merlot-dev/Domoticz-SMA-SunnyBoy
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
| **Debug** | default is True |

## Acknowledgements

Based on the script found here

https://community.openhab.org/t/example-on-how-to-access-data-of-a-sunny-boy-sma-solar-inverter/50963/19


