# 2:4 Decoder

## Overview

A 2:4 Decoder is a combinational logic circuit that converts a 2-bit binary input into one of four unique output lines. For each input combination, only one output is active.

## Inputs

- A - Input bit
- B - Input bit

## Outputs

- Y0 - Output 0
- Y1 - Output 1
- Y2 - Output 2
- Y3 - Output 3

## Truth Table

| A | B | Y0 | Y1 | Y2 | Y3 |
|---|---|----|----|----|----|
| 0 | 0 | 1  | 0  | 0  | 0  |
| 0 | 1 | 0  | 1  | 0  | 0  |
| 1 | 0 | 0  | 0  | 1  | 0  |
| 1 | 1 | 0  | 0  | 0  | 1  |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `decoder2x4_structural.v` - Structural Verilog implementation
- `decoder2x4_dataflow.v` - Dataflow Verilog implementation
- `decoder2x4_behavioral.v` - Behavioral Verilog implementation
- `tb_decoder2x4.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 2:4 Decoder was verified using a Verilog testbench and Vivado simulation by testing all possible input combinations.

## Result

The 2:4 Decoder successfully activates the corresponding output line for each 2-bit input combination.
