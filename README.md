<h1 align="center">
  <img align="center" src="Documentation/Logo/Marlin%20Logo%20GitHub.png" alt="Marlin4Delta Logo">
</h1>
# Marlin4Delta 3D Printer Firmware

Documentation has moved to [marlinfirmware.org](http://www.marlinfirmware.org).

## About this fork

This fork is primarily destined for calibrating individual delta diagonal rod and horizontal radius parameters for dimensional accuracy of your prints. Also include parameters for towers rotation (angle mismatch). See the section [Delta Settings](https://github.com/clefranc/Marlin4Delta/blob/master/Marlin/example_configurations/delta/biv2.5/Configuration.h#L315) in delta Configuration.h examples for instructions.

The hotend offset (if used) are properly implemented after homing and when printing.

When printing, menu will not return automatically to the status screen. Useful for eliminating stuttering with high segments per second.

## Specifics

* All thermal security and watchdog enabled by default.
* M665 command have been updated.
* Added G131 command (remove active extruder offset).
* Added G132 command (calibrate endstops offset).
* Added M99 command (disable stepper motor(s) for X seconds).
* Now shows 4 extruders on status screen (animated bed).
* Added new M2 M3 and M4 experimental commands.
* Switch to SD menu when SD card is inserted.
* Fix G29 for horizontal moves during probing (not U shaped).
* Added About... menu in LCD display (updated M115).

See the [wiki](https://github.com/clefranc/Marlin4Delta/wiki) (not completed yet) for more information.
<h1 align="center">
  <img align="center" src="Documentation/Status%20screen%20with%204%20extruders.jpg" alt="Status screen">
</h1>
## Development Only

__Not for production use – use with caution!__

This fork is from the [Marlin development branch](https://github.com/MarlinFirmware/MarlinDev/tree/dev) and DO NOT ALWAYS contains the most up-to-date Marlin code. I'll try to rebase it on the most up-to-date Marlin code from time to time. When reporting any issues, please check to see if they are resolved in the [Marlin development branch](https://github.com/MarlinFirmware/MarlinDev/tree/dev) first. But let me know if an update is available that can help you.

For the latest tagged version of Marlin (currently 1.0.2 – January 2015) you should switch to the [Release Repository](https://github.com/MarlinFirmware/Marlin).

## Current Status: Bug Fixing

[![Coverity Scan Build Status](https://scan.coverity.com/projects/6300/badge.svg)](https://scan.coverity.com/projects/6300)
[![Travis Build Status](https://travis-ci.org/clefranc/Marlin4Delta.svg)](https://travis-ci.org/clefranc/Marlin4Delta)

##### [RepRap.org Wiki Page](http://reprap.org/wiki/Marlin)

## Contact

This fork is maintained by [Christian Lefrançois ](https://github.com/clefranc).

## Credits and special thanks

Special thanks to the current Marlin dev team consisting of:

 - Scott Lahteine [@thinkyhead] - English
 - Andreas Hardtung [@AnHardt] - Deutsch, English
 - [@Wurstnase] - Deutsch, English
 - F. Malpartida [@fmalpartida] - English, Spanish
 - [@CONSULitAS] - Deutsch, English
 - [@maverikou]
 - Chris Palmer [@nophead]
 - [@paclema]
 - [@epatel]
 - Erik van der Zalm [@ErikZalm]
 - David Braam [@daid]
 - Bernhard Kubicek [@bkubicek]
 - Richard Wackerbarth [@Wackerbarth] - English
 - Roxanne Neufeld [@Roxy-3DPrintBoard] - English

More features have been added by:
  - Alberto Cotronei [@MagoKimbra]
  - Lampmaker,
  - Bradley Feldman,
  - and others...

## License

Marlin is published under the [GPL license](/Documentation/COPYING.md) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.

[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=ErikZalm&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)
