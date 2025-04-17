# GNU-Radio-Project
This GNU Radio Companion project demonstrates how a sinusoidal signal can be visualized and understood in time, frequency, and phasor domains. Users can interactively modify the amplitude, frequency, and phase of the signal and observe the real-time effects using QT GUI visualizations.

How to Run
Steps:
Open GNU Radio Companion

Load the .grc file (File > Open)

Click Run

Use the sliders to change:

Amplitude 

Frequency 

Phase 

___________________________________________________________

Visualizations update in real time:

Time Domain: Shows the waveform over time

Frequency Domain: Shows FFT of the signal

Phasor View: Visualizes the path of a signal(dot)

__________________________________________________________________


What It Demonstrates:
How sinusoidal signals behave when parameters like amplitude, frequency, and phase are varied

The relationship between the time-domain waveform and its frequency content as well as its phasor content

_____________________________________________________________________

How it was made:
We start with two signal sources with the real part being cos and imaginary part being sine

The signal sources are connected to a range block for each of amplitude, phase , and freq to allow the user full control of the signals 

The real part is put through a throttle block in order to limit the flow rate to under the sampling rate

The real part connects to a Time Sink GUI to show the amplitude vs time as well as connecting to a Frequency Sink to show the frequency domain

The real and imaginary part combine using a float to complex block in order feed and input to a Constellation Sink which allows us to visualize the path of the pahsor
