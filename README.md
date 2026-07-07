# DMH-Output
Kosmo format output module

<img width="651" height="869" alt="image" src="https://github.com/user-attachments/assets/49cfe7ba-f8a9-4ebc-8888-ad162b3b316b" />

<img width="651" height="869" alt="image" src="https://github.com/user-attachments/assets/359aef5b-c412-4d04-ab10-f7115af3be43" />

<img width="651" height="869" alt="image" src="https://github.com/user-attachments/assets/43efbdd4-0ef6-4521-95e2-ccb7a9f8663e" />


## Features

### Line outputs and and main volume

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

+12V --> 105mA
-12V --> 105mA

## Dimensions

Height: 20cm

Width: 10cm

Depth: 4cm

## PCB set

### Front Panel

<img width="446" height="867" alt="panel" src="https://github.com/user-attachments/assets/764925c6-9d72-4200-b7ff-75c81ad03acf" />

### Controls

<img width="527" height="797" alt="controls_front" src="https://github.com/user-attachments/assets/bed222dd-8213-46e1-926a-9eb5f1b79a4f" />
<img width="485" height="812" alt="controls_back" src="https://github.com/user-attachments/assets/14a6070d-344b-4c20-958c-9a2f34fc222b" />

### LEDs Aligner

<img width="397" height="762" alt="LED_aligner" src="https://github.com/user-attachments/assets/a042b71a-2dc3-42e8-ba62-c84637896d35" />

### Main

<img width="777" height="782" alt="main_front" src="https://github.com/user-attachments/assets/1dea57ee-c1fd-40f8-8990-2a275d378295" />
<img width="500" height="842" alt="main_back" src="https://github.com/user-attachments/assets/67c615bc-0325-43b8-90a8-feeea42efab8" />

### Mezzanine

<img width="597" height="862" alt="mezzanine_front" src="https://github.com/user-attachments/assets/b6178ea6-a4dc-4d31-8eeb-487901b44f70" />
<img width="537" height="840" alt="mezzanine_back" src="https://github.com/user-attachments/assets/63cd2d41-9567-4097-a709-0a4931e2038c" />



Final Gerbers available in "Gerbers" folder


## Font

For viewing/customizing in KiCad, I recommend downloading and installing the Nulshock font from Typodermic: https://typodermicfonts.com/nulshock/
