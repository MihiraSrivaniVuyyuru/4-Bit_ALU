# Logical Shift Right (LSR)

## Overview

This folder contains the **transistor-level implementation of a Logical Shift Right (LSR) circuit** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. The circuit performs a logical right shift operation on a binary input by shifting all bits one position toward the least significant bit (LSB) while inserting a **logic 0** into the most significant bit (MSB).

Logical Shift Right is a fundamental operation in digital systems and is widely used in Arithmetic Logic Units (ALUs), processors, digital signal processing, and hardware-based arithmetic operations. The implementation was functionally verified through transient simulations to ensure correct shifting behavior.

---

## Folder Structure

```text
LSR/
├── Schematic.png
├── Symbol.png
├── Test.png
└── Waveform.png
```

---

## Design Details

The Logical Shift Right (LSR) circuit shifts every bit of the input operand one position toward the right.

```text
Y = A >> 1
```

where

- **A = A₃A₂A₁A₀** – Input operand
- **Y = Y₃Y₂Y₁Y₀** – Shifted output

The shifted output is obtained as:

```text
Y₃ = 0
Y₂ = A₃
Y₁ = A₂
Y₀ = A₁
```

The most significant bit is filled with **0**, while the least significant bit is discarded after the shift.

**Available Files**

- **Schematic** – Transistor-level CMOS Logical Shift Right implementation.
- **Symbol** – Custom symbol created for hierarchical circuit integration.
- **Test** – Testbench developed for functional verification.
- **Waveform** – Transient simulation validating correct logical right shift operation.

---

## Design Flow

1. Designed the transistor-level Logical Shift Right circuit in Cadence Virtuoso.
2. Created a reusable schematic symbol for hierarchical design.
3. Developed a dedicated testbench for functional verification.
4. Performed transient simulations.
5. Verified the shifted output against the expected logical right shift operation.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Arithmetic Logic Units (ALUs)
- Binary Division by Powers of Two
- Digital Signal Processing (DSP)
- Processor Datapaths
- Embedded Systems
- Address Manipulation
- Bitwise Data Processing
- Digital Communication Systems

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS shift circuit design
- Transistor-level implementation of logical shift operations
- Hierarchical schematic development
- Symbol creation in Cadence Virtuoso
- Testbench development for functional verification
- Transient simulation and waveform analysis
- Hardware implementation of bitwise shift operations

---

## Author

**Vuyyuru Mihira Srivani**

B.Tech in Electronics and Communication Engineering (VLSI)  
VIT-AP University

- **GitHub:** https://github.com/MihiraSrivaniVuyyuru
- **LinkedIn:** https://www.linkedin.com/in/vuyyurumihirasrivani

**Interests:** Full-Custom CMOS Design • Digital VLSI • Low-Power VLSI • ASIC Design
