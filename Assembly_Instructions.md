# Output Module - Instructions

## Soldering

Always start solder the "shortest" components, and move on to the "taller" ones.

### Main PCB:

Solder these components in the following order:

- Resistors
- Diodes
- IC sockets
- Ceramic capacitors
- Electrolytic capacitors
- Power and IO (IDC type) connectors
- Pin sockets for PCB stacking (use 11mm stackable sockets on J23, J26, J27 and J28)
- TRS jack sockets

Tip: don't forget to soldeer pin sockets J35 and J36 before the TRS jack sockets. This is very hard to rework if not done in this order.

### Mezzanine PCB:

Solder these components in the following order:

- Resistors
- IC sockets
- Ceramic capacitors
- Trimpots
- Electrolytic capacitors
- Pin headers for PCB stacking (use 11mm long pin headers to avoid volume conflicts)



### Controls PCB:

Solder these components in the following order:

- Resistors
- IC sockets
- Ceramic capacitors
- Transistors and LM4040 regulator
- Potentiometers

Once the potentiometers are secured, make use of 2x 5mm standoffs to secure the LED Aligner PCB in place.
The LED Aligner will be flush with the IC sockets, but this is expected. It will be removed later to make space for the ICs.


Insert the LEDs through the holes of the LED Aligner. Make sure the shorter terminals are inserted into the square solder pads on the PCB:


Now, attach the Fronty Panel and secure it in place with the potentiometers' nuts:


Flip the assembly so that gravity pulls the LEDs downwards. Make sure all LEDs are well aligned and flush with the back of the Front Panel:
(don't forget the 3-pin LEDs D31 and D32, which are missing in the picture!!)


Solder all LED terminals and trim the excess, then remove the LED Alginer PCB and the standoffs.

Now finish the Controls PCB by soldering the pin sockets for PCB stacking.


## Voltage Supply Testing

Without inserting the ICs in their sockets, stack all PCBs together.
Tip: If necessary, "thicken" the pins of the stacking sockets with a bit of solder, in case you suspect they are not making contact.
Set your multimeter in continuinity test mode.
Make sure all TRS jack socket barrels are well connected to GND.
Tip: Pad J0 close to C1 on the Main PCB can be used as a helpful GND terminal for any measurements.
Connect the power cable to J100 and switch on your power supply.
Make sure there's no magic smoke nor excessive heat coming from any component.
Use a multimeter to check if +12V and -12V supply voltages are correct on the IC sockets.
Tip: Temporarily unstack the Mezzanine PCB to allow measuring on the Main PCB IC sockets.
Measure also the +10V reference voltage on the top terminal of C42 on the Controls PCB.


## Final Assembly

Power off the module.
Insert all ICs in their respective sockets.
Tip: Make sure to align the IC and socket grooves to avoid frying your precious chips.
Power the module back on.
Position the LED Aligner PCB on top of the ICs on the Controls PCB. No need to secure it with standoffs.
The Aligner should be flush with both the ICs and LEDs top surfaces. This will help reducing light bleeding from one LED to the other.
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

Repeat the procedure for the Right channel by using In R, TP23, TP24 and RV5.


## Configuration

Connector J200 can be used to make the module's IO available at another PCB for internal "normalling" with other modules, like in a semimodular synthesizer.
When J200 is not in use, pins 1 and 6 can be joined together (with a jumper). This will "stereophy" a mono signal plugged to In L when In R is not in use.
The same can be done with pins 2 and 5 in order to "stereophy" a mono signal from an external instrument at the Euro L/R outputs.















