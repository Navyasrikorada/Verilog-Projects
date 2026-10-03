# 2-Bit Comparator

## Overview

A 2-Bit Comparator is a combinational logic circuit used to compare two 2-bit binary numbers and determine whether one number is greater than, less than, or equal to the other.

## Inputs

- A[1:0] - First 2-bit input
- B[1:0] - Second 2-bit input

## Outputs

- A_gt_B - Indicates A is greater than B
- A_eq_B - Indicates A is equal to B
- A_lt_B - Indicates A is less than B

## Truth Table

| A1 | A0 | B1 | B0 | A_gt_B | A_eq_B | A_lt_B |
|----|----|----|----|--------|--------|--------|
| 0  | 0  | 0  | 0  |   0    |   1    |   0    |
| 0  | 0  | 0  | 1  |   0    |   0    |   1    |
| 0  | 0  | 1  | 0  |   0    |   0    |   1    |
| 0  | 0  | 1  | 1  |   0    |   0    |   1    |
| 0  | 1  | 0  | 0  |   1    |   0    |   0    |
| 0  | 1  | 0  | 1  |   0    |   1    |   0    |
| 0  | 1  | 1  | 0  |   0    |   0    |   1    |
| 0  | 1  | 1  | 1  |   0    |   0    |   1    |
| 1  | 0  | 0  | 0  |   1    |   0    |   0    |
| 1  | 0  | 0  | 1  |   1    |   0    |   0    |
| 1  | 0  | 1  | 0  |   0    |   1    |   0    |
| 1  | 0  | 1  | 1  |   0    |   0    |   1    |
| 1  | 1  | 0  | 0  |   1    |   0    |   0    |
| 1  | 1  | 0  | 1  |   1    |   0    |   0    |
| 1  | 1  | 1  | 0  |   1    |   0    |   0    |
| 1  | 1  | 1  | 1  |   0    |   1    |   0    |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `comparator2bit_structural.v` - Structural Verilog implementation
- `comparator2bit_dataflow.v` - Dataflow Verilog implementation
- `comparator2bit_behavioral.v` - Behavioral Verilog implementation
- `tb_comparator2bit.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 2-Bit Comparator was verified using a Verilog testbench and Vivado simulation by testing all possible combinations of the two 2-bit inputs.

## Result

The 2-Bit Comparator successfully determines whether A is greater than, equal to, or less than B.
