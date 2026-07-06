# DMH-Output
Kosmo format output module

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
