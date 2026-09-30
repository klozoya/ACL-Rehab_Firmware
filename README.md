# ACL Rehab Firmware

Zephyr application for the ACL rehabilitation device.

## Requirements

- nRF Connect SDK v3.4.1 with its matching toolchain
- A supported Nordic development board

Keep the SDK installation outside this repository. The current SDK installation is at `/opt/nordic/ncs/v3.4.1`.

## Build

Choose the board target that matches your hardware, then build from this directory:

```sh
west build -b <board_target> .
```

For example, the board target for an nRF52840 DK is `nrf52840dk/nrf52840`. The target must match the board you will flash.

The application currently prints a startup message. Board-specific features and rehabilitation logic can be added once the hardware is identified.