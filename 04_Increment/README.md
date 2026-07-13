# Increment

## Overview

This folder contains the **transistor-level implementation of CMOS Increment circuits** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. Both **1-bit** and **4-bit** incrementers are implemented to demonstrate binary increment operations at the transistor level.

An incrementer is a fundamental arithmetic circuit that increases a binary number by **one**. It is widely used in processors, program counters, address generators, loop counters, and Arithmetic Logic Units (ALUs). The circuits were functionally verified through transient simulations to ensure accurate increment operations.

---

## Folder Structure

```text
Increment/
├── 1Bit/
│   ├── Schematic.png
│   ├── Symbol.png
│   ├── Test.png
│   └── Waveform.png
│
└── 4Bit/
    ├── Schematic.png
    ├── Symbol.png
    ├── Test.png
    └── Waveform.png
```

---

## Design Details

### 1-Bit Incrementer

The 1-bit incrementer performs the operation:

```text
Output = Input + 1
```

For a single-bit input, the circuit generates the incremented output while handling the carry generated during the addition.

**Available Files**

- **Schematic** – Transistor-level CMOS 1-bit incrementer implementation.
- **Symbol** – Custom symbol created for hierarchical circuit design.
- **Test** – Testbench developed for functional verification.
- **Waveform** – Transient simulation validating correct increment operation.

---

### 4-Bit Incrementer

The 4-bit incrementer performs binary incrementation by adding **1** to a 4-bit input operand.

```text
Y = A + 1
```

where

- **A = A₃A₂A₁A₀**
- **Y = Y₃Y₂Y₁Y₀**

The carry generated at each stage propagates through the higher-order bits to produce the correct incremented output.

**Available Files**

- **Schematic** – Complete transistor-level 4-bit incrementer.
- **Symbol** – Hierarchical symbol for reusable circuit integration.
- **Test** – Testbench covering multiple input combinations.
- **Waveform** – Simulation results validating correct increment functionality.

---

## Design Flow

1. Designed the transistor-level CMOS incrementer circuits in Cadence Virtuoso.
2. Created reusable schematic symbols for hierarchical circuit design.
3. Developed dedicated testbenches for functional verification.
4. Performed transient simulations.
5. Verified the outputs against the expected increment operation for all test cases.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Arithmetic Logic Units (ALUs)
- Program Counters (PC)
- Address Generation Units
- Loop Counters
- Digital Counters
- Embedded Systems
- Microprocessors and Microcontrollers
- Digital Signal Processing Systems

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS incrementer design
- Transistor-level arithmetic circuit implementation
- Single-bit and multi-bit increment operations
- Hierarchical schematic development
- Symbol creation in Cadence Virtuoso
- Testbench development for functional verification
- Transient simulation and waveform analysis

---

## Author

**Vuyyuru Mihira Srivani**

B.Tech in Electronics and Communication Engineering (VLSI)  
VIT-AP University

- **GitHub:** https://github.com/MihiraSrivaniVuyyuru
- **LinkedIn:** https://www.linkedin.com/in/vuyyurumihirasrivani

**Interests:** Full-Custom CMOS Design • Digital VLSI • Low-Power VLSI • ASIC Design
