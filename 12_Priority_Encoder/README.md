# Priority Encoder

## Overview

A Priority Encoder is a combinational logic circuit that converts multiple input lines into a binary code based on priority.

When more than one input is HIGH, the input with the highest priority is encoded into the binary output.

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
- Valid - Indicates that at least one input is active

## Priority

The priority is:

D7 > D6 > D5 > D4 > D3 > D2 > D1 > D0

## Truth Table

| D7 | D6 | D5 | D4 | D3 | D2 | D1 | D0 | Y2 | Y1 | Y0 | Valid |
|----|----|----|----|----|----|----|----|----|----|----|-------|
| 1  | X  | X  | X  | X  | X  | X  | X  | 1  | 1  | 1  | 1 |
| 0  | 1  | X  | X  | X  | X  | X  | X  | 1  | 1  | 0  | 1 |
| 0  | 0  | 1  | X  | X  | X  | X  | X  | 1  | 0  | 1  | 1 |
| 0  | 0  | 0  | 1  | X  | X  | X  | X  | 1  | 0  | 0  | 1 |
| 0  | 0  | 0  | 0  | 1  | X  | X  | X  | 0  | 1  | 1  | 1 |
| 0  | 0  | 0  | 0  | 0  | 1  | X  | X  | 0  | 1  | 0  | 1 |
| 0  | 0  | 0  | 0  | 0  | 0  | 1  | X  | 0  | 0  | 1  | 1 |
| 0  | 0  | 0  | 0  | 0  | 0  | 0  | 1  | 0  | 0  | 0  | 1 |
| 0  | 0  | 0  | 0  | 0  | 0  | 0  | 0  | 0  | 0  | 0  | 0 |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `priority_encoder_structural.v` - Structural Verilog implementation
- `priority_encoder_dataflow.v` - Dataflow Verilog implementation
- `priority_encoder_behavioral.v` - Behavioral Verilog implementation
- `tb_priority_encoder.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The Priority Encoder was verified using a Verilog testbench and Vivado simulation by testing different input combinations, including multiple active inputs.

## Result

The Priority Encoder successfully generates the binary code corresponding to the highest-priority active input.
