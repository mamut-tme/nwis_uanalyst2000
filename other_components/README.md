one of the 15V power supplies:
![DSC_0177.JPG](DSC_0177.JPG)
Below the fuse you can see 3 yellowish capacitors and there is also one a bit to the right. These are metalized paper capacitors, manufactured by RIFA . Their lifespan is about 30 years... please inspect them before running the system, cracks in the casing are possible to be seen with a bare eye. In any case I recommend replacing them. It is possible to buy direct replacements in the same technology made by Kemet (they bought RIFA), but they are quite expensive and franky speaking I don't trust that technology. I suggest replacing them with some MKP (metalized polypropylene foil) caps, X2/Y2 rating as below:
* 100nF 250VAC X2 class (1 pcs per PSU), pin raster is originally about 21mm, but there is also a pad allowing to install a 15 mm cap
* 2,2nF (marked 2200pF) 250VAC Y2 class (3 pcs per PSU), pin raster = 10mm

These caps are here to reduce EMC emissions, meaning general noise. Various advice on the internet say, that these caps have 20% tolerance, so the exact value is not so important, but I am not so sure. These caps have some reactance/inductance, which has been calculated/selected based on the frequency of the generated noise, so I would stick with the values.

the 5V power supply with the remote sensing voltage regulator (the upper two cables in the left screw terminal seem to be for that purpuse):
![DSC_0189.JPG](DSC_0189.JPG)
Similarily to the power supplies aboce there are 3 caps of same technology, which should be replaced.
* 4,7nF (marked 4700pF) 250V Y2 class (3 pcs), pin raster=10 mm
there is also 1 bigger cap X2 rated, in my case it is a different type, branded by Philips.

Power Distribution Board (just a mains voltage splitter):
![DSC_0180.JPG](DSC_0180.JPG)
Power Distribution Board on top of the EMC filter:
![DSC_0181.JPG](DSC_0181.JPG)
front panel LED bottom:
![DSC_0182.JPG](DSC_0182.JPG)
seems that the LED are multiple LEDs in one package, the resistors just limit the current, the 3 wires going to the board are +5V and 2x GND
front panel LED top:
![DSC_0183.JPG](DSC_0183.JPG)
