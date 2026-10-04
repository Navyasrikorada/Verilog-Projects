# Parity Checker

## Overview

A Parity Checker is a combinational logic circuit used to check whether the received binary data satisfies the required parity condition.

This project implements an Even Parity Checker for 4-bit data with a received parity bit.

## Inputs

- D[3:0] - 4-bit received data
- Parity - Received parity bit

## Output

- Error - Indicates whether a parity error is detected

## Working Principle

For even parity, the total number of 1s in the received data and parity bit should be even.

- `Error = 0` → No parity error
- `Error = 1` → Parity error detected

## Truth Table

| D3 | D2 | D1 | D0 | Parity | Error |
|----|----|----|----|--------|-------|
| 0  | 0  | 0  | 0  |   0    |   0   |
| 0  | 0  | 0  | 1  |   1    |   0   |
| 0  | 0  | 1  | 0  |   1    |   0   |
| 0  | 0  | 1  | 1  |   0    |   0   |
| 0  | 1  | 0  | 0  |   1    |   0   |
| 0  | 1  | 0  | 1  |   0    |   0   |
| 0  | 1  | 1  | 0  |   0    |   0   |
| 0  | 1  | 1  | 1  |   1    |   0   |
| 1  | 0  | 0  | 0  |   1    |   0   |
| 1  | 0  | 0  | 1  |   0    |   0   |
| 1  | 0  | 1  | 0  |   0    |   0   |
| 1  | 0  | 1  | 1  |   1    |   0   |
| 1  | 1  | 0  | 0  |   0    |   0   |
| 1  | 1  | 0  | 1  |   1    |   0   |
| 1  | 1  | 1  | 0  |   1    |   0   |
| 1  | 1  | 1  | 1  |   0    |   0   |

## Verilog Implementations

- Structural Modeling
- Dataflow Modeling
- Behavioral Modeling

## Files

- `parity_checker_structural.v` - Structural Verilog implementation
- `parity_checker_dataflow.v` - Dataflow Verilog implementation
- `parity_checker_behavioral.v` - Behavioral Verilog implementation
- `tb_parity_checker.v` - Testbench
- `waveform.png` - Vivado simulation waveform
- `schematic.png` - Vivado schematic

## Tools Used

- Verilog HDL
- Xilinx Vivado

## Verification

The Parity Checker was verified using a Verilog testbench and Vivado simulation by testing valid and invalid parity combinations.

## Result

The Parity Checker successfully detects parity errors in the received 4-bit data and parity bit.
