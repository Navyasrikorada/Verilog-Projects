# 1-Bit Comparator

## Overview

A 1-Bit Comparator is a combinational logic circuit used to compare two 1-bit binary inputs and determine whether one input is greater than, less than, or equal to the other.

## Inputs

- A - First 1-bit input
- B - Second 1-bit input

## Outputs

- A_gt_B - Indicates A is greater than B
- A_eq_B - Indicates A is equal to B
- A_lt_B - Indicates A is less than B

## Truth Table

| A | B | A_gt_B | A_eq_B | A_lt_B |
|---|---|--------|--------|--------|
| 0 | 0 |   0    |   1    |   0    |
| 0 | 1 |   0    |   0    |   1    |
| 1 | 0 |   1    |   0    |   0    |
| 1 | 1 |   0    |   1    |   0    |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `comparator1bit_structural.v` - Structural Verilog implementation
- `comparator1bit_dataflow.v` - Dataflow Verilog implementation
- `comparator1bit_behavioral.v` - Behavioral Verilog implementation
- `tb_comparator1bit.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 1-Bit Comparator was verified using a Verilog testbench and Vivado simulation by testing all possible input combinations.

## Result

The 1-Bit Comparator successfully determines whether A is greater than, equal to, or less than B.
