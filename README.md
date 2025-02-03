# Pico2_12bitADC_PCMAudio
This is a PCB to neatly package a Raspberry Pi Pico 2, AD9226 ADC PCB and a PCM1802 audio board for capture with hsdaoh.
Specifically designed to still be usefull without smds (no head switch input then). Through-hole only works just fine.
For use with https://github.com/steve-m/hsdaoh-rp2350/tree/pcm1802

<img src="https://github.com/Sev5000/Pico2_12bitADC_PCMAudio/blob/main/Pico2%20Adapter%20PCB%20Render.png?raw=true" alt="">

Features:
- The Pico 2 can be socketed with and without a DVI sock
- Mounting holes for the AD9226 pcb, PCM1802 and a socketed Pi Pico 2 with DVI sock (original and adafruit verfied)
- Audio input with either chinch or 3.5mm jack
- Jumper to choose between head switch input and clipping bit of the AD9226
- Protected head switch input has footprints for jst, as well as edge and horizontal SMA/SMB

<img src="https://raw.githubusercontent.com/Sev5000/Pico2_12bitADC_PCMAudio/refs/heads/main/Pico2%20ADC%20Board.webp" alt="">

What you need to build: 
1x This PCB (Send the Gerber .zip to JLC, PCBWay, ..)

1x Raspberry Pi Pico 2

1x AD9226: https://aliexpress.com/item/1005003038271519.html

1x PCM1802: https://aliexpress.com/item/1005006412873984.html

2x RCA-105 or RCA-106: https://aliexpress.com/item/1005006152724809.html

1x PJ-324M 5P: https://aliexpress.com/item/1005006146950431.html

1x 3pin 2.54mm pin header vertical or horizontal for the headswitch/overflow selection jumper

No SMD variant:

1x DVI-Sock: https://github.com/Wren6991/Pico-DVI-Sock for a flush fit with the pcb edge, otherwise the adafruit DVI sock works fine too

1x 9pin 2.54mm pin-socket header 

1x 2x10pin 2.54mm pin-socket header

2x 15pin 2.54mm pin-socket header

SMD Variant:
1× Stewart SS-53000-001 connector (See https://github.com/Wren6991/Pico-DVI-Sock BOM for details)

8× 0402 270 ohm resistors

5x 0805 100nF ceramic capacitors

For head switch input:

1x SOD123 3.3V zener diode

1x SOD123 standard diode

1x 0805 1k resistor

1x edge SMA/SMB or horizontal SMA/SMB and/or 2pin header

Notes:
The PCM1802 board needs MODE0 and MODE1 bridged *and* connected to 3.3V with a wire (Those boards have a design error):

<img src="https://raw.githubusercontent.com/Sev5000/Pico2_12bitADC_PCMAudio/refs/heads/main/PCM1802Mod.webp" alt="">

