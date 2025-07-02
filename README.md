# 4T-Pixel-LTSpice

Photodiode Simulation:


 I1 simulates the photocurrent (Id), representing light intensity.


The 1pF capacitor and large resistor (1Mohm) simulate the parasitic capacitance and leakage path.


Transfer Gate (TX):


V2 generates a PULSE that controls the gate of M3, which acts as the transfer gate (TX).


When TX is ON, charge from the photodiode node is transferred to the floating diffusion node.


Reset Transistor (RST):


M2 is the reset transistor, resetting the FD node to VDD, whenVS2is high.


Controlled by a pulse signal through the gate of M2.


Floating Diffusion Node (FD):


The node labeled vg (between M3 and M2) serves as the FD node, which holds charge transferred from the photodiode.


Source Follower (SF):


M1 is  a common source follower (buffer), reading out the voltage from the FD node (vg).


Vout is connected at the source of M1.


Row Select (SEL):


M4 acts as the row select transistor, controlled by rsel=V3 (another pulse).


It connects the source follower output to the column line.







