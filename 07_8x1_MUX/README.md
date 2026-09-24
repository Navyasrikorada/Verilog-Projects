# 8:1 Multiplexer (MUX)

## Overview

An 8:1 Multiplexer is a combinational logic circuit that selects one of eight input signals and forwards the selected input to the output using three select lines.

## Inputs

- I0 - Input 0
- I1 - Input 1
- I2 - Input 2
- I3 - Input 3
- I4 - Input 4
- I5 - Input 5
- I6 - Input 6
- I7 - Input 7
- S0 - Select input
- S1 - Select input
- S2 - Select input

## Output

- Y - Selected output

## Truth Table

| S2 | S1 | S0 | Y  |
|----|----|----|----|
| 0  | 0  | 0  | I0 |
| 0  | 0  | 1  | I1 |
| 0  | 1  | 0  | I2 |
| 0  | 1  | 1  | I3 |
| 1  | 0  | 0  | I4 |
| 1  | 0  | 1  | I5 |
| 1  | 1  | 0  | I6 |
| 1  | 1  | 1  | I7 |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `mux8x1_structural.v` - Structural Verilog implementation
- `mux8x1_dataflow.v` - Dataflow Verilog implementation
- `mux8x1_behavioral.v` - Behavioral Verilog implementation
- `tb_mux8x1.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 8:1 Multiplexer was verified using a Verilog testbench and Vivado simulation by testing all possible select combinations.

## Result

The 8:1 Multiplexer successfully selects one of the eight input signals according to the three select inputs.
