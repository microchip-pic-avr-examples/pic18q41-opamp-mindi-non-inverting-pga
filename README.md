# Getting started with Mindi® simulation and PIC18-Q41 microcontrollers
This guide will get you up and running with simulating the analog OPAMP module in PIC18-Q41 family devices using the Mindi simulation tool.
## Configuration: Non-Inverting Programmable Gain Amplifier (PGA)
The Non-Inverting Programmable Gain Amplifier is a configuration with run-time selectable positive gain.

![Non-Inverting PGA](images/configuration.png)

![Non-Inverting PGA Equation](images/non-inverting-gain.PNG)

### Mindi Simulation
![Mindi](images/mplab-mindi-analog-simulator.png)

Download and open the follower **Mindi schematic [here](schematics/Non_inverting_PGA.wxsch)**

Press the _play_ button to simulate with an example stimulus source.

### Tweaking
The amplification of the Non-Inverting PGA can be adjusted to any of 8 levels from 1.06 to 16 by changing the MUXWIP value in the control register. The Mindi schematic contains a table detailing the levels of gain and their associated register and resistor values.

### Updating composer fields
Once the desired result has been verified with Mindi simulation, the corrected values should be moved back into MCC/Start by copying resistor values across to the composer of your preference.

### Don't have Mindi?
Download and install [Mindi simulation tool](https://www.microchip.com/mplab/mplab-mindi)
Download and install Mindi model for AVR DB device
