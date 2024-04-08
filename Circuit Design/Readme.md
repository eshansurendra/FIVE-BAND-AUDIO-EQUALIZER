# Five-Band Equalizer Circuit Implementation

## Overview
This project involves the design and implementation of a five-band equalizer circuit using various electronic components such as operational amplifiers (Op-Amps), resistors, capacitors, and Integrated Circuits (ICs). The equalizer circuit aims to adjust the audio signals' frequency response across five different bands, allowing for customized audio output.

## Circuit Components
### Buffer Circuit
- Utilizes Op-Amp follower configuration for impedance matching and circuit isolation.
- High input impedance and low output impedance ensure signal fidelity and compatibility with subsequent circuits.

### Differential Amplifier
- Suppresses common-mode noise in the audio signal.
- Differential noise and common-mode noise are attenuated using Op-Amps, improving signal quality.

### Band Pass Filters (BPF)
- Active BPFs are used to isolate specific frequency bands.
- Advantages over passive filters include better responsivity, no resonance issues, voltage regulation capability, and reliable operation.
- Two active BPF designs (Multiple Feedback and Sallen-Key) are employed for filter implementation.

### Amplifier for Gain Adjustment
- Each band of the input signal is amplified individually, with gain adjustable from 0 to 10.
- Variable resistor values are adjusted to control the gain of each amplifier stage.

### Variable Scaling Adder Circuit
- Combines the outputs of the five filtered bands to produce a scaled sum.
- Enables volume control functionality for the equalizer system.

### LM3914 IC Visualized Audio Level Display
- Used to measure and display the audio signal level.
- Drives LEDs in a logarithmic manner based on the input signal level.
- Supply voltage range: 3 to 25 volts.

## Circuit Design Considerations
- TL072CP IC selected for filters and differential amplifier due to its high slew rate, low noise, and wide power supply range.
- NE5532P IC used for amplifiers due to its high slew rate and wide power supply range.

## System Model and Design Parameters
- TL072CP IC configured as a non-inverting amplifier for high-pass filter input.
- Gain calculated based on resistor values in the feedback loop.
- Multiple feedback BPF topology employed for bandpass filter design.
- Transfer functions and equations used to determine resistor and capacitor values for filter circuits.


