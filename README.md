# Salt-level-ultrasonic
ESP to read out a watersoftener Salt tank with ultrasonic sensor.

See README directory for more information on how to set this up and connect.

# Platforms
Currently supprted ESP32 S3 (wemos S3 mini) and ESP8266 (wemos d1 mini) platforms.
By default ESP32 S3 mini is used. If you want to use ESP8266 for example, edit file `esphome/salt-level.yaml`, comment out esp32 include and uncomment esp8266 include file.

```
packages:
  remote_package:
    url: https://github.com/fonske/Salt-level-ultrasonic
    ref: main
    files: 
      - esphome/.salt-level-labels-en.yaml
      # - esphome/.salt-level-labels-nl.yaml
      - esphome/board-esp32-wemos-s3.yaml
      # - esphome/board-esp8266-wemos-d1.yaml
```

# Translations
Currently supported languages are en, nl.
In order to change language, edit file `esphome/salt-level.yaml`, and change include file (esphome-/.salt-level-labels-<language>.yaml)

## Contact
Contact me: alphonsuijtdehaag at gmail dot com, if you are interested in a Wemos s3 mini and ultrasonic sensor (DFrobot) in a small black 3d printed box.
