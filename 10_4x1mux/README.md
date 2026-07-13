# 4×1 Multiplexer (MUX)

## Overview

This folder contains the **transistor-level implementation of CMOS Multiplexer (MUX) circuits** designed using **Cadence Virtuoso** in **45 nm CMOS technology**. The design follows a hierarchical approach, beginning with a **2×1 Multiplexer** and extending it to implement a **4×1 Multiplexer**.

A multiplexer is a fundamental combinational circuit that selects one of several input signals and forwards it to a single output based on the values of the select lines. Multiplexers are widely used in processors, digital communication systems, ALUs, datapath design, and embedded systems. The circuits were verified through transient simulations to ensure correct data selection for all input combinations.

---

## Folder Structure

```text
4x1mux/
├── 2x1mux/
│   ├── Schematic.png
│   ├── Symbol.png
│   ├── Test.png
│   └── Waveform.png
│
├── Schematic.png
├── Symbol.png
├── Test.png
└── Waveform.png
```

---

## Design Details

### 2×1 Multiplexer

The 2×1 Multiplexer selects one of two input signals based on a single select line.

#### Logic Equation

```text
Y = S̅·I₀ + S·I₁
```

where

- **I₀, I₁** – Input signals
- **S** – Select input
- **Y** – Output

**Available Files**

- **Schematic** – Transistor-level CMOS 2×1 multiplexer implementation.
- **Symbol** – Reusable symbol for hierarchical circuit design.
- **Test** – Testbench developed for functional verification.
- **Waveform** – Transient simulation validating correct input selection.

---

### 4×1 Multiplexer

The 4×1 Multiplexer is implemented hierarchically using **2×1 Multiplexers**. It selects one of four input signals based on two select lines.

#### Logic Equation

```text
Y = I₀·S₁'S₀' + I₁·S₁'S₀ + I₂·S₁S₀' + I₃·S₁S₀
```

where

- **I₀, I₁, I₂, I₃** – Input signals
- **S₁, S₀** – Select lines
- **Y** – Output

The design demonstrates hierarchical circuit construction by combining multiple 2×1 multiplexers to realize a higher-order multiplexer.

**Available Files**

- **Schematic** – Complete transistor-level CMOS 4×1 multiplexer.
- **Symbol** – Hierarchical symbol for reusable integration.
- **Test** – Testbench covering all select-line combinations.
- **Waveform** – Simulation verifying correct data selection for every input.

---

## Design Flow

1. Designed the transistor-level CMOS 2×1 Multiplexer.
2. Created a reusable symbol for hierarchical circuit design.
3. Constructed the 4×1 Multiplexer using multiple 2×1 Multiplexers.
4. Developed dedicated testbenches for functional verification.
5. Performed transient simulations.
6. Verified correct output selection for all input and select-line combinations.

---

## Technology

- **EDA Tool:** Cadence Virtuoso
- **Technology Node:** 45 nm CMOS
- **Design Style:** Full-Custom CMOS
- **Simulation:** Transient Analysis

---

## Applications

- Arithmetic Logic Units (ALUs)
- Processor Datapaths
- Data Routing Networks
- Bus Arbitration
- Communication Systems
- Embedded Systems
- Memory Address Selection
- Digital Signal Processing

---

## Learning Outcomes

This implementation demonstrates:

- Full-custom CMOS multiplexer design
- Hierarchical circuit construction using reusable modules
- Transistor-level combinational logic implementation
- Symbol creation in Cadence Virtuoso
- Testbench development for functional verification
- Transient simulation and waveform analysis
- Data routing and selection in digital systems

---

## Author

**Vuyyuru Mihira Srivani**

B.Tech in Electronics and Communication Engineering (VLSI)  
VIT-AP University

- **GitHub:** https://github.com/MihiraSrivaniVuyyuru
- **LinkedIn:** https://www.linkedin.com/in/vuyyurumihirasrivani

**Interests:** Full-Custom CMOS Design • Digital VLSI • Low-Power VLSI • ASIC Design
