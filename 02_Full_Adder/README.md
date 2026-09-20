# Full Adder

## Overview
A Full Adder is a combinational logic circuit that adds three 1-bit binary inputs and produces Sum and Carry outputs.

## Inputs
- A
- B
- Cin (Carry-in)

## Outputs
- Sum
- Cout (Carry-out)

## Verilog Implementations
- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Truth Table

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
| 0 | 0 |  0  |  0  |  0   |
| 0 | 0 |  1  |  1  |  0   |
| 0 | 1 |  0  |  1  |  0   |
| 0 | 1 |  1  |  0  |  1   |
| 1 | 0 |  0  |  1  |  0   |
| 1 | 0 |  1  |  0  |  1   |
| 1 | 1 |  0  |  0  |  1   |
| 1 | 1 |  1  |  1  |  1   |

## Tools Used
- Verilog HDL
- Xilinx Vivado

## Verification
The Full Adder was verified using a Verilog testbench and Vivado simulation waveform.

## Schematic
The design schematic was generated using Xilinx Vivado.
