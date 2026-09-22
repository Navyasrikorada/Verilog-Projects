# 2:1 Multiplexer (MUX)

## Overview

A 2:1 Multiplexer is a combinational logic circuit that selects one of two input signals and forwards the selected input to the output based on the select signal.

## Inputs

- I0 - Input 0
- I1 - Input 1
- S - Select input

## Output

- Y - Selected output

## Truth Table

| S | Y |
|---|---|
| 0 | I0 |
| 1 | I1 |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files
- `mux2x1_behavioral.v` - Behavioral Verilog implementation
- `tb_mux2x1.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The 2:1 Multiplexer was verified using a Verilog testbench and Vivado simulation.

## Result

The 2:1 Multiplexer successfully selects one of the two input signals based on the select input.
