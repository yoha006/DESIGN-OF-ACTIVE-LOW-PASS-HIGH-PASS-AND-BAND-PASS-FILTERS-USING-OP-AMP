# DESIGN-OF-ACTIVE-LOW-PASS-HIGH-PASS-AND-BAND-PASS-FILTERS-USING-OP-AMP
## AIM: 	
To design and obtain the frequency response of
i)	First order Low Pass Filter (LPF)
ii)	First order High Pass Filter (HPF)
iii)	Band pass filter

## APPARATUS REQUIRED:  
<img width="653" height="177" alt="image" src="https://github.com/user-attachments/assets/707b4cca-e253-4b36-8951-e688e1450abf" />

## THEORY:
## LOW PASS FILTER
A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB frequency, break frequency, or corner frequency.

## CIRCUIT DIAGRAM:
## LOW PASS FILTER
<img width="547" height="310" alt="image" src="https://github.com/user-attachments/assets/d2b52f47-02d3-4683-99b3-71be13b4dced" />

## MODEL GRAPH: LOW PASS FILTER
 <img width="602" height="346" alt="image" src="https://github.com/user-attachments/assets/db9d11c7-e823-46f2-bb3e-635a71cbd0b2" />

## TABULATION: LOW PASS FILTER
![IMG-20251114-WA0005](https://github.com/user-attachments/assets/4716959d-22d5-45a1-8938-8101ed56ff50)
                                                                               		
## GRAPH: LOW PASS FILTER
![IMG-20251114-WA0006](https://github.com/user-attachments/assets/a86e7c77-2b54-4e80-9d0e-bf263124f529)

## HIGH PASS FILTER
The frequency at which the magnitude of the gain is 0.707 times the maximum value of gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band frequencies with the highest frequency determined by the closed –loop band width all of the op-amp.

## CIRCUIT DIAGRAM:
HIGH PASS FILTER
<img width="587" height="314" alt="image" src="https://github.com/user-attachments/assets/219176d8-9b2c-4fa1-bc87-fa84bfaf6f91" />

## MODEL GRAPH: HIGH PASS FILTER
<img width="1007" height="488" alt="image" src="https://github.com/user-attachments/assets/ebcb29eb-14e0-4a94-99c6-8962f80db50c" />

## TABULATION: HIGH PASS FILTER
![IMG-20251114-WA0008](https://github.com/user-attachments/assets/ad757d88-b023-4d14-bab9-98ece8d3cdc0)

## GRAPH: HIGH PASS FILTER
![IMG-20251114-WA0007](https://github.com/user-attachments/assets/f69ba1c6-afb3-4f11-a3d7-219d4e59ed01)

## DESIGN:LPF & HPF
Given: fH = 1 KHz = 1/ (2πRC)

   Let C = 0.1 µF, R = 1.6 KΩ

   For n = 2, α (damping factor) = 1.414,

   Passband gain = Ao = 3 - α =3 – 1.414 = 1.586.

   Transfer function of second order butterworth LPF as:
1.586
H(s) = ---------------------------
S2 + 1.414 s + 1

                Now	  Ao = 1 + (Rf / R1) = 1.586 = 1 + 0.586

                 Let Ri = 10 KΩ, then Rf = 5.86 KΩ

## BAND PASS FILTER
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM:
## BANDPASS FILTER
<img width="1068" height="446" alt="image" src="https://github.com/user-attachments/assets/8f060ede-0036-4055-98d8-f1ca4fd8221f" />
 
## MODEL GRAPH: BANDPASS FILTER
<img width="1058" height="537" alt="image" src="https://github.com/user-attachments/assets/46f7ef48-e8af-437c-958f-680c32873aaa" />

 ## TABULATION: BANDPASS FILTER
![IMG-20251114-WA0010](https://github.com/user-attachments/assets/35d4dcbc-1408-4b68-b894-6360ffc7b7be)

## GRAPH: BANDPASS FILTER
   ![IMG-20251114-WA0009](https://github.com/user-attachments/assets/14853445-7789-4b86-af9b-927cb918bf21)
                                                                                               
## DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4. 
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency of HPF as fL = 1 KHz. 
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf. 
Let C = 0.1μf. 
3. Calculate R from the expression. 
Given: fH = 2KHz  = 1/ (2πR1C1)
   Let C1 = 0.1 µF, R1 = 7.9 KΩ
Given: fL = 400Hz  = 1/ (2πR2C2)
   Let C2 = 0.1 µF, R2 = 39.8 KΩ
  Pass band Gain=4
   Now	  Ao = 1 + (Rf / R1) 
               2-1=(Rf / Ri)
                Ri = Rf
                 Let  Ri = Rf = 10 KΩ

## PROCEDURE - (LPF & HPF):
1. Connect the circuit as shown in the circuit diagram.
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. select the value of R1 & Rf depending on desired passband gain Af..
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp.
4. Tabulate the output voltage Vo with respect to different values of input frequency.
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the graph to  get approximately the same characteristic as shown in the model graph.

## PROCEDURE:BAND PASS FILTER
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given frequencies.
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF followed by a LPF (i.e) HPF in series with LPF.
3. Connect the circuit as shown in the circuit diagram.
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp.
5. Tabulate the output voltage Vo with respect to different values of input frequency.
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the graph to get approximately the same characteristic as shown in the model graph.

## RESULT:
Thus, an active low pass, high pass and band pass filter are designed and tested using Op-Amp IC741
