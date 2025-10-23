# AM-USING-PYTHON-
## Aim
To implement and analyze  modulation (AM) using Python's NumPy and Matplotlib libraries. 

## Apparatus Required

1.	Software: Python with NumPy and Matplotlib libraries
2.	Hardware: Personal Computer
  
## Theory
Modulation can be defined as the process by which the characteristics of carrier wave are varied in accordance with the modulating wave (signal). Modulation is performed in a transmitter by a circuit called a modulator. Need for modulation is as follows: • Avoid mixing of signals • Reduction in antenna height • long distance communication • Multiplexing • Improve the quality of reception • Ease of radiation. Amplitude Modulation is the process of changing the amplitude of a relatively high frequency carrier signal in proportion with the instantaneous value of the modulating signal. The output waveform contains all the frequencies that make up the AM signal and is used to transport the information through the system. Therefore the shape of the modulated wave is called the AM envelope. With no modulating signal the output waveform is simply the carrier signal. Coefficient of modulation is a term used to describe the amount of amplitude change present in an AM waveform. There are three degrees of modulation available based on value of modulation index.

Under modulation : m<1, Em < Ec
Critical modulation: m-1, Em = Ec
Over modulation: m>1, Em > Ec
Note: Keep all the switch faults in off position

## Algorithm


1.	Initialize Parameters: Set the values for carrier frequency, message frequency, sampling frequency, and frequency deviation.
2.	Generate Time Axis: Create a time vector for the signal duration.
3.	Generate Message Signal: Define the message signal as a cosine wave.
4.	Compute the Integral of the Message Signal: Calculate the integral of the message signal over time.
5.	Generate FM Signal: Apply the FM modulation formula to obtain the modulated signal.
6.	Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

## Program

<img width="363" height="452" alt="Screenshot 2025-10-23 203118" src="https://github.com/user-attachments/assets/0f4f5bfe-6b71-4664-9bab-7c08882a18bb" />

## Output Waveform

<img width="748" height="584" alt="Screenshot 2025-10-23 203130" src="https://github.com/user-attachments/assets/136db7d9-5dd5-45ea-9948-79f363cf778c" />

## Tabular Column


## Result
The message signal, carrier signal, and Amplitude modulated (AM) signal will be displayed in separate plots. The modulated signal will show frequency variations corresponding to the amplitude of the message signal.
