# 8-Bit DRAM using 1-Bit DRAM Cells

This project demonstrates the design of an 8-bit DRAM (Dynamic Random Access Memory) system using 1-bit DRAM cells. The 8-bit DRAM array is constructed by expanding the basic 1-bit DRAM cell to store an entire 8-bit word. Each memory cell consists of a transistor and a capacitor to store individual bits, and the array utilizes row and column decoders to access the data.

## Project Overview

This design simulates the basic architecture of a DRAM system where the memory is organized as a matrix of rows and columns. The goal is to design and simulate the functionality of an 8-bit memory block using individual 1-bit DRAM cells. The main components include:

- **1-bit DRAM Cell**: Each memory cell stores one bit of data using a transistor and a capacitor.
- **8-bit DRAM Array**: An array of 8 1-bit DRAM cells, forming an 8-bit memory word.
- **Row/Column Decoding**: A mechanism for selecting a specific bit in the memory matrix using row and column address decoding.
- **Refresh Circuit**: DRAM cells require periodic refreshing to maintain their data integrity due to charge leakage from the capacitors.

## Features

- **Basic 1-bit DRAM Cell**: Each cell is implemented with a transistor and a capacitor to store one bit of data.
- **8-bit Memory Array**: The design uses eight 1-bit cells to represent an 8-bit word.
- **Read/Write Operations**: Allows basic read and write operations to interact with the memory.
- **Refresh Mechanism**: Ensures that the data in the cells is maintained over time by periodically refreshing the charge in the capacitors.
- **Address Decoding**: Uses row and column decoders to access specific memory locations.

## Block Diagram

The following block diagram illustrates the key components of the design:

