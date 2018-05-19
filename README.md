# hassio

## razberry

- add `dtoverlay=pi3-miniuart-bt` to `config.txt`

- and add the following to `configuration.yaml`
  ```
  # Z-wave
  zwave:
    usb_path: /dev/ttyAMA0
  ```
## USB drive filesystem

- Do: https://www.raspberrypi.org/documentation/hardware/raspberrypi/bootmodes/msd.md

- then set `root=/dev/sda2` in `cmdline.txt`
