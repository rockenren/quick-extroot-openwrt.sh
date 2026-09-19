# WARNING
This script if for OpenWRT 25.12+ only, it will not work on 24.10.x or lower versions.
For 24.10.x and lower versions of OpenWRT please use original script from: https://github.com/suuhm/quick-extroot-openwrt.sh

# quick-extroot-openwrt.sh
Easy and fast shell script to create an extroot on your Storage devives to extend the space on your Openwrt devices.

## How to run the script:
1. First put your wished Storage-Device (USB Stick / USB HDD etc.) in the device witb OpenWRT installed.

2. Now, simply run these lines on your serial/ssh console: 
```bash
wget https://raw.githubusercontent.com/rockenren/quick-extroot-openwrt.sh/refs/heads/main/quick-extroot.sh -qO- | \
sh -s -- --create-extroot 
```
3. Finally reboot your device and enjoy extroot.

<hr>

Alternatively you can just clone the project or copy/paste the file to your ssh console

<hr>

### Functions:
- ```--create-extroot <dev>``` Creating the extroot on your Device (Replace <dev> eg. `/dev/sda`)
- ```--create-swap <dev>``` Creating swap device on Device <dev> (Replace <dev> eg. `/dev/sda`)
- ```--set-apk2er``` Set up apk cache to extroot
- ```--fixup-extroot <dev>``` For some cases this may help you to fix up your Extroot
