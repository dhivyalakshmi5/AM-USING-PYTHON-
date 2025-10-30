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
```
import numpy as np
import matplotlib.pyplot as plt
Am=3.2
fm=283
fs=28300
Ac=6.4
fc=2830
t=np.arange(0,2/fm,1/fs)
m=Am*np.cos(2*np.pi*fm*t)
plt.subplot(3,1,1)
plt.plot(t,m)
c=Ac*np.cos(2*np.pi*fc*t)
plt.subplot(3,1,2)
plt.plot(t,c)
s=(Ac+m)*np.cos(2*3.14*fc*t)
plt.subplot(3,1,3)
plt.plot(t,s)
plt.tight_layout()
plt.show()
```
## Output Waveform
<img width="826" height="602" alt="Screenshot 2025-10-28 173256" src="https://github.com/user-attachments/assets/4a200c9e-6518-4753-9447-43f404a6d639" />

## Tabular Column
![WhatsApp Image 2025-10-30 at 10 20 09_84abdf75](https://github.com/user-attachments/assets/3ee7964e-1f72-4072-b34f-4ff62f3ba5ce)
## Calculation
![WhatsApp Image 2025-10-30 at 10 20 23_c412eab5](https://github.com/user-attachments/assets/7c558318-4c05-4578-9815-a7c40c8ebb96)


## Result
The message signal, carrier signal, and Amplitude modulated (AM) signal will be displayed in separate plots. The modulated signal will show frequency variations corresponding to the amplitude of the message signal.
