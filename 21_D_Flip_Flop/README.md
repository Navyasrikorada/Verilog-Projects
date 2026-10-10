# D Flip-Flop

## Overview

A D Flip-Flop is a basic sequential logic circuit used to store one bit of data.

D stands for Data. Unlike a D Latch, a D Flip-Flop changes its output only at the active edge of the clock signal.

This project implements a positive-edge triggered D Flip-Flop.

## Inputs

- D - Data input
- CLK - Clock input

## Outputs

- Q - Main output
- Qbar - Complementary output

## Truth Table

| CLK | D | Q(next) | Operation |
|-----|---|---------|-----------|
| ↑ | 0 | 0 | Store 0 |
| ↑ | 1 | 1 | Store 1 |
| No active edge | X | Q | Hold |

## Working

- The D Flip-Flop is triggered at the rising edge of the clock.
- When `CLK` changes from `0` to `1`, the value of `D` is stored in `Q`.
- Between clock edges, the output remains unchanged.
- Therefore, it can store one bit of information.

## D Flip-Flop vs D Latch

| D Latch | D Flip-Flop |
|----------|-------------|
| Level triggered | Edge triggered |
| Controlled by Enable | Controlled by Clock |
| Output can change while Enable is active | Output changes only at clock edge |
| Simpler storage element | More suitable for synchronous systems |

## Verilog Implementations

The D Flip-Flop is implemented using three Verilog modeling styles:

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `d_flip_flop_structural.v` - Structural Verilog implementation
- `d_flip_flop_dataflow.v` - Dataflow Verilog implementation
- `d_flip_flop_behavioral.v` - Behavioral Verilog implementation
- `tb_d_flip_flop.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The D Flip-Flop was verified using a Verilog testbench and Vivado simulation by applying different data values at the rising edge of the clock.

## Result

The D Flip-Flop successfully stores the input data at the rising edge of the clock and holds the stored value until the next active clock edge.
