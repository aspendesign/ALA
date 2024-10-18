# ALA
**Aspen Linear Actuator-A high speed, low noise, low cost actuator**

The main design differences from comparable in function hardware is as follows:

- The immediate difference here is a lack of a linear rail. By using plain bushings and a linear shaft, it is immensely cheaper, but more importantly, quieter. Near silent in fact.

- The method of locomotion has changed as well. Rather than using gt2 belts which create resonance, bulk, and require tension and looping around the pulley to properly drive, this design utilizes a tensioned UHMWPE string wrapped around the motor shaft, acting as a driven capstan. Such is elegant. More importantly though, it avoids further hardware and bulk.

- The shaft end of the shaft is a design for a tooless tensioning mechanism for the driving line. The string is tied off to the red, blue is fixed in place, and green is threaded as well. By twisting green, the red is pushed further away, tensioning it. The keyway between red and blue constrains red to only move linearly, thereby avoiding winding the driving line around the driven shaft.

- The last difference noted in the readme is how it indexes and attaches to the frame. It does so using a hirth joint, constraining it near the axis of movement to reduce moments, and to further streamline the design. It rigidly connects with a mating hirth and indexes at a number of positions. Such is entirely toolless, quick, and effective.

The hardware side of things is equally elegant. Using a silicone insulated four conductor wire, connections are made, utilizing a common ground. Said wire then goes to a control board to provide step+direction inputs as well as a power supply. For initial testing, a  4 axis breakout board and mach3 demo has been exceedingly helpful, but it will likely be an esp32 for the final product. There can be an integrated E-Stop button in numerous places, such as a simple button on the esp32 board, on the app, or otherwise. In order to avoid increasing wire count and clutter of rs485 communications, the esp32 may be programmed to act as an ammeter from the power supply, with a pause and reverse function to occur above a certain current threshold.

While there are numerous further avenues I seek to pursue, this is what currently has been designed. Significant documentation has been created and uploaded showing dates of ideas as well as multiple future ideas. **This is nevertheless still in progress, with more to be done.**

Shield: [![CC BY-NC-ND 4.0][cc-by-nc-nd-shield]][cc-by-nc-nd]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-NoDerivs 4.0 International License][cc-by-nc-nd].

[![CC BY-NC-ND 4.0][cc-by-nc-nd-image]][cc-by-nc-nd]

[cc-by-nc-nd]: http://creativecommons.org/licenses/by-nc-nd/4.0/
[cc-by-nc-nd-image]: https://licensebuttons.net/l/by-nc-nd/4.0/88x31.png
[cc-by-nc-nd-shield]: https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg
