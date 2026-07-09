# DMH-Output
Kosmo format output module

<img width="651" height="869" alt="image" src="https://github.com/user-attachments/assets/49cfe7ba-f8a9-4ebc-8888-ad162b3b316b" />

<img width="651" height="869" alt="image" src="https://github.com/user-attachments/assets/359aef5b-c412-4d04-ab10-f7115af3be43" />

<img width="651" height="869" alt="image" src="https://github.com/user-attachments/assets/43efbdd4-0ef6-4521-95e2-ccb7a9f8663e" />


## Features

### Line outputs and main volume

The L and R inputs accept the usual (Eurorack) modular synth audio amplitude of 10 V peak-to-peak.
The line level L and R outputs accept both balanced TRS and unbalanced TS cables.
The main volume control affects both L and R channels. The reduction factor can be set from from -infinite (silence) to -3 dB (max).
Since the usual 10 Vpp amplitude corresponds to around +13 dBu, this means the module can output from -infinite up to +10 dBu.
The precision dBu meter will max out at +6 dBu (red LED). Most professional audio equipment like mixers and audio interfaces expect a nominal input line level of +4 dBu.

### Headphone output

There's a separate stereo (TRS) headphone driving output with its own volume control, also with a range of -infinite to +10 dBu.
It can drive headphones with 32ohms or 85ohms with no problem. Higher impedances are also probably fine.

### External instrument inputs

The external inputs can amplify line level signals to the usual Eurorack amplitude of 10 Vpp with the help of a dedicated volume control. The input metering LEDs will turn yellow when the amplified signals at the Euro L and R outputs is between 9 and 11 Vpp, and red when above 11 Vpp.
This pre-amp has been designed with line level signals in mind, like those coming from another synthesizer or professional audio equipment. High impedance instrument outputs like electric guitars might not produce the best sound when connected directly to this module.

## Current consumption

+12V --> 110mA

-12V --> 110mA

## Dimensions

Height: 20cm

Width: 10cm

Depth: 5cm

## PCB set

- Front Panel
- Controls
- LEDs Aligner
- Main
- Mezzanine

## Gerbers

https://github.com/DeMarco/DMH-Output/tree/main/Gerbers

## Schematic and BoM

https://github.com/DeMarco/DMH-Output/blob/main/DMH_Output_Schematic.pdf

https://github.com/DeMarco/DMH-Output/blob/main/DMH_Output_BoM.csv

## Assembly and Calibration Instructions

https://github.com/DeMarco/DMH-Output/blob/main/Assembly_Instructions.md

## Font

For viewing/customizing in KiCad, I recommend downloading and installing the Nulshock font from Typodermic: https://typodermicfonts.com/nulshock/
