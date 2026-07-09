# Output Module - Instructions

## Schematic and BoM

https://github.com/DeMarco/DMH-Output/blob/main/DMH_Output_Schematic.pdf

https://github.com/DeMarco/DMH-Output/blob/main/DMH_Output_BoM.csv


## Soldering

### Main PCB:

Solder these components in the following order:

- Resistors
- Diodes
- IC sockets
- Ceramic capacitors
- Electrolytic capacitors
- Power (J100) and IO (J200) connectors
- Pin sockets for PCB stacking (use 11mm stackable sockets on J23, J26, J27 and J28)
- TRS jack sockets

*__Tip:__* don't forget to solder pin sockets J35 and J36 before the TRS jack sockets. This is very hard to rework if not done in this order.

<img width="777" height="782" alt="main_front" src="https://github.com/user-attachments/assets/1dea57ee-c1fd-40f8-8990-2a275d378295" />
<img width="500" height="842" alt="main_back" src="https://github.com/user-attachments/assets/67c615bc-0325-43b8-90a8-feeea42efab8" />



### Mezzanine PCB:

Solder these components in the following order:

- Resistors
- IC sockets
- Ceramic capacitors
- Trimpots
- Electrolytic capacitors
- Pin headers for PCB stacking (use 11mm long pin headers to avoid volume conflicts)

<img width="597" height="862" alt="mezzanine_front" src="https://github.com/user-attachments/assets/b6178ea6-a4dc-4d31-8eeb-487901b44f70" />
<img width="537" height="840" alt="mezzanine_back" src="https://github.com/user-attachments/assets/63cd2d41-9567-4097-a709-0a4931e2038c" />



### Controls PCB:

Solder these components in the following order:

- Resistors
- IC sockets
- Ceramic capacitors
- Transistors and LM4040 regulator
- Potentiometers
- _Don't solder the LEDs and pin sockets yet_

<img width="527" height="797" alt="controls_front" src="https://github.com/user-attachments/assets/bed222dd-8213-46e1-926a-9eb5f1b79a4f" />



Once the potentiometers are secured, make use of 2x 5mm standoffs to secure the LED Aligner PCB in place.
The LED Aligner will be flush with the IC sockets, but this is expected. It will be removed later to make space for the ICs.

<img width="476" height="805" alt="image" src="https://github.com/user-attachments/assets/b02a6060-42a5-41a8-a78e-c41ac3505fbe" />
<img width="663" height="746" alt="image" src="https://github.com/user-attachments/assets/641aee41-b112-40e1-839f-df04d91acc68" />



Insert the LEDs through the holes of the LED Aligner. Make sure the shorter terminals are inserted into the square solder pads on the PCB:

<img width="721" height="765" alt="image" src="https://github.com/user-attachments/assets/de1d0695-4101-4f19-8545-42c15ff4d60f" />



Now, attach the Front Panel and secure it in place with the potentiometers' nuts:

<img width="508" height="690" alt="image" src="https://github.com/user-attachments/assets/65282b7a-109e-4d27-9566-95cef119d052" />



Flip the assembly so that gravity pulls the LEDs downwards. Make sure all LEDs are well aligned and flush with the back of the Front Panel:
(don't forget the 3-pin LEDs D31 and D32, which are missing in the picture!!)

<img width="754" height="505" alt="image" src="https://github.com/user-attachments/assets/5616cb07-ddfd-463e-a632-98cadaa4608f" />



Solder all LED terminals and unscrew the Front Panel. This should be the result:

<img width="607" height="922" alt="image" src="https://github.com/user-attachments/assets/5792c5ba-08c2-4019-b393-3c11679a7cb8" />



Remove the LED Alginer PCB and the standoffs.

Now finish the Controls PCB by soldering the pin sockets for PCB stacking.

<img width="485" height="812" alt="controls_back" src="https://github.com/user-attachments/assets/14a6070d-344b-4c20-958c-9a2f34fc222b" />




## Voltage Supply Testing

Without inserting the ICs in their sockets, stack all PCBs together.

*__Tip:__* If necessary, "thicken" the pins of the stacking sockets with a bit of solder, in case you suspect they are not making contact.

<img width="855" height="706" alt="image" src="https://github.com/user-attachments/assets/154058a8-0baf-4275-8f00-825856a485f8" />


Set your multimeter in continuinity test mode.

Make sure all TRS jack socket barrels are well connected to GND.

*__Tip:__* Pad J0 close to C1 on the Main PCB can be used as a helpful GND terminal for any measurements.

<img width="655" height="497" alt="image" src="https://github.com/user-attachments/assets/e8eb363c-12d9-4555-a2a5-236b26d06e1c" />


Connect the power cable to J100 and switch on your power supply.

Make sure there's no magic smoke nor excessive heat coming from any component.

Use a multimeter to check if +12V and -12V supply voltages are correct on the IC sockets.

*__Tip:__* Temporarily unstack the Mezzanine PCB to allow measuring on the Main PCB IC sockets.

Measure also the +10V reference voltage on the top terminal of C42 on the Controls PCB.

<img width="655" height="497" alt="image" src="https://github.com/user-attachments/assets/2442f8a7-b35d-4076-a15c-300f38722ced" />



## Final Assembly

Power off the module.

Insert all ICs in their respective sockets.

*__Tip:__* Make sure to align the IC and socket grooves to avoid frying your precious chips.

Power the module back on.

Position the LED Aligner PCB on top of the ICs on the Controls PCB. No need to secure it with standoffs.

The Aligner should be flush with both the ICs and LEDs top surfaces. This will help reducing light bleeding from one LED to the other.

<img width="343" height="729" alt="image" src="https://github.com/user-attachments/assets/2d626f79-a42e-4f77-bc5a-1dfa4b1d7980" />


Finally, put the Front Panel in place and secure it agains the pots and TRS sockets with their respective washers and nuts.

Mount the knob covers. The module is now ready for calibration.


## Calibration

Power the module again, still on your bench.

Set all 3 knobs to the max (fully clockwise).

Check that the current consumption indicated by your power supply is about 110mA for both the +12V and -12V supply voltages.

Plug a realiable sawtooth wave signal to In L (like from a VCO). 

Make sure both channels 1 and 2 of your oscilloscope are centered on the 0V.

Attach channels 1 and 2 of the oscilloscope to test points TP21 and T22 respectively.

Adjust the oscilloscope for amplitude and frequency.

A 10Vpp sawtooth input signal (like that coming from a VCO) should result in a 7Vpp signal (thus +/-3.5V) at TP21. An inverted sawtooth signal of same amplitude should appear at TP22.

Adjust trimpot RV4 until both signals are "perfectly" centered around the 0V line.

<img width="1029" height="498" alt="image" src="https://github.com/user-attachments/assets/b5afa373-3085-477f-b15d-29f6084618c8" />


Repeat the procedure for the Right channel by using In R, TP23, TP24 and RV5.

<img width="426" height="602" alt="image" src="https://github.com/user-attachments/assets/190100e7-cb5b-43cf-b247-b626a3e26e61" />


## Configuration

Connector J200 can be used to make the module's IO available at another PCB for internal "normalling" with other modules, like in a semimodular synthesizer.

When J200 is not in use, pins 1 and 6 can be joined together (with a jumper). This will "stereofy" a mono signal plugged to In L when In R is not in use.

The same can be done with pins 2 and 7 in order to "stereofy" a mono signal from an external instrument at the Euro L/R outputs.

<img width="582" height="501" alt="image" src="https://github.com/user-attachments/assets/2ee58092-84d6-4305-9a1e-d8eef4377a37" />














