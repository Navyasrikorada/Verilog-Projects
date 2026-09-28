# 3:8 Decoder

## Overview

A 3:8 Decoder is a combinational logic circuit that converts a 3-bit binary input into one of eight unique output lines. For each input combination, only one output is active.

## Inputs

- A - Input bit
- B - Input bit
- C - Input bit

## Outputs

- Y0 - Output 0
- Y1 - Output 1
- Y2 - Output 2
- Y3 - Output 3
- Y4 - Output 4
- Y5 - Output 5
- Y6 - Output 6
- Y7 - Output 7

## Truth Table

| A | B | C | Y0 | Y1 | Y2 | Y3 | Y4 | Y5 | Y6 | Y7 |
|---|---|---|----|----|----|----|----|----|----|----|
| 0 | 0 | 0 | 1  | 0  | 0  | 0  | 0  | 0  | 0  | 0  |
| 0 | 0 | 1 | 0  | 1  | 0  | 0  | 0  | 0  | 0  | 0  |
| 0 | 1 | 0 | 0  | 0  | 1  | 0  | 0  | 0  | 0  | 0  |
| 0 | 1 | 1 | 0  | 0  | 0  | 1  | 0  | 0  | 0  | 0  |
| 1 | 0 | 0 | 0  | 0  | 0  | 0  | 1  | 0  | 0  | 0  |
| 1 | 0 | 1 | 0  | 0  | 0  | 0  | 0  | 1  | 0  | 0  |
| 1 | 1 | 0 | 0  | 0  | 0  | 0  | 0  | 0  | 1  | 0  |
| 1 | 1 | 1 | 0  | 0  | 0  | 0  | 0  | 0  | 0  | 1  |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `decoder3x8_structural.v` - Structural Verilog implementation
- `decoder3x8_dataflow.v` - Dataflow Verilog implementation
- `decoder3x8_behavioral.v` - Behavioral Verilog implementation
- `tb_decoder3x8.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 3:8 Decoder was verified using a Verilog testbench and Vivado simulation by testing all possible input combinations.

## Result

The 3:8 Decoder successfully activates the corresponding output line for each 3-bit input combination.
