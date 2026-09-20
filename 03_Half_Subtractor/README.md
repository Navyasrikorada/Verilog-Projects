# Half Subtractor

## Overview

A Half Subtractor is a combinational logic circuit that subtracts one 1-bit binary input from another and produces two outputs: Difference and Borrow.

## Inputs

- A - Minuend
- B - Subtrahend

## Outputs

- Difference
- Borrow

## Truth Table

| A | B | Difference | Borrow |
|---|---|------------|--------|
| 0 | 0 |     0      |   0    |
| 0 | 1 |     1      |   1    |
| 1 | 0 |     1      |   0    |
| 1 | 1 |     0      |   0    |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `half_subtractor_structural.v` - Structural Verilog implementation
- `half_subtractor_dataflow.v` - Dataflow Verilog implementation
- `half_subtractor_behavioral.v` - Behavioral Verilog implementation
- `tb_half_subtractor.v` - Testbench for verification
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The Half Subtractor was verified using a Verilog testbench. All possible input combinations were tested using Vivado simulation.

## Result

The Half Subtractor successfully performs 1-bit binary subtraction and produces the correct Difference and Borrow outputs.
