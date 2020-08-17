Backlight
=========

## Software
```console
sudo pacman -Syu xorg-xbacklight
```

### Driver
```console
ls /sys/class/backlight
```

## Config

Rules to change brightness file group to video

```console
# /etc/udev/rules.d/backlight.rules
# ----------------------------------

ACTION=="add", SUBSYSTEM=="backlight", KERNEL=="intel_backlight", RUN+="/bin/chgrp video /sys/class/backlight/%k/brightness"
ACTION=="add", SUBSYSTEM=="backlight", KERNEL=="intel_backlight", RUN+="/bin/chmod g+w /sys/class/backlight/%k/brightness"

```

## Control
```console
xbacklight -set [1-100]
xbacklight -inc 10
xbacklight -dec 10

echo 500 >/sys/class/backlight/intel_backlight/brightness
```
