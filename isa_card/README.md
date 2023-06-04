ISA card for communication with the mainframe

(there are also some pictures with pumped saturation and contrast in this folder, you may check them out)\
![Top side photo](DSC_0181.JPG)
![Bottom side photo](DSC_0177.jpg)

I have reverse engineered the card, here is the schematic: [Schematic](isa_interface_schematic.pdf)\
Please consider, that there might be some mistakes. The U11 chip has no designator on the original PCB. Also, the IRQ jumpers seem to be a future feature or the PCB was also used for other systems/devices. Here it has no use, it works fine with the OFF setting. Also, in the software you can only set the base address of the card, no IRQ (in that era there was no autoconfig). The manual ignores the existence of it.

The 74LS74 flip-flops seem to have only testing purposes, they are generating a signal accessible on a pad (possibly testpoint) on the top of the PCB. The SIP resistor networks are in reality 9 resistor ones, one is not used, I used instead 8 resistor ones.

I reversed the card because I am thinking of replacing it with a new interface e.g. to the GPIO of a Raspberry PI (generating all the signals on the DB25 connector via software), but this is a long way to go... Also a "driver" would need to be written to dosbox or similar.
