Connectors, left from top:
* 2x 15V power (the connectors are interchangeable, the connections on the PCB create a series connection).
* front panel LED connector, +5V and 2x GND
* 5V power, with a connection for the voltage feedback signal

Right from top:
- EXT (input) on a BNC connector - external trigger
- CL  (output) on a BNC connector - programmable output or interconnect for dual state/timing analyzer

Some words about the supply section:
there are two +5V rails: a normal rail with filtered just with a electrolytic (1000uF/10V) + ceramic capacitor (220nF) and a second rail additionally filtered with a LC filter (10uH+same caps as the first rail). The inductor is a Renco RL-1256-1-10 (10uH, 0,01 Ohms, Irms=9A). On my board there was an actual fault arround this inductor: half of one of the top pads was missing and the metal plating of the pad was most likely gone. Someone soldered the component from both sides, but at some point the connection got weaker and the final cap was very slowly working, after some wiggling I got it to work, afterwards fixed with a piece of wire soldered below.

The additionally filtered voltage rail is used only by the ITA cards! (and they don't use the normal 5V at all). So if the cards are not detected it is most likely a problem of this rail...

The bodged wire on the bottom side seems like a factory thing, there is a trace missing on the top layer...

![DSC_0174.JPG](DSC_0174.JPG)
![DSC_0176.JPG](DSC_0176.JPG)
