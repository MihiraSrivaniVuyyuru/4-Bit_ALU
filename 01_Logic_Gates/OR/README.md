# OR Gate

## Overview

This folder contains the **transistor-level implementation of CMOS OR gates** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. Both **1-bit** and **4-bit** implementations are included to demonstrate the realization of the OR operation and its scalability for multi-bit digital systems.

The OR gate is one of the fundamental combinational logic gates in digital electronics. It produces a HIGH output whenever at least one input is HIGH, making it an essential building block for arithmetic circuits, control logic, and digital processing systems. The implementations were verified through transient simulations to ensure accurate logical functionality.

---

## Folder Structure

```
OR/
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

### 1-Bit OR Gate

The 1-bit OR gate performs the logical OR operation by producing a HIGH output whenever one or both inputs are HIGH.

#### Truth Table

| Input A | Input B | Output Y |
|:-------:|:-------:|:--------:|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 1 |

**Available Files**

- **Schematic** – Transistor-level CMOS OR gate implementation.
- **Symbol** – Custom symbol created for hierarchical circuit design.
- **Test** – Testbench used for functional verification.
- **Waveform** – Transient simulation confirming correct OR operation.

---

### 4-Bit OR Gate

The 4-bit OR gate performs four independent OR operations simultaneously on two 4-bit input vectors.

```
Y = A | B
```

where

- **A = A₃A₂A₁A₀**
- **B = B₃B₂B₁B₀**
- **Y = Y₃Y₂Y₁Y₀**

Each output bit is independently computed as

```
Yi = Ai | Bi
```

This implementation demonstrates efficient parallel processing of multiple data bits, making it suitable for datapath operations and digital signal processing applications.

**Available Files**

- **Schematic** – Complete 4-bit transistor-level CMOS OR circuit.
- **Symbol** – Hierarchical symbol for higher-level digital designs.
- **Test** – Testbench applying multiple input combinations.
- **Waveform** – Simulation results validating the functionality of all four output bits.

---

## Design Flow

1. Designed the transistor-level CMOS OR gate in Cadence Virtuoso.
2. Created reusable schematic symbols for hierarchical circuit design.
3. Developed dedicated testbenches for functional verification.
4. Performed transient simulations.
5. Verified the outputs against the expected OR truth table.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Arithmetic Logic Units (ALUs)
- Digital Control Logic
- Address Decoding
- Data Selection Circuits
- Processor Datapaths
- Embedded Systems
- Digital Signal Processing
- CMOS Digital Integrated Circuits

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS OR gate design
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
