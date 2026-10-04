# Parity Generator

## Overview

A Parity Generator is a combinational logic circuit used to generate an additional parity bit for a given binary data word.

The parity bit is generated to make the total number of 1s either even or odd, depending on the type of parity.

This project implements an Even Parity Generator.

## Inputs

- D[3:0] - 4-bit input data

## Output

- Parity - Generated even parity bit

## Working Principle

For even parity, the parity bit is generated using XOR of all input bits.

If the number of 1s in the input data is odd, the parity bit becomes 1 to make the total number of 1s even.

If the number of 1s is already even, the parity bit becomes 0.

## Truth Table

| D3 | D2 | D1 | D0 | Parity |
|----|----|----|----|--------|
| 0  | 0  | 0  | 0  |   0    |
| 0  | 0  | 0  | 1  |   1    |
| 0  | 0  | 1  | 0  |   1    |
| 0  | 0  | 1  | 1  |   0    |
| 0  | 1  | 0  | 0  |   1    |
| 0  | 1  | 0  | 1  |   0    |
| 0  | 1  | 1  | 0  |   0    |
| 0  | 1  | 1  | 1  |   1    |
| 1  | 0  | 0  | 0  |   1    |
| 1  | 0  | 0  | 1  |   0    |
| 1  | 0  | 1  | 0  |   0    |
| 1  | 0  | 1  | 1  |   1    |
| 1  | 1  | 0  | 0  |   0    |
| 1  | 1  | 0  | 1  |   1    |
| 1  | 1  | 1  | 0  |   1    |
| 1  | 1  | 1  | 1  |   0    |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `parity_generator_structural.v` - Structural Verilog implementation
- `parity_generator_dataflow.v` - Dataflow Verilog implementation
- `parity_generator_behavioral.v` - Behavioral Verilog implementation
- `tb_parity_generator.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The Parity Generator was verified using a Verilog testbench and Vivado simulation by testing all possible 4-bit input combinations.

## Result

The Parity Generator successfully generates the required even parity bit for the given 4-bit input data.
