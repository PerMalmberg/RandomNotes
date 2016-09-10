# Random Notes

# Arduino
[UNO Schematic](https://www.arduino.cc/en/uploads/Main/arduino-uno-schematic.pdf)

[ATmega 328P datasheet](http://www.atmel.com/Images/Atmel-42735-8-bit-AVR-Microcontroller-ATmega328-328P_datasheet.pdf)

To allow debugWire in AVR Studio to function when run against an Arduino UNO, reset-enable must [be cut](http://www.atmel.com/webdoc/avrdragon/avrdragon.section.gsr_osd_lc.html) to 
remove the capacitive load.

    Some precautions regarding the RESET line must be taken to ensure proper communication over the debugWIRE interface. If there is a pull-up on the RESET line, this resistor must be larger than 10 kΩ, and there should be no capacitive load. The pull-up resistor is not required for debugWIRE functionality. Other logic connected to the RESET line should be removed.

[Quote from AVR freaks](http://www.avrfreaks.net/comment/74027#comment-74027)

    PINx is used to READ the logic state of a port (x = A,B,...)
    PORTx is used to set (OUTPUT) the logical output state of a port.
    DDRx is used to control how the port behaves as an output (or input). The settings of DDRx and PORTx can interact in some interesting ways.
