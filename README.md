# **Breakout board for ESP8266 modules ESP-12 and ESP-07**
 
The single sided self etchable pcb is designed to power the ESP-module, has a reset and flash (program) button, the necessary pull-up/ pull-down resistors and a USB-to-serial IC (CH340G) to connect the adapter board via micro USB to the USB port on a PC. You can also wire a serial connection directly to the RX/ TX module pins.

![image](/images/Board_ESP8266.jpg)

Please bear in mind that the module pins have a 3.3 volt signal level. If you use a signal source with 5 volt (e.g. an Arduino driven by 5 volt) the RX-pin has to be driven by a voltage divider or any kind of level shifter.

The module can be connected to a power source via USB, the Vcc-pin of the module (max. 3.6 volt) or via the Vin-pins (max. 12 volt, min. 4.8 volt).

![image](/images/Kit.jpg)

You can also connect the RTS and DTR lines via the solder bridges. If you do, you can automatically flash the module without any hassle pressing buttons. Unfortunately there are some issues with the serial output with the Arduino IDE then.

The adapter can be placed on any breadboard and leaves one row on each side available to put in jumper wires.

As the pcb is single sided you have to connect three jumper wires on the bottom (see Eagle-files for directions).

#### Parts needed (SMD)

| Part | Device                    | Value |
|------|---------------------------|-------|
| C1   | C-EUC0805                 | 22pF  |
| C2   | C-EUC0805                 | 22pF  |
| C3   | C-EUC0805                 | 100nF |
| C4   | C-EUC1206                 | 10µF  |
| C5   | C-EUC1206                 | 10µF  |
| IC1  | REG1117                   |       |
| JP1  | PINHD-1X8BIG              |       |
| JP2  | PINHD-1X8BIG              |       |
| JP3  | USB_MICROB_PLUGCONN-11752 |       |
| Q1   | CRYSTALHC49UP             | 12MHz |
| R1   | R-EU_M0805                | 4k7   |
| R2   | R-EU_M0805                | 4k7   |
| R3   | R-EU_M0805                | 4k7   |
| R4   | R-EU_M0805                | 4k7   |
| R5   | R-EU_M0805                | 1k    |
| R6   | R-EU_M0805                | 1k    |
| SJ1  | SJ                        |       |
| SJ2  | SJ                        |       |
| U$1  | ESP8266_ESP-12/ ESP-07    |       |
| U$2  | CH340G                    |       |
| U$3  | TACTILE-SWITCH-7914G      |       |
| U$4  | TACTILE-SWITCH-7914G      |       |