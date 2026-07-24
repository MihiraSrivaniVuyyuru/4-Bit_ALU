# 4-Bit Arithmetic Logic Unit (ALU)

## Overview

This folder contains the **transistor-level implementation of a 4-Bit Arithmetic Logic Unit (ALU)** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. The ALU integrates multiple arithmetic, logical, comparison, and shift operations into a single combinational circuit capable of executing different operations based on a **4-bit control opcode**.

The design follows a **hierarchical full-custom CMOS methodology**, where previously developed digital modules—including logic gates, arithmetic circuits, comparator, multiplier, multiplexers, and shift units—are integrated to construct a complete 4-bit ALU. Functional verification was performed using transient simulations to validate every supported operation.

---

## Folder Structure

```text
ALU/
├── Schematic.png
├── Symbol.png
├── Test.png
└── Waveform.png
```

---

## Design Details

The ALU accepts two 4-bit operands (**A** and **B**) and executes one of sixteen operations depending on the applied **4-bit opcode**.

### Features

- 4-Bit Operand Processing
- 16 Supported Operations
- Hierarchical Full-Custom CMOS Design
- Arithmetic, Logical, Shift, Comparison, and Multiplication Operations
- Modular Circuit Architecture
- Complete Functional Verification using Transient Simulation

---

## Operation Selection (Opcode Table)

The operation performed by the ALU is determined by the applied **4-bit opcode**.

| Opcode | Operation | Description |
|:------:|-----------|-------------|
| `0000` | **NOT** | Bitwise NOT (Inversion) |
| `0001` | **BUFFER** | Pass input directly to output |
| `0010` | **AND** | Bitwise AND |
| `0011` | **OR** | Bitwise OR |
| `0100` | **NAND** | Bitwise NAND |
| `0101` | **NOR** | Bitwise NOR |
| `0110` | **XOR** | Bitwise Exclusive-OR |
| `0111` | **XNOR** | Bitwise Exclusive-NOR |
| `1000` | **ADD** | Binary Addition |
| `1001` | **SUB** | Binary Subtraction |
| `1010` | **INC** | Increment by 1 |
| `1011` | **DEC** | Decrement by 1 |
| `1100` | **LSL** | Logical Shift Left |
| `1101` | **LSR** | Logical Shift Right |
| `1110` | **COMP** | Magnitude Comparison |
| `1111` | **MUL** | Binary Multiplication |

---

## Available Files

- **Schematic** – Complete transistor-level CMOS implementation of the 4-Bit ALU.
- **Symbol** – Hierarchical symbol for system-level integration.
- **Test** – Testbench developed to verify all supported ALU operations.
- **Waveform** – Transient simulation results validating the functionality of every opcode.

---


## Performance Analysis

Post-layout/schematic-level performance metrics were extracted through simulation to evaluate the power and timing characteristics of the 4-Bit ALU.

### Power Analysis

| Parameter | Value |
|-----------|-------|
| **Average Power (P_avg)** | 1.3559e-04 W (135.59 µW) |
| **Static Power (P_static)** | 2.0579e-10 W (0.21 nW) |
| **Leakage Power (P_leakage)** | 2.0579e-10 W (0.21 nW) |
| **Dynamic Power (P_dynamic)** | 1.3559e-04 W (135.59 µW) |

### Timing Analysis

| Parameter | Value |
|-----------|-------|
| **Average Propagation Delay** | 3.6565e-10 s (365.65 ps) |
| **Worst-Case (Max) Delay** | 1.7745e-09 s (1774.54 ps) |

**Observation:** Dynamic power dominates total power consumption, indicating the design is switching-activity driven with negligible static/leakage contribution — consistent with expected behavior in 45 nm CMOS combinational logic.

---

## Design Flow

1. Designed transistor-level CMOS implementations of individual logic gates.
2. Developed arithmetic modules including Adder, Subtractor, Incrementer, Decrementer, and Multiplier.
3. Implemented Comparator and Shift Logic circuits.
4. Designed multiplexers for operation selection based on the opcode.
5. Integrated all functional blocks into a unified 4-Bit ALU architecture.
6. Created a reusable hierarchical symbol in Cadence Virtuoso.
7. Developed comprehensive testbenches covering all sixteen operations.
8. Performed transient simulations to verify the functionality of every supported operation.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Arithmetic Logic Units (ALUs)
- Microprocessors
- Microcontrollers
- CPU Datapaths
- Digital Signal Processing (DSP)
- Embedded Systems
- FPGA and ASIC Prototyping
- General-Purpose Digital Computing Systems

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS digital circuit design
- Hierarchical VLSI design methodology
- Transistor-level implementation of arithmetic and logical circuits
- Integration of reusable digital building blocks
- Symbol creation in Cadence Virtuoso
- Testbench development for functional verification
- Transient simulation and waveform analysis
- Complete ALU implementation using modular CMOS architecture

---

## Project Highlights

- **Technology:** 45 nm CMOS
- **EDA Tool:** Cadence Virtuoso
- **Architecture:** Hierarchical Modular Design
- **Supported Operations:** 16
- **Design Methodology:** Full-Custom CMOS
- **Verification:** Transient Simulation

---

## Author

**Vuyyuru Mihira Srivani**

B.Tech in Electronics and Communication Engineering (VLSI)  
VIT-AP University

- **GitHub:** https://github.com/MihiraSrivaniVuyyuru
- **LinkedIn:** https://www.linkedin.com/in/vuyyurumihirasrivani

**Interests:** Full-Custom CMOS Design • Digital VLSI • Low-Power VLSI • ASIC Design
