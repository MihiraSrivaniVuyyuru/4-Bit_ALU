# XOR Gate

## Overview

This folder contains the **transistor-level implementation of CMOS XOR (Exclusive-OR) gates** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. Both **1-bit** and **4-bit** implementations are included to demonstrate the realization of the Exclusive-OR operation and its application in multi-bit digital systems.

The XOR gate is a fundamental combinational logic circuit that produces a HIGH output only when the inputs are different. It plays a crucial role in arithmetic circuits, parity generation, error detection, and data comparison. The designs were verified through transient simulations to ensure accurate logical functionality.

---

## Folder Structure

```
XOR/
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

### 1-Bit XOR Gate

The 1-bit XOR gate performs the Exclusive-OR operation, producing a HIGH output only when the two inputs are different.

#### Truth Table

| Input A | Input B | Output Y |
|:-------:|:-------:|:--------:|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

**Available Files**

- **Schematic** – Transistor-level CMOS XOR gate implementation.
- **Symbol** – Custom symbol created for hierarchical circuit design.
- **Test** – Testbench used for functional verification.
- **Waveform** – Transient simulation confirming correct XOR operation.

---

### 4-Bit XOR Gate

The 4-bit XOR gate performs four independent Exclusive-OR operations simultaneously on two 4-bit input vectors.

```
Y = A ⊕ B
```

where

- **A = A₃A₂A₁A₀**
- **B = B₃B₂B₁B₀**
- **Y = Y₃Y₂Y₁Y₀**

Each output bit is independently computed as

```
Yi = Ai ⊕ Bi
```

This implementation demonstrates efficient parallel bitwise comparison, making it suitable for arithmetic operations, parity checking, and digital communication systems.

**Available Files**

- **Schematic** – Complete 4-bit transistor-level CMOS XOR circuit.
- **Symbol** – Hierarchical symbol for higher-level digital designs.
- **Test** – Testbench applying multiple input combinations.
- **Waveform** – Simulation results validating the functionality of all four output bits.

---

## Design Flow

1. Designed the transistor-level CMOS XOR gate in Cadence Virtuoso.
2. Created reusable schematic symbols for hierarchical circuit design.
3. Developed dedicated testbenches for functional verification.
4. Performed transient simulations.
5. Verified the outputs against the expected XOR truth table.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Arithmetic Logic Units (ALUs)
- Half Adders and Full Adders
- Parity Generators and Checkers
- Error Detection and Correction
- Data Comparison Circuits
- Cryptographic Hardware
- Digital Communication Systems
- Processor Datapaths

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS XOR gate design
- Transistor-level digital circuit implementation
- Hierarchical schematic development
- Symbol creation in Cadence Virtuoso
- Testbench development for functional verification
- Transient simulation and waveform analysis
- Multi-bit combinational logic implementation

---

## Author

**Vuyyuru Mihira Srivani**

B.Tech in Electronics and Communication Engineering (VLSI)  
VIT-AP University

- **GitHub:** https://github.com/MihiraSrivaniVuyyuru
- **LinkedIn:** https://www.linkedin.com/in/vuyyurumihirasrivani

**Interests:** Full-Custom CMOS Design • Digital VLSI • Low-Power VLSI • ASIC Design
