<p align="center">
  <img alt="Jasen's Customs Logo" src="https://jasenscustoms.com/cdn/shop/files/jcc_logo.png?width=125" />
</p>

The <a href="https://jasenscustoms.com/collections/fight-stick-pcbs/products/integrated-pico-fighting-board-gp2040ce">Integrated Pico Fighting Board</a> is now open sourced under the Creative Commons Attribution-Non Commercial Sharealike 4.0 International License. This is a HARDWARE device that was designed to easily run the GP2040-CE firmware UNMODIFIED. That has always been the intent despite narratives suggesting otherwise.

It was designed to intentionally follow the Fighting Game Community Layout Generally Accepted Standard. This was originally pioneered by AkiShop and was adopted by Brook for most of their fighting boards at the behest and urging of myself and a few other makers in the space early in Brook's entry to the market. The goal was to make the IPFB a low cost, easily dropped in replacement for the PS360+ or any Brook Board if a person so chose.

## Design Files

All design files are make using Autodesk EagleCAD and will only be published in that format. Gerbers and Centroids will not be provided. A basic BOM will be provided. This is to allow hobbyists with some design experience to have thier favortie board house make PCBs for them, without influencing whom they use. There are many to chose from. All files are provided as-is without any guarantee of support or help. 

## Sale Channels

Note: The only entity that may sell the Integrated Pico Fighting Board Design is at the link above. If you wish to offer this design commercially, please reach out to [jasenhicks@jasenscustoms.com ](mailto:jasenhicks@jasenscustoms.com). If others are approved to sell the design, they will be listed here. I encourage you to inform me if you see unapproved commercial sale of the IPFB. As of now, I have chosen to stop production of the IPFB. A full discussion can be found on our discord, linked below.

## GP2040-CE Firmware

This repository will not house any GP2040 firmware releases, nor will it build them. 

## GPIO Settings

The Integrated Pico Fighting Board derived many of its pin definitions from FeralAI's carrier board. As such you should be able to use the current releases of the Pico Fighting Board published at the official GP2040-CE GitHub. 

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

If you have any issues with the Integrated Pico Fight Board hardware that was bought and sold via JasensCustoms.com, please reach out on the [Jasen's Customs Discord](https://discord.gg/M9E8PFHSCm).

If you would like to discuss features, issues or anything else related to GP2040-CE in general please [create an issue](https://github.com/OpenStickCommunity/GP2040-CE/issues/new) or join the [OpenStick GP2040-CE Discord](https://discord.gg/k2pxhke7q8) support channel.

Files are all provided as is without warranty. Please use the issues tracker to make suggestions on hardware changes. They will be handled case by case by the JasensCustoms.com team. Not all recommendations will be implemented. 

## Acknolwedgements

- [RegentOfOrigin](https://github.com/RegentOfOrigin) for helping manage the GitHub
- [wrennnnnn](https://github.com/wrennnnnn). for the initial management and compiling of the FW with the IPFB Config.h file
- [The entire Open Stick Community](https://github.com/OpenStickCommunity) for the GP2040-CE firmware, and most specifically FeralAI for the intial work.

Copyright for portions of project GP2040-IPFB are held by the Open Stick Community, 2024 as part of project GP2040-CE under MIT License ([included here](LICENSE)).  All other copyright for project GP2040-IPFB are held by Jasen's Custom, 2024.
