# RibbaEdison
RibbaEdison - APA102 based 16x16 LED-Matrix fitted inside Ribba picture frame, controlled by Raspberry Pi in Python

These are some, but certainly not all, things that I used to build my RibbaEdison:
- Ikea Ribba picture frame, size 50x50cm
- 5m, white PCB, 60 LEDs/m APA102 strip
- Intel Edison with Intel or Arduino Breakout board
- 74AHCT125 level shifter
- Edison prototyping hat for soldering the logic level converter circuit
- 488x488x3,2mm wood plate (HDF)
- 2,5mm^2 copper wire for the outer power rails
- 1,5mm^2 copper wire for each power row
- 0,8mm silver copper wire
- lots of hot glue
- lots of solder
- Meanwell LRS-100-5 power supply
- adequate power supply casing
- XT60 connectors
- switch and power plug
- some WAGO clamps
- 50x70cm 5mm white foam board
- adhesive plastic foil and 50x70cm sheet of architecture paper for light diffusion
- sharp knife (scalpel)
- soldering iron 25W
- cordless screwdriver with 1mm metal drill
- some heat shrink tubes
- USB cord to power Raspberry Pi (USB A side cut off)
- some more wires, plugs, fuse and stuff
- I did NOT use a capacitor as seems recommended in many WS2812b tutorials. With my power supply, the APA102 LEDs, the way of soldering EACH LED there seems no need to add an additional capacitor. Please correct me if I am wrong.

Notes about the software:
- gameframe animations supported
- original blinkenlights animations supported
- analogue clock animation shows current time
- http server accepts strings that RibbaEdison displays as scrolling text
- tpm2.net server receives tpm2.net streams any time and interrupts playing animations
- when not connected to APA102 LEDs a virtual display can be used on the local computer that simulates the LED matrix. Very handy for development!
- currently all parameters are set in the RibbaEdison.py - also called "the brain"

A lot of fine tuning and enhancements are needed.

TODO-List:
- make html server look nicer (especially on mobile) and more capable
- enhance selection process of animations (enable, disable, randomness, weight)
- moodlight animation module!
- moodlight control via html server
- maybe make html server show gif previews of all animations
