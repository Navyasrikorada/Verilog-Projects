# 4-Bit ALU

## Overview

A 4-Bit Arithmetic Logic Unit (ALU) is a combinational digital circuit that performs arithmetic and logical operations on two 4-bit binary inputs.

The operation is selected using control/select lines.

## Inputs

- A[3:0] - First 4-bit input
- B[3:0] - Second 4-bit input
- S[2:0] - Operation select inputs

## Outputs

- Y[3:0] - 4-bit ALU result
- Carry - Carry output

## Operations

| S2 | S1 | S0 | Operation |
|----|----|----|-----------|
| 0  | 0  | 0  | A + B |
| 0  | 0  | 1  | A - B |
| 0  | 1  | 0  | A & B |
| 0  | 1  | 1  | A | B |
| 1  | 0  | 0  | A ^ B |
| 1  | 0  | 1  | ~A |
| 1  | 1  | 0  | A + 1 |
| 1  | 1  | 1  | A - 1 |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `alu4bit_structural.v` - Structural Verilog implementation
- `alu4bit_dataflow.v` - Dataflow Verilog implementation
- `alu4bit_behavioral.v` - Behavioral Verilog implementation
- `tb_alu4bit.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 4-Bit ALU was verified using a Verilog testbench and Vivado simulation by testing the supported arithmetic and logical operations.

## Result

The 4-Bit ALU successfully performs the selected arithmetic and logical operations on two 4-bit input values.
