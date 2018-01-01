# hassio

## razberry

- add `dtoverlay=pi3-miniuart-bt` to `config.txt`

- and add the following to `configuration.yaml`
  ```
  # Z-wave
  zwave:
    usb_path: /dev/ttyAMA0
  ```
