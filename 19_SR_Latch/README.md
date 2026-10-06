# SR Latch

## Overview

An SR Latch is a basic sequential logic circuit used to store one bit of information.

SR stands for Set-Reset. The output changes according to the Set (S) and Reset (R) inputs and retains its previous state when both inputs are inactive.

## Inputs

- S - Set input
- R - Reset input

## Outputs

- Q - Main output
- Qbar - Complementary output

## Truth Table

| S | R | Q | Qbar | Operation |
|---|---|---|------|-----------|
| 0 | 0 | Q | Qbar | Hold |
| 0 | 1 | 0 | 1 | Reset |
| 1 | 0 | 1 | 0 | Set |
| 1 | 1 | X | X | Invalid |

## Verilog Implementations

The SR Latch is implemented using three Verilog modeling styles:

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `sr_latch_structural.v` - Structural Verilog implementation
- `sr_latch_dataflow.v` - Dataflow Verilog implementation
- `sr_latch_behavioral.v` - Behavioral Verilog implementation
- `tb_sr_latch.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The SR Latch was verified using a Verilog testbench and Vivado simulation by testing Set, Reset, Hold, and Invalid conditions.

## Result

The SR Latch successfully stores one bit of information and responds correctly to Set and Reset inputs.
