# Buffer

## Overview

This folder contains the **transistor-level implementation of CMOS Buffer circuits** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. Both **1-bit** and **4-bit** buffer implementations are included to demonstrate signal buffering at the transistor level and its scalability for multi-bit digital systems.

A buffer is a non-inverting logic circuit that reproduces the input signal at the output while improving signal integrity, increasing drive strength, and isolating circuit stages. The designs were verified using transient simulations to ensure correct functionality.

---

## Folder Structure

```
Buffer/
├── 1_Bit/
│   ├── Schematic.png
│   ├── Symbol.png
│   ├── Test.png
│   └── Waveform.png
│
└── 4_Bit/
    ├── Schematic.png
    ├── Symbol.png
    ├── Test.png
    └── Waveform.png
```

---

## Design Details

### 1-Bit Buffer

The 1-bit CMOS buffer reproduces the input logic level at the output without inversion while providing improved driving capability for subsequent circuit stages.

#### Truth Table

| Input (A) | Output (Y) |
|:---------:|:----------:|
| 0 | 0 |
| 1 | 1 |

**Available Files**

- **Schematic** – Transistor-level CMOS buffer implementation.
- **Symbol** – Custom symbol for hierarchical circuit integration.
- **Test** – Testbench used for functional verification.
- **Waveform** – Transient simulation confirming correct buffer operation.

---

### 4-Bit Buffer

The 4-bit buffer simultaneously transfers four input bits to their corresponding outputs without modifying the logic values.

```
Y = A
```

where

- **A = A₃A₂A₁A₀**
- **Y = Y₃Y₂Y₁Y₀**

Each output bit is independently buffered as

```
Yi = Ai
```

This implementation demonstrates the use of multiple buffer stages for parallel data transmission in digital systems.

**Available Files**

- **Schematic** – Complete 4-bit transistor-level buffer circuit.
- **Symbol** – Hierarchical symbol for system-level integration.
- **Test** – Testbench for validating multiple input combinations.
- **Waveform** – Simulation results confirming correct operation of all four output bits.

---

## Design Flow

1. Designed the CMOS transistor-level buffer in Cadence Virtuoso.
2. Created reusable schematic symbols for hierarchical design.
3. Developed dedicated testbenches for functional verification.
4. Performed transient simulations.
5. Verified that the output accurately follows the input under all test conditions.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Signal Buffering
- Fan-Out Enhancement
- Digital Signal Distribution
- Clock Distribution Networks
- Processor Datapaths
- Memory Interfaces
- High-Speed Digital Circuits
- Arithmetic Logic Units (ALUs)

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS buffer design
- Transistor-level digital circuit implementation
- Hierarchical schematic design in Cadence Virtuoso
- Symbol creation for reusable circuit blocks
- Testbench development and transient simulation
- Functional verification of single-bit and multi-bit buffer circuits

---

## Author

**Vuyyuru Mihira Srivani**

B.Tech in Electronics and Communication Engineering (VLSI)  
VIT-AP University

- GitHub: https://github.com/MihiraSrivaniVuyyuru
- LinkedIn: https://www.linkedin.com/in/vuyyurumihirasrivani

**Research Interests:** VLSI Design, CMOS Digital Circuit Design, Low-Power VLSI, ASIC Design
