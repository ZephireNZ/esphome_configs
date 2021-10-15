## Zeph's ESPHome Configs

Configuration is stored in the `common` folder, grouped into "layers":

- Base config, configures things like Wifi and API password
- Device configs, which define core functionality (eg relays and LED for a smart plug)
- Functions, such as IR transciever or BLE monitor

These are then references in the root config, to build a complete config which can be deployed to a device.

Substitutions are used for things like device name, as well as secrets stored in `common/secrets.yaml`.