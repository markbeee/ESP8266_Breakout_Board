# **Breakout board for ESP8266 modules ESP-12 and ESP-07**
 
The single sided self etchable pcb is designed to power the ESP-module, has a reset and flash (program) button, the necessary pull-up/ pull-down resistors and a USB-to-serial IC (CH340G) to connect the adapter board via micro USB to the USB port on a PC. You can also wire a serial connection directly to the RX/ TX module pins.

Please bear in mind that the module pins have a 3.3 volt signal level. If you use a signal source with 5 volt (e.g. an Arduino driven by 5 volt) the RX-pin has to be driven by a voltage divider or any kind of level shifter.

The module can be connected to a power source via USB, the Vcc-pin of the module (max. 3.6 volt) or via the Vin-pins (max. 12 volt, min. 4.8 volt).

You can also connect the RTS and DTR lines via the solder bridges. If you do, you can automatically flash the module without any hassle pressing buttons. Unfortunately there are some issues with the serial output with the Arduino IDE then.

The adapter can be placed on any breadboard and leaves one row on each side available to put in jumper wires.

As the pcb is single sided you have to connect three jumper wires on the bottom (see Eagle-files for directions).

ESP8266 Board Adapter 
![alt text](https://github.com/markbeee/ESP8266_Breakout_Board/images/Board_ESP8266.jpg "ESP8266 Board Adapter")

ESP8266 Board Adapter parts
![alt text](https://github.com/markbeee/ESP8266_Breakout_Board/images/Kit.jpg "ESP8266 Board Adapter parts")
