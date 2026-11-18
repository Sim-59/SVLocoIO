## Overview
**SVLocoIO** is a sketch for an Arduino based LocoIO module.
The code is e.g. used with a [LocoIO-A-InOut](https://simandit.de/simwiki/doku.php?id=modellbahn:digital#locoio-a-inout) hardware from [Sim&IT](https://simandit.de/Alle/about_simandit.php) that works like Arduino Pro Mini. There are found the schematic, assembly, bom and possibility to order the pcb for personal use.  
### Author
[Michael Hochmuth](https://github.com/Sim-59)

## Description
SVLocoIO is a LocoNet Interface with 16 I/O that can be individually configured as either Input or Output and emulates the functionality of a GCA50 module from Peter Giling. The idea for the LocoIO came from John Jabour.\
Configuration is done in Rocrail with Programming->LocoNet->LocoIO/GCA50...

Not all functions of the LocoIO-PIC-Vers-148 as used in the GCA123/GCA50 are implemented in the ClubNCaldes/SVLocoIO sketch.\
At first the missing "Active High" function in the sensor function was added in version 107 to the sketch as implemented in the PIC.\
In version 109 the continous output function was added if contact2 is activated like in PIC-Version-148. It realizes the invers function at the output.\
Next added support for flashing outputs.\
The version number is changed to 10 to avoid conflicts with development from [Silverailscolo](https://github.com/silverailscolo/SVLocoIO/)

## Credits
* Based on SVLocoIO from [Daniel Guisado Serra / ClubNCaldes](https://github.com/ClubNCaldes/SVLocoIO)
* Used [MRRwA LocoNet libraries for Arduino](http://mrrwa.org/)
* Inspired on the GCA123 board from [Peter Giling](http://www.phgiling.net/)
* Initialisation inspired by SVLocoIO from [Egbert Broerse](https://github.com/silverailscolo)

## Installation
In the Arduino-IDE the above said LocoIO hardware ist programmed like Arduino Pro Mini. To the blank hardware at first the bootloader must be programmed. There is an ISP connector for this purpose. Afterwards you can use an USB-TTL-adapter like  Arduino Pro Mini.\
Additional information found [here](https://simandit.de/simwiki/doku.php?id=modellbahn:digital_en#locoio-keypad-arduino).
