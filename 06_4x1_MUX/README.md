# 4:1 Multiplexer (MUX)

## Overview

A 4:1 Multiplexer is a combinational logic circuit that selects one of four input signals and forwards the selected input to the output based on two select lines.

## Inputs

- I0 - Input 0
- I1 - Input 1
- I2 - Input 2
- I3 - Input 3
- S0 - Select input
- S1 - Select input

## Output

- Y - Selected output

## Truth Table

| S1 | S0 | Y  |
|----|----|----|
| 0  | 0  | I0 |
| 0  | 1  | I1 |
| 1  | 0  | I2 |
| 1  | 1  | I3 |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `mux4x1_structural.v` - Structural Verilog implementation
- `mux4x1_dataflow.v` - Dataflow Verilog implementation
- `mux4x1_behavioral.v` - Behavioral Verilog implementation
- `tb_mux4x1.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 4:1 Multiplexer was verified using a Verilog testbench and Vivado simulation by testing all select combinations.

## Result

The 4:1 Multiplexer successfully selects one of the four input signals according to the select inputs.
