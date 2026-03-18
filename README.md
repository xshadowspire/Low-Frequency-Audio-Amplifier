Low-Frequency Audio Amplifier (AAF/AJF)
Project Overview
This project consists of the complete design, dimensioning, and simulation of a low-frequency voltage amplifier (20 Hz - 20 kHz). Developed as part of the Fundamental Electronic Circuits 2 course at National University of Science and Technology POLITEHNICA Bucharest, the design is inspired by the internal architecture of the BA4558 operational amplifier.

Technical Specifications
The amplifier was designed to meet the following parameters:
Voltage Gain:10
Input Signal:1020mV
Output Load 170 ohm
Input Resistance >150kohm
Output Resistance < 2.8Oohm
Operating Temperature range 0-70 celsius degrees

Circuit Architecture
The circuit is divided into three specialized functional stages to balance gain, impedance matching, and current drive:
Input Stage: A differential amplifier utilizing PNP bipolar transistors (QBC856B) to achieve high input impedance. It includes a current mirror (QBC846B) for improved stability and signal-to-noise ratio.

Gain Stage: Composed of a Common Emitter configuration for voltage amplification and a Common Collector stage acting as a buffer to transition to the low impedance of the output.

Output Stage: A Class B push-pull configuration using complementary transistors (BC807/BC817). These were selected for their ability to manage output currents of approximately 60 mA and superior thermal characteristics.

Key Design Features:
Negative Feedback: A global negative feedback network is employed to stabilize the gain and reduce distortions, making the amplification factor dependent on passive components rather than transistor variations.
Frequency Response: Controlled by an input high-pass filter and an output low-pass filter to cover the 20 Hz - 20 kHz audio band precisely.
Phase Compensation: A Miller capacitor (C5) is integrated to provide phase compensation, preventing unwanted oscillations and ensuring circuit stability at high frequencies.

Simulation and Validation
The design was validated using the OrCAD/PSpice environment:
Transient Analysis: Confirmed an undistorted harmonic output of 10.2V with a 1020mV input signal.AC Sweep: Verified the 20 Hz to 20 kHz frequency response with a 3dB attenuation at the band edges.Temperature Stability: Simulations at 9,20,70 degrees celsius showed no significant variations in the output waveform, confirming a robust and reliable design.


