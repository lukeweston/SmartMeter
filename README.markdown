 This design is almost identical to the Smart Energy Groups SEGMeter (for which kits can be purchased, from Sam @ Smart Energy Groups), however, I have started making some improvements.
(When I find where I put the original CAD/CAM files that actually correspond to the SEGMeter boards that exist already, I will upload those too.)

* The schematic is drawn significantly more cleanly and tidy
* Integrated AVR on the board (that is, not an Arduino shield)
* Surface-mount components used, making the board smaller and more compact and (arguably) easier to assemble
* Programming of the AVR through the Arduino IDE is done using an external FTDI adapter, just like the Arduino Pro.
* A header is provided to connect a phototransistor, which can be stuck onto the front of a modern electricity meter to read the frequency of the flashing LED.
* An open-collector transistor output (connected to 12 V) is provided on the board instead of a low-current reed relay. This can be connected to the coil of a power relay to switch 240 VAC.

Things to do:
--------------

* Design and test improvments to the analog input filter/coupling circuits
* Fix the silkscreen layers on the PCB so they're neatly arranged and tidy, in the appropriate places, and not overlapping or over the pads.
* Run ERC and DRC
* Generate Gerber files

