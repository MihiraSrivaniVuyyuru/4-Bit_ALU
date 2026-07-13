# AND Gate

## Overview

This folder contains the transistor-level implementation of the **AND Gate** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. Both **1-bit** and **4-bit** implementations are included to demonstrate the scalability of the design from a basic logic gate to a multi-bit digital circuit.

Each implementation was verified through transient simulations to ensure correct logical functionality.

---

## Folder Structure

```
AND/
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

### 1-Bit AND Gate

The 1-bit AND gate performs the fundamental logical AND operation.

| Input A | Input B | Output Y |
|:------:|:------:|:---------:|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

**Available Files**

- **Schematic** – Transistor-level CMOS implementation.
- **Symbol** – Custom symbol created for hierarchical circuit design.
- **Test** – Testbench used for functional verification.
- **Waveform** – Simulation output confirming correct AND operation.

---

### 4-Bit AND Gate

The 4-bit AND gate performs four AND operations simultaneously on two 4-bit input vectors.

\[
Y = A and B
\]

where

- **A = A₃A₂A₁A₀**
- **B = B₃B₂B₁B₀**
- **Y = Y₃Y₂Y₁Y₀**

Each output bit is independently computed as

```
Yi = Ai AND Bi
```

This design demonstrates the scalability of the transistor-level implementation while maintaining correct logical behavior across multiple bits.

**Available Files**

- **Schematic** – Complete 4-bit transistor-level circuit.
- **Symbol** – Hierarchical symbol used in higher-level designs.
- **Test** – Testbench for applying multiple input combinations.
- **Waveform** – Simulation results validating all four output bits.

---

## Design Flow

1. Designed the transistor-level CMOS schematic in Cadence Virtuoso.
2. Created reusable schematic symbols.
3. Built dedicated testbenches for verification.
4. Performed transient simulations.
5. Verified outputs against the expected AND truth table.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full Custom CMOS
- **Simulation:** Transient Simulation

---

## Applications

- Arithmetic Logic Units (ALUs)
- Digital Signal Processing
- Data Masking
- Bitwise Operations
- Control Logic
- Embedded Systems
- Processor Datapaths

---

## Learning Outcomes

This implementation demonstrates:

- CMOS transistor-level logic design
- Hierarchical schematic development
- Symbol creation in Cadence Virtuoso
- Testbench construction
- Functional verification using transient analysis
- Multi-bit digital circuit implementation

---

## Author

**Vuyyuru Mihira Srivani**

B.Tech in Electronics and Communication Engineering (VLSI)  
VIT-AP University

- GitHub: https://github.com/MihiraSrivaniVuyyuru
- LinkedIn: https://www.linkedin.com/in/vuyyurumihirasrivani

**Research Interests:** VLSI Design, CMOS Digital Circuit Design, Low-Power VLSI, ASIC Design
