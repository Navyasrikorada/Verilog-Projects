# 8:3 Encoder

## Overview

An 8:3 Encoder is a combinational logic circuit that converts one of eight active input lines into a 3-bit binary output.

For a standard 8:3 encoder, only one input should be HIGH at a time.

## Inputs

- D0 - Input 0
- D1 - Input 1
- D2 - Input 2
- D3 - Input 3
- D4 - Input 4
- D5 - Input 5
- D6 - Input 6
- D7 - Input 7

## Outputs

- Y2 - Output bit 2
- Y1 - Output bit 1
- Y0 - Output bit 0

## Truth Table

| D7 | D6 | D5 | D4 | D3 | D2 | D1 | D0 | Y2 | Y1 | Y0 |
|----|----|----|----|----|----|----|----|----|----|----|
| 0  | 0  | 0  | 0  | 0  | 0  | 0  | 1  | 0  | 0  | 0  |
| 0  | 0  | 0  | 0  | 0  | 0  | 1  | 0  | 0  | 0  | 1  |
| 0  | 0  | 0  | 0  | 0  | 1  | 0  | 0  | 0  | 1  | 0  |
| 0  | 0  | 0  | 0  | 1  | 0  | 0  | 0  | 0  | 1  | 1  |
| 0  | 0  | 0  | 1  | 0  | 0  | 0  | 0  | 1  | 0  | 0  |
| 0  | 0  | 1  | 0  | 0  | 0  | 0  | 0  | 1  | 0  | 1  |
| 0  | 1  | 0  | 0  | 0  | 0  | 0  | 0  | 1  | 1  | 0  |
| 1  | 0  | 0  | 0  | 0  | 0  | 0  | 0  | 1  | 1  | 1  |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `encoder8x3_structural.v` - Structural Verilog implementation
- `encoder8x3_dataflow.v` - Dataflow Verilog implementation
- `encoder8x3_behavioral.v` - Behavioral Verilog implementation
- `tb_encoder8x3.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 8:3 Encoder was verified using a Verilog testbench and Vivado simulation by testing each valid one-hot input combination.

## Result

The 8:3 Encoder successfully converts the active input line into its corresponding 3-bit binary code.
