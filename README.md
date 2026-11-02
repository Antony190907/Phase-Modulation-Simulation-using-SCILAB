# Phase-Modulation
# EXP NO: 5 PHASE MODULATION using SCILAB

**AIM:**

To write a program for Phase Modulation using SCILAB and to observe and measure the frequency deviation and the modulation index of PM.

**APPARATUS REQUIRED:**

•	Computer with i3 Processor

•	SCI LAB software

**THEORY:**

Phase modulation is a type of modulation in which the phase of the high-frequency (carrier) signal is varied in accordance with the instantaneous value of the modulating signal.

***PHASE DEVIATION Δφ AND MODULATION INDEX mp:***

The phase deviation Δφ represents the maximum shift in the phase of the modulated signal with respect to the phase of the carrier.

We define the modulation index \(m_p\) as the maximum phase deviation.

$$ m_p = \Delta \phi $$

***PHASE MODULATION GENERATION:***

The circuits used to generate phase modulation must vary the phase of a high-frequency signal (carrier) as a function of the amplitude of a low-frequency signal (modulating signal). In practice, phase modulation is generated using a phase modulator circuit.

**ALGORITHM:**

***1. Define Parameters:***

Fs: Sampling frequency.

T: Duration of the signal.

Fc: Carrier frequency.

Fm: Frequency of the modulating signal.

Beta: Modulation index, which controls the extent of phase deviation.

***2. Generate Signals:***

Modulating signal: Sinusoidal signal used for modulation.

Carrier signal: The high-frequency carrier signal.

Modulated signal: PM modulated signal calculated by varying the carrier phase according to the modulating signal.

***3. PM Modulation:***

Modulated signal is obtained by varying the phase of the carrier signal according to the instantaneous amplitude of the modulating signal.

***4. Visualization:***

Plots the modulating signal, carrier signal, and PM modulated signal for analysis.

**PROCEDURE:**

•	Refer Algorithms and write code for the experiment.

•	Open SCILAB in System

•	Type your code in New Editor

•	Save the file

•	Execute the code

•	If any Error, correct it in code and execute again
Verify the generated waveform using Tabulation and Model Waveform

**MODEL GRAPH:**

<img width="550" height="596" alt="image" src="https://github.com/user-attachments/assets/1fb5b08b-7be2-484c-bfa0-65e8f77aa1a9" />



**PROGRAM:**
~~~

Am=2.96;
fm=361;
Ac=1.8*Am;
fc=10*fm;
fs=10*fc;
t=0:1/fs:2/fm;
bp=3.74;
em=Am*cos(2*3.14*fm*t);
ec=Ac*cos(2*3.14*fc*t);
ePM=Ac*cos(2*3.14*fc*t+bp*cos(2*3.14*fm*t));
subplot(3,1,1);
plot(t,em);
subplot(3,1,2);
plot(t,ec);
subplot(3,1,3);
plot(t,ePM);


~~~


**OUTPUT WAVEFORM:**

<img width="1365" height="677" alt="Screenshot 2026-11-02 215131" src="https://github.com/user-attachments/assets/2207a100-e825-451a-abcd-e9360ac3bcdf" />




**TABULATION:**

<img width="3406" height="2002" alt="IMG_20261102_191955_edit_140133076303616 jpg" src="https://github.com/user-attachments/assets/2d51984a-1ce9-4c16-9870-c83c9a70e00f" />



**CALCULATION:**

<img width="2736" height="1024" alt="IMG_20261102_215732_edit_142381959325148 jpg" src="https://github.com/user-attachments/assets/e445ab5f-5bd0-4dfc-89c1-9a22205520ee" />


<img width="2439" height="3240" alt="IMG_20261102_215728_edit_142395208343375 jpg" src="https://github.com/user-attachments/assets/0cc91063-7087-4863-997a-ff15192f906a" />




**RESULT:**

Thus, the Phase modulation is successfully done and the output is experimentally verified.
