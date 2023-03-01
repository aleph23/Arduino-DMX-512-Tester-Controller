### **Arduino DMX 512 Tester and Controller**

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Hardware/v0.3/media/IMG_9399.JPG)
[![Arduino DMX-512 Tester and Controller](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Hardware/v0.0/media/youtube.JPG)](https://www.youtube.com/watch?v=TxBHMpAWDSY)

***

More info on the [Wiki…](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/wiki)

***

Tool for testing and controlling lighting for shows through the [DMX-512](http://en.wikipedia.org/wiki/Digital_Multiplex) protocol, ideal for quick testing of fixed or temporary lighting installations.
This project arises from the need to have a portable system to carry out rapid tests in lighting installations, without the need to install lighting consoles, interfaces or computers in outdoor, hostile or difficult-to-access environments.

Based on:
* [Arduino Mega 2560 Rev-3](http://www.arduino.cc/en/Main/ArduinoBoardMega2560)
* [Arduino Library Four DMX Universes v0.3 - 'Deskontrol'](http://www.deskontrol.net/blog/libreria-arduino-cuatro-universos-dmx/)
* [LCD Library v1.2.1 - Francisco Malpartida](https://bitbucket.org/fmalpartida/new-liquidcrystal/wiki/Home)

***
### Hardware v0.4
[Release notes...](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Hardware/Documentacion/Hardware%20-%20Notas%20Sobre%20la%20Version.md)
* Compatible with Firmware v0.9 - v1.3
* 4x20 LCD with backlight & contrast control via software  
* Powered from USB, batteries or external power supply  
* Navigation keypad  
* 4x4 numeric keypad  
* Potentiometer for analog control  
* On switch(does not apply to USB power)
* DMX output from terminal block, 3-pin XLR and 5-pin XLR 
* DMX output status LEDs
* Simulation in Proteus v7.7 SP2
* Schematic and PCB in Proteus v8.0 SP1

***

### Firmware v1.9

[Release Notes...](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/Documentacion/Firmware%20-%20Notas%20Sobre%20la%20Version.md)
* Compatible with Hardware v0.7

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Initial.PNG)

* Navigation from easily accessible and intuitive encoder 
* Quick insertion of values from the numeric keypad and encoder 
* Function to locate luminaire from the selected channel
* Startup with preselected DMX universe
* Selection of memory options at boot

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Initial%20Memory.PNG)

* Menu to select control modes, settings and tools

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Options.PNG)

* Control DMX Unitary, permite seleccionar 8 canales especificos ademas de mostrar el valor actual

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Control%20Unitary.PNG)

* DMX Matrix control, displays a 3 x 5 matrix with channel values displayed, start and end channel selectable

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Control%20Matrix.PNG)

* DMX Chaser control, allows sequencing channels automatically, the initial channel, end channel and time are selectable, allows sequencing channels manually from the encoder

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Control%20Chaser.PNG)

* DMX Sequencer control, allows sequencing between the universes stored in the EEPROM memory with a selected time

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Control%20Secuencer.PNG)

* DMX Multiply control, allows to fill values by multiplying the selected channels

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Control%20Multiply.PNG)

* Convert, allows converting between decimal and binary numbers that represent systems with dip switch

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Convert.PNG)

* Memory, EEPROM and RAM memory options, accessible from any control

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Memory.PNG)

* 8 memory banks to store, load and delete current values, accessible from the Memory menu

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Memory%20Bank.PNG)

* Config, allows you to assign the value of the Backlight, Key Light, Contrast and Bank Init

![](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Firmware/v1.9/LCD%20media/Config.PNG)

* Compiled in [Arduino IDE v1.0.6](http://www.arduino.cc/en/Main/OldSoftwareReleases)
* Arduino library four universes DMX v0.3 - [Deskontrol.net](http://www.deskontrol.net/blog/libreria-arduino-cuatro-universos-dmx/)
* LCD Library v1.2.1 - [Francisco Malpartida](https://bitbucket.org/fmalpartida/new-liquidcrystal/wiki/Home)

***

## Repository
[Firmware](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/tree/master/Firmware)
* Firmware versions are numbered consecutively. 
* The "Documentation" folder contains the information of the libraries used 
* The "Documentation/Hardware" folder contains specific hardware information
* El file "Firmware - Notas Sobre la Version.md" contains the history of changes in the different versions of the Firmware en Espanol

[Hardware](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/tree/master/Hardware)
* Hardware versions are numbered consecutively. 
* The "Documentation/Components" folder contains the information of the specific components
* El file "Hardware - Notas Sobre la Version.md" contiene el historico de cambios en las diferentes versiones del Hardware

[Simulador](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/tree/master/Simulador)
* Simulator versions are numbered consecutively

[Social](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/tree/master/Social)
* Contains the information of the activity in Webs, Blogs and Social Networks

[Software](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/tree/master/Software)
* Contains the software used for the project

[Licencias](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/tree/master/Licencias)
* Contains information about the licensing of the project

***

## License
* [GNU General Public Licence Version 3](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Licencias/Licence%20-%20Firmware.md)
* [Open Source Hardware (OSHW) v1.0](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Licencias/Licence%20-%20Hardware.md)

## Original Author
- Copyright (C) 2015
- [Daniel Roberto Becerril Angeles](https://www.facebook.com/daniel.3514)

[![Instructables](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Social/logos/Instructables%2050x50.jpg)](http://www.instructables.com/id/Arduino-DMX-512-Tester-and-Controller/)
[![Hack a Day](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Social/logos/hackaday%2050x50.jpg)](https://hackaday.io/project/5342-arduino-dmx-512-tester-and-controller)
[![Youtube](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Social/logos/Youtube%2050x50.png)](https://www.youtube.com/watch?v=TxBHMpAWDSY)
[![Tech Inside](https://github.com/daniel3514/Arduino-DMX-512-Tester-Controller/blob/master/Social/logos/techinside%2045x45.png)](https://techinsideblog.wordpress.com/)
