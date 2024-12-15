##8-Bit DRAM Design Using Cadence Virtuoso

#Project Overview

This project focuses on designing, simulating, and verifying an 8-bit DRAM module using Cadence Virtuoso. The DRAM architecture is built from a single 1-bit memory cell, scaled to an 8-bit array for parallel read/write operations. The project showcases the use of 180nm CMOS technology, simulates DRAM read and write functionality, and ensures the reliability of data storage through retention tests.

#Features

1-bit DRAM Cell Design: Based on an access transistor and a storage capacitor.
8-bit DRAM Array: Combines individual 1-bit cells into a functional array with shared wordlines.
#Functionality:
Read/Write operations.
Refresh and retention simulations.
Technology: 180nm CMOS library.
#Tools:
Schematic and layout design using Cadence Virtuoso.
Circuit simulation using Spectre.
Verification of layout design (DRC, LVS).

#Tools and Environment
Cadence Virtuoso: Schematic design, layout creation, and netlist generation.
Spectre: Simulation of DRAM functionality and transient behavior.
Assura or Calibre: Design Rule Check (DRC) and Layout Versus Schematic (LVS) verification.
Linux/UNIX: Recommended operating system for running Cadence.
Technology: 180nm PDK for component modeling.
Design Description

##1. 1-Bit DRAM Cell
#Components:
Access Transistor: Connects the storage capacitor to the bitline when the wordline is activated.
Storage Capacitor: Holds the charge representing the memory bit (1 or 0).
Connections:
Wordline (WL): Activates the cell for read/write.
Bitline (BL): Facilitates data transfer.
VDD: Supplies the voltage for operation.
#2. 8-Bit DRAM Array
Composed of 8 DRAM cells arranged in a single row.
Shared wordline (WL) for row access.
Individual bitlines (BL1–BL8) for each cell to enable parallel data operations.
