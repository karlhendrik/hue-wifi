# Hue WiFi

#### This scripts will forward all the traffic from Raspberry Pi **wlan0** interface to **eth0** 

## Why?

Since [Philips Hue Bridge](https://www.philips-hue.com/en-us/p/hue-bridge/046677458478) does not support officialy WiFI - this simple scripts acts as a workaround to that problem. 

## Requirements

* Any Raspberry (with ethernet port) should work,
* Philips Hue Bridge,
* RJ-45 cable
* Git
* Raspberry Pi OS

## Setup
I use Raspberry Pi OS for this setup. After installing the distro, just clone the repository:

**NOTE! Raspberry Pi must be connected to existing WiFI network for this to work**

```
git clone git@github.com:karlhendrik/hue-wifi.git
```

After cloning the repository, you can copy-paste the following commands:

```
cd hue-wifi/
chmod +x bridge.sh
bash bridge.sh
```

Now the script will install all the necessary dependecies and do all the configurations.
After the script is finished all the traffic from **wlan0** should be forward to **eth0** interface.

Connect RJ-45 cable between Raspberry Pi and Philips Hue bridge and now your Philips devices in you network should see the brdige in the network