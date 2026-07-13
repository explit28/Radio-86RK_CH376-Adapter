**Radio-86RK CH376 Adapter**

CH376 USB storage adapter PCB for the Radio-86RK v1.4 computer board by Sergey Kiselev.

This small adapter board connects a CH376/CH376S USB module to the Radio-86RK expansion/bus connector and allows the machine to communicate with USB storage hardware when used together with compatible ROM/software support.


##Project status

This repository contains the PCB production files and reference photos for the CH376 adapter.

##What is this board for?

The Radio-86RK is a Soviet 8080-compatible home computer. This adapter is intended to make it easier to connect a CH376 USB interface module to the Radio-86RK bus.

The CH376 module provides a simple parallel interface that can be used by retro computers to access USB mass-storage devices, depending on the ROM/software used on the target machine.

##Typical use case:

Radio-86RK v1.4 mainboard
CH376/CH376S USB module (Check Pinout! There are different modules with different pinout on the market!)
Adapter PCB from this repository
Compatible ROM or disk operating system with CH376 support
Compatibility

##Designed for:

Radio-86RK v1.4
Sergey Kiselev Radio-86RK board layout
CH376/CH376S module with parallel bus interface

##Not guaranteed for:

other Radio-86RK board revisions
heavily modified boards
different CH376 module pinouts
serial-only CH376 modules

Before connecting power, compare your CH376 module pinout with the adapter pinout.


##Images
Top side
<img width="937" height="498" alt="CH376_Adapter_Top" src="https://github.com/user-attachments/assets/f9d2880f-8dec-4d8b-8954-f7cd83f3e7b3" />


Bottom side
<img width="967" height="533" alt="CH376_Adapter_Bottom" src="https://github.com/user-attachments/assets/f9952c0a-2d92-49c7-80aa-0a97a18bdcc0" />


Traces
<img width="1053" height="332" alt="CH376_Adapter_Traces" src="https://github.com/user-attachments/assets/39cfcf91-e5fd-41d9-9d18-c1f52594cedd" />


Pinout
<img width="672" height="1080" alt="CH376_Adapter_Pinout" src="https://github.com/user-attachments/assets/a15918a4-fcc6-4e3e-aa4c-7e7c3266d929" />


Cable connection
<img width="960" height="1280" alt="CH376_cable_connection" src="https://github.com/user-attachments/assets/407085cc-63b8-4484-84d7-3b3d9660686e" />




CH376 signals

The adapter is intended for the CH376 parallel interface. The important signals are:

Signal	Function
D0–D7	8-bit data bus
A0	Register select
RD	Read strobe
WR	Write strobe
CS / EXT_CS	Chip select
+5V	Power supply
GND	Ground

Check the exact pin order on your module before soldering or connecting the cable.

##PCB manufacturing
The Gerber and drill files are included in the Gerber directory as a zip file. They can be uploaded to a PCB manufacturer such as PCBWay, JLCPCB, or another Gerber-compatible board house.


##Recommended before ordering:

Open the Gerber files in a Gerber viewer.
Check board outline and hole positions.
Check that the pin header orientation matches your installation.
Compare the generated preview with the reference images in this repository.
Assembly notes

##Before powering the Radio-86RK:

Check for shorts between +5V and GND.
Verify CH376 module orientation.
Verify cable orientation.
Check continuity for all bus signals.
Do not connect or disconnect the adapter while the computer is powered on.
Software / ROM support

This adapter is only the hardware interface. The Radio-86RK still needs software or ROM support that knows how to communicate with the CH376 module.
The simplest way is to use PeaceDOS Operating System: https://github.com/explit28/peace-dos

**Warning**
**Incorrect wiring can damage the CH376 module, the adapter, or the Radio-86RK bus interface.**

Use this project at your own risk. Always verify the pinout before applying power.

##Credits
Radio-86RK v1.4 board: Sergey Kiselev<br>
PeaceDOS: Dmitry Ivanov<br>
Adapter PCB: PC-RATH.de<br>

##License
No license has been specified yet.

If you want others to build, modify, and reuse this project, add an explicit open-source hardware license, for example:

CERN-OHL-S
CERN-OHL-W
CC BY-SA 4.0

Until a license is added, the files are publicly visible but reuse rights are not clearly defined.

<a href="https://www.pcbway.com/project/shareproject/Radio_86RK_CH376_Adapter_78427d9a.html"><img src="https://www.pcbway.com/project/img/images/frompcbway-1220.png" alt="PCB from PCBWay" /></a>
