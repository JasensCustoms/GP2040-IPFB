<p align="center">
  <img alt="Jasen's Customs Logo" src="https://jasenscustoms.com/cdn/shop/files/jcc_logo.png?width=125" />
  <img alt="GP2040-CE Logo" src="https://raw.githubusercontent.com/OpenStickCommunity/Site/main/docs/assets/images/gp2040-ce-logo.png" />
</p>


<p align="center">
  Multi-Platform Gamepad Firmware for the <a href="https://jasenscustoms.com/collections/fight-stick-pcbs/products/integrated-pico-fighting-board-gp2040ce">Integrated Pico Fighting Board</a>.
</p>

<p align="center">
  <img alt="" src="https://img.shields.io/github/license/JasensCustoms/IPFB" />
  <img alt="" src="https://img.shields.io/github/actions/workflow/status/JasensCustoms/IPFB/cmake.yml" />
</p>

Closed source board based on FeralAI's innovative Pico Fighting Board. Designed to have the same level of polish as any purchasable board, and to be inter-compatible with existing Brook offerings.

## GP2040-CE Links

[Installation](https://gp2040-ce.info/installation) | [Usage](https://gp2040-ce.info/usage) | [GP2040-CE GitHub](https://github.com/OpenStickCommunity/GP2040-CE)

Full documentation for GP2040-CE can be found at [https://gp2040-ce.info](https://gp2040-ce.info)

## GPIO Settings

Main Buttons and Directions:

- GPIO 0: Left
- GPIO 1: Up
- GPIO 2: Down
- GPIO 3: Right
- GPIO 4: HOME (PS)
- GPIO 5: SELECT (SHARE)
- GPIO 6: START
- GPIO 7: Punch 1
- GPIO 8: Punch 2
- GPIO 9: Punch 3
- GPIO 10: Punch 4
- GPIO 11: Kick 1
- GPIO 12: Kick 2
- GPIO 13: Kick 3
- GPIO 14: Kick 4

RGB Data Channel

- GPIO 15: RGB Data

Player LEDS (Version 2.0+ PCB can designate these as other functions as the resistor on the line has been removed)

- GPIO 16: Player 1 LED
- GPIO 17: Player 2 LED
- GPIO 18: Player 3 LED
- GPIO 19: Player 4 LED

Modern Controller Buttons, Turbo Functions

- GPIO 20: Touch Pad Click
- GPIO 21: L3
- GPIO 22: R3
- GPIO 23: TURBO LED (Version 2.0+ PCB can designate this as another function as the resistor on the line has been removed)
- GPIO 28: TURBO KEY

I2C Lines both have been pulled high via resistor (3.3V)

- GPIO 26: SDA
- GPIO 27: SCL

USB Passthrough GPIO

- GPIO 24: DATA PLUS
- GPIO 25: DATA MINUS

## Support

If you would like to discuss features, issues or anything else related to GP2040-CE please [create an issue](https://github.com/OpenStickCommunity/GP2040-CE/issues/new) or join the [OpenStick GP2040-CE Discord](https://discord.gg/k2pxhke7q8) support channel.

## Acknolwedgements

- [RegentOfOrigin](https://github.com/RegentOfOrigin) for helping manage the GitHub
- [wrennnnnn](https://github.com/wrennnnnn). for the initial management and compiling of the FW with the IPFB Config.h file.

