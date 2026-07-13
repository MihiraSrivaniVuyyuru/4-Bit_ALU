# NAND Gate

## Overview

This folder contains the **transistor-level implementation of CMOS NAND gates** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. Both **1-bit** and **4-bit** implementations are provided to demonstrate the scalability of the design from a fundamental logic gate to a multi-bit digital circuit.

The NAND gate is one of the most important universal logic gates, capable of implementing any Boolean function through suitable combinations. The designs were verified using transient simulations to ensure accurate logical functionality.

---

## Folder Structure

```
NAND/
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

### 1-Bit NAND Gate

The 1-bit NAND gate performs the logical NAND operation, producing a LOW output only when all inputs are HIGH.

#### Truth Table

| Input A | Input B | Output Y |
|:-------:|:-------:|:--------:|
| 0 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

**Available Files**

- **Schematic** – Transistor-level CMOS NAND gate implementation.
- **Symbol** – Custom symbol for hierarchical circuit integration.
- **Test** – Testbench developed for functional verification.
- **Waveform** – Transient simulation confirming correct NAND operation.

---

### 4-Bit NAND Gate

The 4-bit NAND gate performs four independent NAND operations simultaneously on two 4-bit input vectors.

```
Y = ~(A & B)
```

where

- **A = A₃A₂A₁A₀**
- **B = B₃B₂B₁B₀**
- **Y = Y₃Y₂Y₁Y₀**

Each output bit is computed independently as

```
Yi = ~(Ai & Bi)
```

This implementation demonstrates efficient parallel processing of multiple data bits while preserving the universal logic characteristics of the NAND gate.

**Available Files**

- **Schematic** – Complete 4-bit transistor-level CMOS NAND circuit.
- **Symbol** – Hierarchical symbol for higher-level digital designs.
- **Test** – Testbench applying multiple input combinations.
- **Waveform** – Simulation results validating all four output bits.

---

## Design Flow

1. Designed the transistor-level CMOS NAND gate in Cadence Virtuoso.
2. Created reusable schematic symbols for hierarchical design.
3. Developed dedicated testbenches for functional verification.
4. Performed transient simulations.
5. Verified the outputs against the expected NAND truth table.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Analog/Transient Analysis

---

## Applications

- Universal Logic Design
- Arithmetic Logic Units (ALUs)
- Digital Control Logic
- Sequential Circuit Design
- Processor Datapaths
- Memory Address Decoding
- Embedded Systems
- General-Purpose Digital Integrated Circuits

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS NAND gate design
- Transistor-level digital logic implementation
- Hierarchical schematic development
- Symbol creation in Cadence Virtuoso
- Testbench development for functional verification
- Transient simulation and waveform analysis
- Multi-bit digital circuit implementation using universal logic gates

---

## Author

**Vuyyuru Mihira Srivani**

B.Tech in Electronics and Communication Engineering (VLSI)  
VIT-AP University

- GitHub: https://github.com/MihiraSrivaniVuyyuru
- LinkedIn: https://www.linkedin.com/in/vuyyurumihirasrivani

**Research Interests:** VLSI Design, CMOS Digital Circuit Design, Low-Power VLSI, ASIC Design
