# 8085 Microprocessor Calculator

This project implements a basic calculator using the **8085 Microprocessor**. The calculator performs arithmetic operations such as **addition, subtraction, multiplication, and division**.

## Features
- Addition of two numbers
- Subtraction of two numbers
- Multiplication of two numbers
- Division of two numbers
- Supports user input through assembly instructions

## Requirements
- 8085 Microprocessor Kit or Emulator (e.g., GNUSim8085, EdSim51, or similar)
- Assembler for 8085 (if using an emulator)
- Basic knowledge of 8085 Assembly language

## How to Use
1. Load the program into the 8085 microprocessor or an emulator.
2. Enter the required inputs when prompted.
3. The result will be displayed in the output register or memory location.

## Assembly Code Overview
The calculator uses **8085 assembly language** instructions to perform operations:
- `LDA` – Load data from memory
- `MOV` – Move data between registers
- `ADD` – Perform addition
- `SUB` – Perform subtraction
- `MUL` (SIMULATED) – Multiplication using repeated addition
- `DIV` (SIMULATED) – Division using repeated subtraction
- `HLT` – Halt execution

## Installation
If using an emulator:
1. Install **GNUSim8085** or any 8085 simulator.
2. Copy and paste the assembly code into the emulator.
3. Assemble and run the code.

## Example Code (Addition)
```assembly
LDA 2000H   ; Load first number from memory address 2000H
MOV B, A    ; Move it to register B
LDA 2001H   ; Load second number from memory address 2001H
ADD B       ; Add the value in register B
STA 2002H   ; Store result at memory address 2002H
HLT         ; Halt program execution
