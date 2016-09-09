# Random Notes

# Arduino
To allow debugWire in AVR Studio to function when run against an Arduino UNO, reset-enable must [be cut](http://www.atmel.com/webdoc/avrdragon/avrdragon.section.gsr_osd_lc.html) to 
remove the capacitive load.

    Some precautions regarding the RESET line must be taken to ensure proper communication over the debugWIRE interface. If there is a pull-up on the RESET line, this resistor must be larger than 10 kΩ, and there should be no capacitive load. The pull-up resistor is not required for debugWIRE functionality. Other logic connected to the RESET line should be removed.
