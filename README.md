# 4-Bit_ALU
4-bit Arithmetic Logic Unit (ALU) designed in Cadence Virtuoso using 45nm CMOS technology. Implements 16 arithmetic, logical, and shift operations with transistor-level CMOS schematics. Developed during my Research Internship at VIT-AP University.

## Overview

This repository documents the complete design flow of a 4-bit ALU, built bottom-up:

- Basic logic gates (1-bit and 4-bit) → arithmetic blocks (adder, subtractor, incrementer, decrementer) → comparator → multiplier → shifters → operation-select mux → full ALU
- Every module was designed at the transistor level in Virtuoso Schematic Editor, verified with Spectre transient simulations

---

## Tech Stack

| Tool / Technology | Purpose |
|---|---|
| Cadence Virtuoso (Schematic Editor, ADE-XL) | Circuit design & simulation setup |
| Spectre | Transient simulation /waveform analysis |
| 45nm CMOS | Target technology node |

---

## Repository Structure

```

4-Bit_ALU/
├── 01_Logic_Gates/       → NOT, Buffer, AND, OR, NAND, NOR, XOR, XNOR (1-bit & 4-bit)
├── 02_Adder/             → Half Adder, Full Adder (1-bit), 4-bit Adder
├── 03_Subtractor/        → Half Subtractor, Full Subtractor (1-bit), 4-bit Subtractor
├── 04_Increment/         → 1-bit & 4-bit Incrementer
├── 05_Decrement/         → 1-bit & 4-bit Decrementer
├── 06_Comparator/        → 1-bit & 4-bit Comparator
├── 07_Multiplier/        → 4-bit Multiplier
├── 08_LSL/               → 4-bit Logical Shift Left
├── 09_LSR/               → 4-bit Logical Shift Right
├── 10_4x1mux/             → Operation-select multiplexer
├── 11_ALU/               → Top-level 4-bit ALU integration
├── docs/                 → Internship certificate
├── .gitignore
├── LICENSE
└── README.md

```

Each module folder contains its own `README.md` with schematic, testbench, and waveform screenshots, along with a truth table or operation summary.

---


## Internship & Research Context

This project was completed as part of a VLSI research internship at **VIT-AP University**, ECE Department (VLSI specialization).

---

## License

This repository is licensed under the [MIT License](LICENSE).

⚠️ **Note:** This license covers only the original documentation, schematics, screenshots, and written content created by the author. It does **not** extend to Cadence Virtuoso software or any PDK (Process Design Kit) files, which remain the property of their respective owners and are **not included** in this repository.

---

## Author

**Vuyyuru Mihira Srivani**
B.Tech ECE (VLSI Specialization), VIT-AP University

Feel free to explore, raise issues, or reach out with questions about the design.
