# Introduction
This repository will contain all data about the Northwest Instruments System Inc. uAnalyst 200 state timing analyzer. Partially a collection of data from the internet, some thoughts of my own, partialy reverse engineering of some elements.

![est](adverts_articles/PC-Mag-1984-02-07_0319.jpg)
Advertisement from PC-MAG 1994/2

# Hardware Details
The hardware consists of a mainframe case with 8 slots for measurement cards. In the mainframe there are also 3 power supplies (2x15V connected in series to get +15V and -15V and +5V). The mainframe is connected to a PC via an 8-bit ISA card. Software runs under DOS. The manual states an IBM PC (TM) is required which implies an 8088 CPU. However I have made a connection from a Pentium 166 MMX without problems.

* [ISA interface card](isa_card/README.md)
* [21-006-00 PC interface](mainframe_cards/21-006-00_pc_interface/README.md)
* [21-013-00 C-2101 State Analyzer Controller](mainframe_cards/21-013-00_C-2101_state_analyzer_controller/README.md)
* [21-026-00 32 Channel Memory Board](mainframe_cards/21-026-00_32_channel_memory_board/README.md)
* [21-020-00 ITA Trigger Board/](mainframe_cards/21-020-00_ITA_trigger_board/README.md)
* [ITA Memory Board](mainframe_cards/ITA_memory_board/README.md)

There existed also a 003 Option Time Stamp Board and a 16 Channel Memory Board, none of which I own. On the timestamp there is a Manual in the Manuals section.

# Software
Software runs under DOS and has very little memory requirements (256KB or 512KB). I also tried FreeDOS - no problem. It can also run under the command line window in Windows 95/98, however due to the text/graphic mode switching it is quite annoying (Windows can display the graphics mode in a window, but each switch text->graphics mode switches back to fullscreen.
The software has also printing capabilities, one can print to LPT1-LPT3 and COM1-2 but also to a file (raw printer data). The printer data contains an ESC/P code, which can be easily converted these days to something modern (using e.g. [PrinterToPDF](https://github.com/RWAP/PrinterToPDF/))
