<p align="center">
  <img alt="Jasen's Customs Logo" src="https://jasenscustoms.com/cdn/shop/files/jcc_logo.png?width=125" />
</p>

The <a href="https://jasenscustoms.com/collections/fight-stick-pcbs/products/integrated-pico-fighting-board-gp2040ce">Integrated Pico Fighting Board</a> is an open source arcade fight stick PCB design made available under the Creative Commons Attribution-Non Commercial Sharealike 4.0 International License. This is a solely **hardware** project that is designed to easily run **unmodified** GP2040-CE firmware. That has always been the intent despite narratives suggesting otherwise.

![image](https://github.com/user-attachments/assets/0402e3fc-74b1-4511-bbe3-5bbda8b60b5d)

It was designed to follow the Fighting Game Community Layout Generally Accepted Standard originally pioneered by AkiShop. This design was adopted by Brook for most of their fighting boards at the behest and urging of myself and a few other makers in the space early in Brook's entry to the market. The goal was to make the IPFB a low cost, easy drop-in in replacement for the PS360+ or any Brook Board if a person so chose.

## Design Files

All design files are made using Autodesk EagleCAD and will only be published in that format. Gerbers and Centroids will not be provided. A basic BOM will also be provided. This is to allow hobbyists with some design experience to use their choice of board house to produce their PCBs. There are many to chose from, and it is not our intent to influence your choice. All files are provided as-is without any guarantee of support or help. 

## Sale Channels

Note: The only entity that may sell the Integrated Pico Fighting Board Design is at the link above. If you wish to offer this design commercially, please reach out to [jasenhicks@jasenscustoms.com ](mailto:jasenhicks@jasenscustoms.com). If others are approved to sell the design, they will be listed here. I encourage you to inform me if you see unapproved commercial sale of the IPFB. As of now, I have chosen to stop production of the IPFB. A full discussion can be found on our discord, linked below.

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

## Firmware

No custom firmware is needed or provided for the Integrated Pico Fighting Board. Because the pin definitions are derived from FeralAI's carrier board, firmware for the Pico Fighting Board is expected to be compatible with minimal settings changes. Steps to customize GP2040-CE settings to fully utilize Turbo and Playstation authentication are indicated below.

### Settings
To manually adust the PicoFightingBoard firmware to work perfectly with the IPFB, just adjust these settings.

#### Turbo
- Add on Configuration:
  - Enable turbo
  - Turbo LED Pin 23
  - Save
- Pin Mappings:
  - Set pin 28 to Turbo
  - Save

#### PS5 (or PS4)
- Input Mode Settings
  - Current Input Mode: PS5 (or PS4)
  - Authentication Settings: Host USB
- Boot Input Modes
  - Set B4 to PS5 (or PS4)

#### XBone
- Boot Input Modes
  - Set R1 to XBone

## Support

All files are provided as is and without warranty.

For issues with Integrated Pico Fight Board hardware that was bought and sold via JasensCustoms.com, please reach out via [Jasen's Customs Discord](https://discord.gg/M9E8PFHSCm).

To discuss GP2040-CE firmware including features, issues, or anything else please join the [OpenStick GP2040-CE Discord](https://discord.gg/k2pxhke7q8) or [create a GitHub issue](https://github.com/OpenStickCommunity/GP2040-CE/issues/new).

Hardware change suggestions can be submitted as GitHub issues on this repository, and will be reviewed on a case by case basis by the JasensCustoms.com team. Not all suggestions will be implemented.

## Acknolwedgements

- [RegentOfOrigin](https://github.com/RegentOfOrigin) for helping manage the GitHub
- [wrennnnnn](https://github.com/wrennnnnn). for the initial management and compiling of the FW with the IPFB Config.h file
- [The entire Open Stick Community](https://github.com/OpenStickCommunity) for the GP2040-CE firmware
- Particularly [FeralAI](https://github.com/FeralAI) for the initial work in designing and making the [PicoFightingBoard](https://github.com/FeralAI/PicoFightingBoard) available

Copyright for the Pico Fighting Board is held by FeralAI, 2021.
Copyright for GP2040-CE is held by The Open Stick Community, 2024.
