# Multiplier

## Overview

This folder contains the **transistor-level implementation of a CMOS Binary Multiplier** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. The multiplier performs binary multiplication of two input operands and produces the corresponding product output through combinational logic.

Binary multipliers are fundamental arithmetic circuits used in digital signal processing (DSP), processors, embedded systems, and Arithmetic Logic Units (ALUs). The design was functionally verified using transient simulations to ensure accurate multiplication results for different input combinations.

---

## Folder Structure

```text
Multiplier/
├── Schematic.png
├── Symbol.png
├── Test.png
├── Waveform1.png
└── Waveform2.png
```

---

## Design Details

The multiplier performs binary multiplication between two input operands by generating partial products and combining them to obtain the final product.

```text
Product = A × B
```

where

- **A** – Multiplicand
- **B** – Multiplier
- **Product** – Binary multiplication result

The design implements transistor-level combinational logic to perform multiplication while ensuring correct propagation of partial products and carries.

**Available Files**

- **Schematic** – Complete transistor-level CMOS multiplier implementation.
- **Symbol** – Custom symbol created for hierarchical circuit integration.
- **Test** – Testbench developed for functional verification.
- **Waveform1** – Transient simulation demonstrating multiplication for one set of input combinations.
- **Waveform2** – Additional transient simulation validating the multiplier under different input conditions.

---

## Design Flow

1. Designed the transistor-level CMOS multiplier in Cadence Virtuoso.
2. Created a reusable schematic symbol for hierarchical design.
3. Developed a dedicated testbench for functional verification.
4. Performed transient simulations using multiple input combinations.
5. Verified the generated product against the expected binary multiplication results.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Arithmetic Logic Units (ALUs)
- Digital Signal Processors (DSPs)
- Microprocessors and Microcontrollers
- Embedded Systems
- Image and Signal Processing
- Digital Communication Systems
- Hardware Accelerators
- ASIC and FPGA Arithmetic Units

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS multiplier design
- Transistor-level arithmetic circuit implementation
- Binary multiplication using combinational logic
- Hierarchical schematic development
- Symbol creation in Cadence Virtuoso
- Testbench development for functional verification
- Transient simulation and waveform analysis
- Verification of arithmetic circuit functionality

---

## Author

**Vuyyuru Mihira Srivani**

B.Tech in Electronics and Communication Engineering (VLSI)  
VIT-AP University

- **GitHub:** https://github.com/MihiraSrivaniVuyyuru
- **LinkedIn:** https://www.linkedin.com/in/vuyyurumihirasrivani

**Interests:** Full-Custom CMOS Design • Digital VLSI • Low-Power VLSI • ASIC Design
