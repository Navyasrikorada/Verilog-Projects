# Full Subtractor

## Overview

A Full Subtractor is a combinational logic circuit that subtracts two 1-bit binary inputs along with a borrow input and produces Difference and Borrow outputs.

## Inputs

- A - Minuend
- B - Subtrahend
- Bin - Borrow input

## Outputs

- Difference
- Bout - Borrow output

## Truth Table

| A | B | Bin | Difference | Bout |
|---|---|-----|------------|------|
| 0 | 0 |  0  |     0      |  0   |
| 0 | 0 |  1  |     1      |  1   |
| 0 | 1 |  0  |     1      |  1   |
| 0 | 1 |  1  |     0      |  1   |
| 1 | 0 |  0  |     1      |  0   |
| 1 | 0 |  1  |     0      |  0   |
| 1 | 1 |  0  |     0      |  0   |
| 1 | 1 |  1  |     1      |  1   |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files
- `full_subtractor_behavioral.v` - Behavioral Verilog implementation
- `tb_full_subtractor.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The Full Subtractor was verified using a Verilog testbench. All possible input combinations were tested using Vivado simulation.

## Result

The Full Subtractor successfully performs 1-bit binary subtraction with borrow input and produces the correct Difference and Borrow outputs.
