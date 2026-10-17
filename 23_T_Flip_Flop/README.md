# T Flip-Flop

## Overview

A T Flip-Flop is a sequential logic circuit used to store one bit of information. T stands for Toggle.

The output changes to its opposite state when T = 1 at the active clock edge. When T = 0, the output retains its previous state.

This project implements a positive-edge-triggered T Flip-Flop.

## Inputs

- `T` - Toggle input
- `CLK` - Clock input

## Outputs

- `Q` - Main output
- `Qbar` - Complementary output

## Truth Table

| CLK | T | Q(next) | Operation |
|---|---|---|---|
| Rising edge | 0 | Q | Hold |
| Rising edge | 1 | Qbar | Toggle |

## Working Principle

- When `T = 0`, the output remains unchanged at the rising edge of the clock.
- When `T = 1`, the output toggles between 0 and 1 at the rising edge.
- The output does not change between active clock edges.
- T Flip-Flops are commonly used in counters and frequency-divider circuits.

## Verilog Implementations

This project includes three Verilog modeling styles:

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `t_flip_flop_structural.v` - Structural Verilog implementation
- `t_flip_flop_dataflow.v` - Dataflow Verilog implementation
- `t_flip_flop_behavioral.v` - Behavioral Verilog implementation
- `tb_t_flip_flop.v` - Testbench for verification
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The T Flip-Flop is verified using a Verilog testbench and Vivado simulation by testing both Hold and Toggle operations at the rising edge of the clock.

## Result

The T Flip-Flop correctly holds its current state when T = 0 and toggles its output when T = 1 at the rising edge of the clock.
