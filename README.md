# raspberrypi5-arm64

CRUX-ARM aarch64 ports overlay for RaspberryPi 5

To use these ports, download the `raspberrypi5-arm64.rsync` file to `/etc/ports`:
```
$ sudo wget -P /etc/ports https://git.crux.nu/crux-arm/raspberrypi5-arm64/raw/branch/3.8/raspberrypi5-arm64.rsync
$ sudo ports -u raspberrypi5-arm64
```

You may want to list it first in `/etc/prt-get.conf` to take advantage of ports overlay:
```
###
### prt-get conf
###

# note: the order matters: the package found first is used
prtdir /usr/ports/raspberrypi5-arm64
prtdir /usr/ports/core-arm64
prtdir /usr/ports/opt-arm64
prtdir /usr/ports/xorg-arm64
prtdir /usr/ports/core
prtdir /usr/ports/opt
prtdir /usr/ports/xorg
```
