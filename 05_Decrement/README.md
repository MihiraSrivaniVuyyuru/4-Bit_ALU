# Decrement

## Overview

This folder contains the **transistor-level implementation of CMOS Decrement circuits** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. Both **1-bit** and **4-bit** decrementers are implemented to demonstrate binary decrement operations at the transistor level.

A decrementer is a fundamental arithmetic circuit that decreases a binary number by **one**. It is commonly used in countdown timers, address generators, loop control logic, stack pointers, and Arithmetic Logic Units (ALUs). The circuits were functionally verified through transient simulations to ensure accurate decrement operations.

---

## Folder Structure

```text
Decrement/
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

### 1-Bit Decrementer

The 1-bit decrementer performs the operation:

```text
Output = Input - 1
```

For a single-bit input, the circuit generates the decremented output while handling the borrow generated during the subtraction.

**Available Files**

- **Schematic** – Transistor-level CMOS 1-bit decrementer implementation.
- **Symbol** – Custom symbol created for hierarchical circuit design.
- **Test** – Testbench developed for functional verification.
- **Waveform** – Transient simulation validating correct decrement operation.

---

### 4-Bit Decrementer

The 4-bit decrementer performs binary decrementation by subtracting **1** from a 4-bit input operand.

```text
Y = A - 1
```

where

- **A = A₃A₂A₁A₀**
- **Y = Y₃Y₂Y₁Y₀**

The borrow generated at each stage propagates through the higher-order bits to produce the correct decremented output.

**Available Files**

- **Schematic** – Complete transistor-level 4-bit decrementer.
- **Symbol** – Hierarchical symbol for reusable circuit integration.
- **Test** – Testbench covering multiple input combinations.
- **Waveform** – Simulation results validating correct decrement functionality.

---

## Design Flow

1. Designed the transistor-level CMOS decrementer circuits in Cadence Virtuoso.
2. Created reusable schematic symbols for hierarchical circuit design.
3. Developed dedicated testbenches for functional verification.
4. Performed transient simulations.
5. Verified the outputs against the expected decrement operation for all test cases.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Arithmetic Logic Units (ALUs)
- Countdown Timers
- Stack Pointers
- Address Generation Units
- Loop Control Circuits
- Embedded Systems
- Microprocessors and Microcontrollers
- Digital Signal Processing Systems

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS decrementer design
- Transistor-level arithmetic circuit implementation
- Single-bit and multi-bit decrement operations
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
