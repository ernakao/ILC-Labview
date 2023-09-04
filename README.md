# ILC-Labview
Iterative Learning Control on Labview for the Quanser srv02 motor

## ILC Algorithm
![image](https://github.com/ernakao/ILC-Labview/assets/109694851/cccd294f-d1c3-4ea0-89b4-f776862ef3c9)

with m = 2, instead of the usual m = 1

## ILC Architecture
The architecture used was the parallel architecture

![image](https://github.com/ernakao/ILC-Labview/assets/109694851/ee1af36f-4b81-446d-8366-dd102a58c96c)

(Image from Bristow, Tharayil and Alleyne(2006))

## How it works
The "gerador_sine_wave.vi" creates the signal for the motor to follow (y_d), being just an auxiliary program. After the initial run on the auxiliary program, the main program (ILC_Final.vi) runs the ILC control on the system given the number of runs and the proporcional value of the feedback controller (used to stabilize the plant)

A more detailed explanation on the ILC method itself and the project can be found on TCC.pdf (in portuguese), mainly on chapters 3 (introduction to the ILC method) and chapter 5 (running the program on the quanser srv02 motor)
