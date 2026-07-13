# NOT Gate

## Overview

This folder contains the **transistor-level implementation of CMOS NOT (Inverter) circuits** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. Both **1-bit** and **4-bit** implementations are included to demonstrate the fundamental inversion operation and its scalability for multi-bit digital systems.

The NOT gate, also known as an **inverter**, is the most fundamental building block of digital electronics. It produces the logical complement of the input signal and is extensively used in combinational and sequential circuit design. The implementations were verified through transient simulations to ensure accurate inversion for all input conditions.

---

## Folder Structure

```
NOT/
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

### 1-Bit NOT Gate

The 1-bit NOT gate performs the logical inversion of a single input bit.

#### Truth Table

| Input (A) | Output (Y) |
|:---------:|:----------:|
| 0 | 1 |
| 1 | 0 |

**Available Files**

- **Schematic** – Transistor-level CMOS inverter implementation.
- **Symbol** – Custom symbol created for hierarchical circuit design.
- **Test** – Testbench used for functional verification.
- **Waveform** – Transient simulation confirming correct inversion.

---

### 4-Bit NOT Gate

The 4-bit NOT gate simultaneously inverts each bit of a 4-bit input vector.

```
Y = ~A
```

where

- **A = A₃A₂A₁A₀**
- **Y = Y₃Y₂Y₁Y₀**

Each output bit is independently computed as

```
Yi = ~Ai
```

This implementation demonstrates efficient parallel inversion of multiple bits, making it suitable for arithmetic units, data processing circuits, and digital control logic.

**Available Files**

- **Schematic** – Complete 4-bit transistor-level CMOS inverter circuit.
- **Symbol** – Hierarchical symbol for system-level integration.
- **Test** – Testbench for validating multiple input combinations.
- **Waveform** – Simulation results confirming correct inversion of all four output bits.

---

## Design Flow

1. Designed the transistor-level CMOS inverter in Cadence Virtuoso.
2. Created reusable schematic symbols for hierarchical circuit design.
3. Developed dedicated testbenches for functional verification.
4. Performed transient simulations.
5. Verified the outputs against the expected inverter truth table.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Signal Inversion
- Clock Signal Generation
- Logic Level Restoration
- Digital Signal Processing
- Arithmetic Logic Units (ALUs)
- Memory Circuits
- Processor Datapaths
- CMOS Digital Integrated Circuits

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS inverter design
- Transistor-level digital circuit implementation
- Hierarchical schematic development
- Symbol creation in Cadence Virtuoso
- Testbench development for functional verification
- Transient simulation and waveform analysis
- Multi-bit inverter implementation for digital systems

---

## Author

**Vuyyuru Mihira Srivani**

B.Tech in Electronics and Communication Engineering (VLSI)  
VIT-AP University

- **GitHub:** https://github.com/MihiraSrivaniVuyyuru
- **LinkedIn:** https://www.linkedin.com/in/vuyyurumihirasrivani

**Interests:** Full-Custom CMOS Design • Digital VLSI • Low-Power VLSI • ASIC Design
