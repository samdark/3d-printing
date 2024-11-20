# Ender 3 v3 SE

## Is auto-leveling applied automatically?

Yes if you're on a stock Creality firmware. 
It happens regardless of auto calibration setting right before print.

You don't need to add `M420 S1` explicitly in your gcode.

Proof:

- [Firmware config](https://github.com/CrealityOfficial/Ender-3V3-SE/blob/main/Marlin/Configuration.h#L1522)
- [Explanation](https://marlinfw.org/docs/gcode/G028.html)
- Also, you can try holding Z-axis during first solid layer print. If it's moving then auto-leveling map is applied.

