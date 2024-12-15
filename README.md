* 1-bit DRAM cell with write and read functionality

* Power supply
VDD Vdd 0 DC 3.3V

* Wordline control
VWL WL 0 PULSE(0 3.3V 0 1ns 1ns 10ns 20ns) 

* Bitline driver
VBIT BL 0 DC 0

* Access transistor
M1 BL Storage WL Vdd PMOS W=0.18u L=0.18u 

* Storage capacitor (represents memory cell)
C1 Storage 0 30f

* Load resistor to simulate read operation
Rload BL 0 1k

* Transistor model
.MODEL PMOS PMOS LEVEL=3

* Simulation control
.TRAN 0.1ns 100ns
.END
