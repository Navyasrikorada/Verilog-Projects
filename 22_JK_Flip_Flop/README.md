# JK Flip-Flop

## Overview

A JK Flip-Flop is a sequential logic circuit used to store one bit of information. It is an improved version of the SR Flip-Flop because it eliminates the invalid input condition.

The JK Flip-Flop has two inputs, J and K, and operates based on the active edge of the clock.

## Inputs

- `J` - Set input
- `K` - Reset input
- `CLK` - Clock input

## Output

- `Q` - Stored output
- `Qbar` - Complementary output

## Truth Table

| CLK | J | K | Q(next) | Operation |
|---|---|---|---|---|
| Rising edge | 0 | 0 | Q | Hold |
| Rising edge | 0 | 1 | 0 | Reset |
| Rising edge | 1 | 0 | 1 | Set |
| Rising edge | 1 | 1 | Qbar | Toggle |

## Working Principle

- When `J = 0` and `K = 0`, the output retains its previous state.
- When `J = 0` and `K = 1`, the output resets to 0.
- When `J = 1` and `K = 0`, the output sets to 1.
- When `J = 1` and `K = 1`, the output toggles to the opposite state at the active clock edge.

## Verilog Implementations

This project includes three Verilog modeling styles:

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `jk_flip_flop_structural.v` - Structural implementation
- `jk_flip_flop_dataflow.v` - Dataflow implementation
- `jk_flip_flop_behavioral.v` - Behavioral implementation
- `tb_jk_flip_flop.v` - Testbench for verification
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The JK Flip-Flop is verified using a Verilog testbench by testing Hold, Reset, Set, and Toggle operations at the rising edge of the clock.

## Result

The JK Flip-Flop performs all four operations correctly and stores one bit of information according to the input conditions and clock edge.
