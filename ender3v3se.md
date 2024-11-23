# Ender 3 v3 SE

## Things to buy/use regularly

- Adhesive glue.
- Brass nozzles.
- Silicone sock.

## Is auto-leveling applied automatically?

Yes if you're on a stock Creality firmware. 
It happens regardless of auto calibration setting right before print.

You don't need to add `M420 S1` explicitly in your gcode.

Proof:

- [Firmware config](https://github.com/CrealityOfficial/Ender-3V3-SE/blob/main/Marlin/Configuration.h#L1522).
- [Explanation](https://marlinfw.org/docs/gcode/G028.html).
- Hold Z-axis during first solid layer print. If it's moving then auto-leveling map is applied.

## Does auto-leveling set Z-offset correctly

Yes, it does. If first layer doesn't stick, use glue.

## Good upgrades

- [Official LED light bar](https://store.creality.com/eu/products/ender-3-v3-se-led-light-bar).
- Orange silicone spacers for bed leveling. Springs are OK as well but silicone spacers are better.

## How to level the bed using silicone spacers

1. Install spacers, tighten screws.
2. Do automatic bed leveling.
3. Look for four corner values. If any of these stand out, adjust: tighten if the value is too high. Untighten if value is too low.
4. Repeat 2-3 until 0.0x in each corner.
5. Save map to memory.

## Not necessary

- Sonic Pad.
- Nebula.
- Wifi box.

It's way better to use Orange Pi and install Octoprint / Klipper there.

## Good upgrades to print

Here's [my collection at printables.com](https://www.printables.com/@samdark_2524499/collections/1863226).