# D Latch

## Overview

A D Latch is a basic sequential logic circuit used to store one bit of data.

D stands for Data. The output follows the input D when the Enable (EN) signal is active. When Enable is inactive, the latch holds its previous state.

## Inputs

- D - Data input
- EN - Enable input

## Outputs

- Q - Main output
- Qbar - Complementary output

## Truth Table

| EN | D | Q | Operation |
|----|---|---|-----------|
| 0 | X | Q | Hold |
| 1 | 0 | 0 | Reset / Store 0 |
| 1 | 1 | 1 | Set / Store 1 |

## Working

- When `EN = 1`, the output `Q` follows the input `D`.
- When `EN = 0`, the output retains its previous value.
- Therefore, the D Latch can store one bit of information.

## Verilog Implementations

The D Latch is implemented using three Verilog modeling styles:

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `d_latch_structural.v` - Structural Verilog implementation
- `d_latch_dataflow.v` - Dataflow Verilog implementation
- `d_latch_behavioral.v` - Behavioral Verilog implementation
- `tb_d_latch.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The D Latch was verified using a Verilog testbench and Vivado simulation by testing Enable, Data, and Hold conditions.

## Result

The D Latch successfully stores one bit of data and allows the output to follow the input when the Enable signal is active.
