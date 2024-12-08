# Pico2_12bitADC_PCMAudio
PCB to neatly package a Raspberry Pi Pico 2, AD9226 ADC and PCM1802 audio board for capture with hsdaoh.
Specifically designed to still be usefull without smds (no head switch input then).
For use with https://github.com/steve-m/hsdaoh-rp2350/tree/pcm1802

<img src="https://github.com/Sev5000/Pico2_12bitADC_PCMAudio/blob/main/Pico2%20Adapter%20PCB%20Render.png?raw=true" alt="">

Features:
- The Pico 2 can be socketed with and without a DVI sock
- Mounting holes for the AD9226 pcb, PCM1802 and a socketed Pi Pico 2 with DVI sock (original and adafruit verfied)
- Audio input with either chinch or 3.5mm jack
- Jumper to choose between head switch input and clipping bit of the AD9226
- Protected head switch input has footprints for jst, edge and horizontal SMA/SMB

Notes:
The PCM1802 board needs MODE0 and MODE1 bridged *and* connected to 3.3V with a wire (Those boards have a design error).
