# Ender 3 v3 SE

Relatively cheap printer with some automatics. Requires some enhancements before being considered good enough.

## Firmware

[Marlin 2.1.x based](https://github.com/navaismo/Marlin_bugfix_2.1_E3V3SE) proved to be the best in terms of features and stability.

Look closely to different flavors for diffrent motherboards and make sure to use "OctoPrint" version if you control the printer via [Octoprint](https://octoprint.org/) which is highly recommended.

## Hardware mods

The following proved to work well:

1. [Add gantry support](https://www.thingiverse.com/thing:6516352)
2. [Rotate spool adapter 90°](https://www.thingiverse.com/thing:6631744)
3. [Filament guide](https://www.thingiverse.com/thing:6422862)
4. [Using Noctua fan + applying its resistor to PSU](https://www.reddit.com/r/Ender3V3SE/comments/1949xsc/creality_ender3_v3_se_fan_upgrade_replace_20mm/). Makes the printer almost silent but that's pricey.
5. [Official LED light bar](https://store.creality.com/eu/products/ender-3-v3-se-led-light-bar).
6. Orange silicone spacers for bed leveling. Springs are OK as well but silicone spacers are better.

### How to level the bed using silicone spacers

1. Install spacers, tighten screws.
2. Do automatic bed leveling.
3. Look for four corner values. If any of these stand out, adjust: tighten if the value is too high. Untighten if value is too low.
4. Repeat 2-3 until 0.0x in each corner.
5. Save map to memory.

### Useless mods

- Sonic Pad.
- Nebula.
- Wifi box.

It's way better to use Orange Pi or a long USB cable and install Octoprint.

## Software

1. [OrcaSlicer](https://www.orcaslicer.com/).
2. [Octoprint](https://octoprint.org/) for remote control and printing right from the slicer.

### SD card formatting

SD card should be formatted in FAT, 4096 allocation unit size:

```sh
mkfs.fat -s 8 /dev/mmcblk0p1
```
