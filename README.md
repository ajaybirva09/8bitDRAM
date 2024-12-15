  # 8-Bit DRAM Design Using 1-Bit DRAM Cells

This project demonstrates the design and layout of an 8-bit DRAM array using 1-bit DRAM cells created in **Cadence Virtuoso**. The goal of this project is to implement a simple, but scalable memory design that can be expanded and adapted for various memory applications.

## Project Overview

The **1-bit DRAM cell** is the basic building block of the **8-bit DRAM array**. The design consists of two main components:

1. **1-bit DRAM Cell**: This cell stores a single bit of data and consists of two inverters, access transistors, and a capacitor for data storage.
2. **8-bit DRAM Array**: A collection of 8 of the 1-bit DRAM cells arranged in a matrix configuration. This design uses wordline and bitline decoding to allow selective access to each bit in the array.

### Key Features:
- **1-bit DRAM cell design** that can be scaled to larger arrays.
- **Array architecture** for accessing multiple bits of data at once.
- **Cadence Virtuoso** used for schematic capture, layout design, and simulation.
- **Design Rule Check (DRC)** and **Layout vs. Schematic (LVS)** were performed to ensure correctness.

## Project Structure

The project is organized into the following directories:

- **`schematics/`**: Contains the schematic files for the 1-bit DRAM cell and the 8-bit DRAM array.
  - `1bit_dram_cell.sch`: Schematic for the 1-bit DRAM cell.
  - `8bit_dram_array.sch`: Schematic for the 8-bit DRAM array.
  
- **`layouts/`**: Contains the layout files for the 1-bit DRAM cell and the 8-bit DRAM array.
  - `1bit_dram_cell.lyt`: Layout for the 1-bit DRAM cell.
  - `8bit_dram_array.lyt`: Layout for the 8-bit DRAM array.
  
- **`documentation/`**: Contains project documentation and design notes.
  - `design_notes.txt`: A text file outlining design decisions, challenges, and solutions.
  
- **`README.md`**: This file, containing an overview of the project, structure, and instructions.

## Instructions

### 1. Schematic Design:
- Open the schematic files (`1bit_dram_cell.sch` and `8bit_dram_array.sch`) in **Cadence Virtuoso**.
- Review the connections and ensure that the 1-bit DRAM cell operates correctly.
  
### 2. Layout Design:
- Open the layout files (`1bit_dram_cell.lyt` and `8bit_dram_array.lyt`) in **Cadence Virtuoso**.
- Check the layout and ensure all components are correctly placed and routed.
  
### 3. Run DRC and LVS:
- Run **Design Rule Check (DRC)** to ensure that the layout adheres to the design rules.
- Run **Layout vs. Schematic (LVS)** to verify that the layout matches the schematic.

### 4. Simulation:
- Perform **functional simulation** to verify the operation of the 1-bit DRAM cell and 8-bit DRAM array.
- Simulate read/write operations, and check for data integrity.

## Tools Used

- **Cadence Virtuoso**: For schematic capture, layout design, and simulation.
- **DRC (Design Rule Check)**: To ensure the layout adheres to design rules.
- **LVS (Layout vs. Schematic)**: To check that the layout matches the schematic.

## Future Improvements

- **Scaling**: The design can be extended to larger DRAM arrays, such as 16-bit, 32-bit, or even larger.
- **Optimization**: Future work could focus on optimizing the area and power consumption of the DRAM array.
- **Performance**: Add control logic for efficient read and write cycles.

## License

This project is open source. You can freely use, modify, and distribute it under the MIT license.

