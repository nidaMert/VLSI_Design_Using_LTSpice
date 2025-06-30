# 🧠 VLSI Design Using LTspice

This repository contains LTspice-based circuit designs and simulation projects developed as part of the **VLSI (Very Large Scale Integration)** course. The projects range from basic logic gate implementations to more complex structures such as SRAM memory cells.

## 📁 Project Descriptions

- **8x8_SRAM_Array – Memory Array Design:**  
  This project involves the design and simulation of a fully functional 8x8 SRAM memory matrix in LTspice, starting from the fundamental 6T SRAM cell. The design includes essential components of SRAM architecture, such as 6T memory cells, pre-charge circuits, write drivers, sense amplifiers, and a 3-to-8 row decoder integrated into a complete system.

  Each cell follows a 6-transistor structure (cross-coupled inverter + access switches), and proper transistor sizing was applied to ensure read/write stability. Sense amplifier blocks were used to convert small voltage differences into full CMOS logic levels quickly and reliably. The row decoder was implemented with a 3-bit input and 8 output lines corresponding to the word lines.

  An 8x8 cell matrix was created, where word lines run horizontally and complementary bitlines (BL/BLB) run vertically. One sense amplifier was assigned to each column. Read and write operations were performed using timing-controlled signals (Write, PC, SE), and system-level correctness was verified through simulation outputs Q[63:0].

- **4_Bit_Radix_4_Booth_Multiplier – Booth Multiplication Algorithm:**  
  This project focuses on designing a multiplier circuit based on the Radix-4 Booth algorithm for signed 4-bit numbers. The system includes key modules such as multiplicand multiple generation (±A, ±2A), Booth encoders, partial product selectors, a shifter block, and a final adder. Each module was implemented at the gate level in LTspice and tested under various input conditions.

- **4_Bit_CLA – 4-Bit Carry Lookahead Adder Design:**  
  This project implements a 4-bit Carry Lookahead Adder (CLA) to perform fast binary addition. Compared to a traditional ripple carry adder, this design significantly reduces propagation delay. The circuit was built and simulated in LTspice to verify functional correctness.

- **D_Flip_Flop – Data Storage Element Design:**  
  This project presents the design of a positive edge-triggered master-slave D flip-flop using CMOS technology in LTspice. Inverter and transmission gate modules were used to construct master and slave latches, which were then combined into a complete flip-flop circuit.

- **Gate Level Modules:** Basic logic gates such as NAND, NOR, INV, and their submodules  
- **Symbol & Subckt Structures:** Each circuit is provided with its `.asy` and `.sub` files for symbolization

## 📄 Reports and Documentation

Detailed explanations, component descriptions, simulation steps, and result analyses for each project can be found under the `Design Reports/` folder.

This folder includes individual sub-reports for each project, covering both the theoretical background and the practical simulation steps in a well-documented format.

## 🛠️ Tools Used

- [LTspice XVII](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) – for circuit design and simulation
- Notepad – for editing netlists and documentation

## 📚 Educational Use Only

All contents of this project are shared solely for individual learning and academic evaluation. Copying, redistribution, or reuse in other projects is **strictly prohibited**.

## © Copyright

**Copyright (c) 2025 Nida Mert**

All rights reserved. The source files, documentation, and visuals are provided strictly for educational and personal review purposes only.