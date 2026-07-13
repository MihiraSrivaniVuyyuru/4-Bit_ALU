# XNOR Gate

## Overview

This folder contains the **transistor-level implementation of CMOS XNOR (Exclusive-NOR) gates** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. Both **1-bit** and **4-bit** implementations are included to demonstrate the realization of the Exclusive-NOR operation and its scalability for multi-bit digital systems.

The XNOR gate is a fundamental combinational logic circuit that produces a HIGH output only when both inputs are identical. It is widely used in equality comparators, parity checking, error detection, and digital decision-making circuits. The designs were verified through transient simulations to ensure accurate logical functionality.

---

## Folder Structure

```
XNOR/
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

### 1-Bit XNOR Gate

The 1-bit XNOR gate performs the Exclusive-NOR operation, producing a HIGH output only when both inputs are equal.

#### Truth Table

| Input A | Input B | Output Y |
|:-------:|:-------:|:--------:|
| 0 | 0 | 1 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

**Available Files**

- **Schematic** – Transistor-level CMOS XNOR gate implementation.
- **Symbol** – Custom symbol created for hierarchical circuit design.
- **Test** – Testbench used for functional verification.
- **Waveform** – Transient simulation confirming correct XNOR operation.

---

### 4-Bit XNOR Gate

The 4-bit XNOR gate performs four independent Exclusive-NOR operations simultaneously on two 4-bit input vectors.

```
Y = ~(A ⊕ B)
```

where

- **A = A₃A₂A₁A₀**
- **B = B₃B₂B₁B₀**
- **Y = Y₃Y₂Y₁Y₀**

Each output bit is independently computed as

```
Yi = ~(Ai ⊕ Bi)
```

This implementation demonstrates efficient parallel equality checking, making it suitable for digital comparators, parity verification, and processor datapath applications.

**Available Files**

- **Schematic** – Complete 4-bit transistor-level CMOS XNOR circuit.
- **Symbol** – Hierarchical symbol for higher-level digital designs.
- **Test** – Testbench applying multiple input combinations.
- **Waveform** – Simulation results validating the functionality of all four output bits.

---

## Design Flow

1. Designed the transistor-level CMOS XNOR gate in Cadence Virtuoso.
2. Created reusable schematic symbols for hierarchical circuit design.
3. Developed dedicated testbenches for functional verification.
4. Performed transient simulations.
5. Verified the outputs against the expected XNOR truth table.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Equality Comparators
- Arithmetic Logic Units (ALUs)
- Parity Generators and Checkers
- Error Detection and Correction
- Digital Decision-Making Circuits
- Data Comparison Systems
- Processor Datapaths
- Embedded Digital Systems

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS XNOR gate design
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
