# Frequency Modulation

EXP NO: 4 Frequency Modulation

Aim:- To simulate frequency modulation and demodulation to verify modulation index and bandwidth using SCILAB.

Equation Used:-
1. em = Am cos (2πfmt)
2. ec = Ac cos (2πfct)
3. efm = Ac cos (ωct + β sin ωmt)


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
MODEL GRAPH
 <img width="919" height="1290" alt="image" src="https://github.com/user-attachments/assets/55326c5b-7dd5-4873-aaf6-d219bb7c4420" />
 TABULATION:
<img width="637" height="332" alt="image" src="https://github.com/user-attachments/assets/7ff79056-9cf7-4ff0-a385-703060457972" />
Calculation
<img width="648" height="362" alt="image" src="https://github.com/user-attachments/assets/07db08ba-635e-410e-914a-efc758fa6b82" />

Output Waveform
<img width="760" height="580" alt="image" src="https://github.com/user-attachments/assets/3efbd926-dbb4-4692-9040-b72d6a7faf32" />

RESULT:
Thus the amplitude modulation and demodulation is experimentally done and the output is verified.
