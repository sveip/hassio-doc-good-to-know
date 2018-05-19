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
- Resize resin-data partition to what is left on the usb-drive 
    - use x-forwarding for gparted: https://stackoverflow.com/questions/33072836/putty-x11-proxy-unsupported-authorisation-protocol 
    - doc: https://community.home-assistant.io/t/usb-boot-on-raspberry-pi-3/20358/33
- then set `root=/dev/sda2` in `cmdline.txt`
