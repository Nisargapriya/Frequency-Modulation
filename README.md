# Frequency Modulation

EXP NO: 4 Frequency Modulation

Aim:- To simulate frequency modulation and demodulation to verify modulation index and bandwidth using SCILAB.

Equation Used:-
1. em = Am cos (2πfmt)
2. ec = Ac cos (2πfct)
3. efm = Ac cos (ωct + β sin ωmt)

THEORY:

Frequency Modulation (FM) is a type of angle modulation in which the frequency of the carrier signal is varied in accordance with the instantaneous amplitude of the modulating signal while the amplitude of the carrier remains constant.

In FM, the frequency deviation of the carrier is directly proportional to the amplitude of the message signal. Frequency modulation provides better noise immunity and improved signal quality compared to amplitude modulation.

The message signal is given by:

em = Am cos(2πfmt)

The carrier signal is given by:

ec = Ac cos(2πfct)

The frequency modulated signal is given by:

efm = Ac cos(2πfct + β sin(2πfmt))

where,

Am = Amplitude of the message signal
Ac = Amplitude of the carrier signal
fm = Frequency of the message signal
fc = Frequency of the carrier signal
β = Modulation index

The modulation index is defined as:

β = Δf / fm

where,

Δf = Frequency deviation
fm = Modulating frequency

Thus, in Frequency Modulation, the instantaneous frequency of the carrier varies according to the message signal while its amplitude remains constant.

Algorithm

1. Start the program.
2. Define Am, Ac, fm, fc, fs, and modulation index β.
3. Generate the time vector.
4. Generate the message signal.
5. Generate the carrier signal.
6. Generate the FM signal using the frequency modulation equation.
7. Plot the message, carrier, and FM signals.
8. Observe the waveforms.
9. Stop the program.
Program
```
Am=10.85;
fm=1584;
fc=15840;
fs=158400;
Ac=16.275;
b=2.7;
t=0:1/fs:2/fm;

em=Am*cos(2*3.14*fm*t);
subplot(3,1,1);
plot(t,em);

ec=Ac*cos(2*3.14*fc*t);
subplot(3,1,2);
plot(t,ec);

efm=Ac*cos(2*3.14*fc*t+b*sin(2*3.14*fm*t));
subplot(3,1,3);
plot(t,efm);


```
TABULATION:

<img width="590" height="322" alt="image" src="https://github.com/user-attachments/assets/02c1f40e-c492-438c-85db-04082328dbaf" />

Calculation:

<img width="339" height="166" alt="image" src="https://github.com/user-attachments/assets/259da0b3-c24b-49d1-af44-664ff6bd7340" />

Output Waveform:

<img width="753" height="692" alt="image" src="https://github.com/user-attachments/assets/3db1a762-6e14-4c45-bacd-f7b75e111707" />

RESULT:
Thus, the Frequency Modulation (FM) signal is generated using SCILAB/MATLAB and the corresponding output waveforms are obtained and verified.
