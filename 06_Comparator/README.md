# Comparator

## Overview

This folder contains the **transistor-level implementation of CMOS Comparator circuits** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. Both **1-bit** and **4-bit** comparators are implemented to perform digital magnitude comparison between two binary numbers.

A comparator is a fundamental combinational circuit that determines the relationship between two binary inputs by indicating whether one value is **greater than**, **less than**, or **equal to** the other. These circuits are widely used in processors, ALUs, sorting hardware, digital control systems, and decision-making logic. The implementations were verified through transient simulations to ensure accurate comparison results.

---

## Folder Structure

```text
Comparator/
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

### 1-Bit Comparator

The 1-bit comparator compares two single-bit inputs (**A** and **B**) and generates three outputs:

- **A > B**
- **A = B**
- **A < B**

#### Truth Table

| A | B | A > B | A = B | A < B |
|:-:|:-:|:-----:|:-----:|:-----:|
| 0 | 0 |   0   |   1   |   0   |
| 0 | 1 |   0   |   0   |   1   |
| 1 | 0 |   1   |   0   |   0   |
| 1 | 1 |   0   |   1   |   0   |

**Available Files**

- **Schematic** – Transistor-level CMOS 1-bit comparator implementation.
- **Symbol** – Custom symbol created for hierarchical circuit design.
- **Test** – Testbench developed for functional verification.
- **Waveform** – Transient simulation validating comparison outputs.

---

### 4-Bit Comparator

The 4-bit comparator compares two 4-bit binary numbers and determines whether one operand is greater than, equal to, or less than the other.

```text
A = A₃A₂A₁A₀
B = B₃B₂B₁B₀
```

The outputs generated are:

- **A > B**
- **A = B**
- **A < B**

The comparison begins with the **Most Significant Bit (MSB)** and proceeds toward the **Least Significant Bit (LSB)** until a difference between the operands is identified.

**Available Files**

- **Schematic** – Complete transistor-level 4-bit comparator.
- **Symbol** – Hierarchical symbol for reusable circuit integration.
- **Test** – Testbench covering multiple comparison scenarios.
- **Waveform** – Simulation results validating correct comparison functionality.

---

## Design Flow

1. Designed the transistor-level CMOS comparator circuits in Cadence Virtuoso.
2. Created reusable schematic symbols for hierarchical circuit design.
3. Developed dedicated testbenches for functional verification.
4. Performed transient simulations.
5. Verified the outputs for greater-than, less-than, and equality conditions across all test cases.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Arithmetic Logic Units (ALUs)
- Microprocessors and Microcontrollers
- Address Comparison
- Digital Decision-Making Systems
- Sorting and Searching Hardware
- Embedded Systems
- Digital Signal Processing
- Processor Datapaths

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS comparator design
- Transistor-level combinational circuit implementation
- Single-bit and multi-bit magnitude comparison
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
