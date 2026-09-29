# 4:2 Encoder

## Overview

A 4:2 Encoder is a combinational logic circuit that converts one of four active input lines into a 2-bit binary output.

For a standard 4:2 encoder, only one input should be HIGH at a time.

## Inputs

- D0 - Input 0
- D1 - Input 1
- D2 - Input 2
- D3 - Input 3

## Outputs

- Y1 - Output bit 1
- Y0 - Output bit 0

## Truth Table

| D3 | D2 | D1 | D0 | Y1 | Y0 |
|----|----|----|----|----|----|
| 0  | 0  | 0  | 1  | 0  | 0  |
| 0  | 0  | 1  | 0  | 0  | 1  |
| 0  | 1  | 0  | 0  | 1  | 0  |
| 1  | 0  | 0  | 0  | 1  | 1  |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `encoder4x2_structural.v` - Structural Verilog implementation
- `encoder4x2_dataflow.v` - Dataflow Verilog implementation
- `encoder4x2_behavioral.v` - Behavioral Verilog implementation
- `tb_encoder4x2.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 4:2 Encoder was verified using a Verilog testbench and Vivado simulation by testing each valid one-hot input combination.

## Result

The 4:2 Encoder successfully converts the active input line into its corresponding 2-bit binary code.
