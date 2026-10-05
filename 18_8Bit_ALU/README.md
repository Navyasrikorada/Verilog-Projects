# 8-Bit ALU

## Overview

An 8-Bit Arithmetic Logic Unit (ALU) is a combinational digital circuit that performs arithmetic and logical operations on two 8-bit binary inputs.

The required operation is selected using control signals.

## Inputs

- A[7:0] - First 8-bit input
- B[7:0] - Second 8-bit input
- S[2:0] - Operation select inputs

## Outputs

- Y[7:0] - 8-bit ALU result
- Carry - Carry output

## Operations

| S2 | S1 | S0 | Operation |
|----|----|----|-----------|
| 0  | 0  | 0  | A + B |
| 0  | 0  | 1  | A - B |
| 0  | 1  | 0  | A & B |
| 0  | 1  | 1  | A \| B |
| 1  | 0  | 0  | A ^ B |
| 1  | 0  | 1  | ~A |
| 1  | 1  | 0  | A + 1 |
| 1  | 1  | 1  | A - 1 |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `alu8bit_structural.v` - Structural Verilog implementation
- `alu8bit_dataflow.v` - Dataflow Verilog implementation
- `alu8bit_behavioral.v` - Behavioral Verilog implementation
- `tb_alu8bit.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 8-Bit ALU was verified using a Verilog testbench and Vivado simulation by testing all supported arithmetic and logical operations.

## Result

The 8-Bit ALU successfully performs the selected arithmetic and logical operations on two 8-bit input values.
