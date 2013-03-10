MCP23017
========

Controlling MPC/MPD with push buttons and a MCP23017 chip

This script is based in this Adafruit tutorial: http://learn.adafruit.com/mcp230xx-gpio-expander-on-the-raspberry-pi


Don't forget to download booth files (the Adafruit_I2C.py file is like a "driver" for the chip) and follow this tutorial to install the python and the I2C tools: http://www.skpang.co.uk/blog/archives/575  (The "Example" part is not necessary).


Before try to run the script REBOOT YOUR RASPBERRY PI! If you don't get the results expected during the tutorial, reboot the Raspberry Pi!




To mount everything you'll need 5 push buttons and OPTIONAL 2 leds (one indicates the radio is off and the other indicates it's on) and 2 270R resistors to connect the LED's.

The connection of the buttons is something like this:
Stop button -> Pin GPA6
Volume - -> Pin GPA5
Volume + -> Pin GPA4
Previous -> Pin GPA3
Next -> Pin GPA2

The buttons are connected to the right port and to the Ground and don't need a resistor (the internal pullup resistors of the MCP are enabled)


The LED's are connected like the adafruit mounting scheme: http://learn.adafruit.com/system/assets/assets/000/002/467/original/MCP23017_bb.png

ON LED -> GPA0
OFF LED -> GPA1

The buttons are connected to the right MCP port and the resistor connect the other LED pin to the 3V3 rail.
