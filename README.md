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

![WhatsApp Image 2024-12-15 at 22 48 23](https://github.com/user-attachments/assets/cb788f58-3906-4218-a83f-76fedd3c6554)




## Components Used

- **1-Bit DRAM Cell**: A single bit of data is stored in a capacitor, with access controlled by a transistor.
- **Row Decoder**: This decoder selects the row of memory cells based on the input address.
- **Column Decoder**: Selects a specific bit within the row.
- **Refresh Mechanism**: A simple logic circuit that periodically refreshes the data in the capacitors to prevent loss of charge.
 

## How the Design Works

### 1-Bit DRAM Cell

A single DRAM cell consists of:
- A **transistor** that acts as a switch.
- A **capacitor** that holds the bit of data as charge.

![image](https://github.com/user-attachments/assets/ae13091f-ce1b-4e45-91a2-69252ea3c23e)

The transistor is controlled by a row decoder to select which row is being accessed. The column decoder selects the specific bit within the row, allowing for either reading or writing data.

### 8-Bit DRAM Array

The 8-bit DRAM array is formed by connecting eight 1-bit DRAM cells together, forming a row of 8 bits. The row and column decoders are responsible for ensuring that the correct cell is accessed during read and write operations.

### Refresh Mechanism

Due to the nature of DRAM, data is stored in capacitors which tend to leak charge over time. A refresh mechanism is required to periodically recharge the capacitors and prevent data loss. This operation must be done at regular intervals.

## Data Operations

- **Write Operation**: The write operation stores a new bit of data in the selected 1-bit DRAM cell. A high voltage will store a "1", while a low voltage stores a "0".
- **Read Operation**: The read operation reads the stored value from the capacitor. The charge is read via the transistor and output to the data bus.

## Getting Started

Follow the instructions below to simulate and test this DRAM design.

### Prerequisites

- **VLSI Design Tool**: You will need a VLSI design tool that supports circuit-level simulations, such as Cadence Virtuoso, Synopsys, or any other tool that supports DRAM cell simulation.
- **Basic Understanding of DRAM**: Familiarity with how DRAM functions and its components, including row/column decoders, capacitors, and transistors, will help in understanding this design.

### Installing

Clone this repository to get access to the simulation files:

```bash
git clone https://github.com/yourusername/8bit-dram-using-1bit-dram.git
