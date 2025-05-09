# 2-Bit ALU Circuit (Logisim)

## Overview

This project implements a 2-bit ALU (Arithmetic Logic Unit) using [Logisim](http://www.cburch.com/logisim/). The ALU performs four basic arithmetic operations on two 2-bit inputs: addition, subtraction, multiplication, and remainder (modulo). The operation is selected via a 2-bit control input.

## Features

- **Inputs:**
  - `A` (2-bit): First operand
  - `B` (2-bit): Second operand
  - `S1, S0` (2-bit selector): Chooses the operation
    - `00`: Addition
    - `01`: Subtraction
    - `10`: Multiplication
    - `11`: Remainder (Modulo)

- **Outputs:**
  - `F3–F0` (4-bit): Result displayed on a 7-segment display
  - `Zero_Flag`: Set if the result is zero
  - `Div_by_Zero`: Set if remainder operation is attempted with B = 0
  - `Sign_Flag`: Set if the result is negative (for subtraction only)

## File

- `aae34b24-3aab-4675-9176-18ec6cc48b8d.circ`: Logisim circuit file for the ALU

## Requirements

- Logisim or Logisim Evolution
- Basic knowledge of digital logic design

## How to Use

1. Open the `.circ` file in Logisim.
2. Set inputs A, B, S1, and S0 using input pins or toggles.
3. Observe the result on the 7-segment display.
4. Check the status of the output flags.

## Notes

- All operations are limited to 2-bit inputs.
- Remainder operation includes division-by-zero protection.
- Negative results are interpreted in 2's complement where applicable.

## License

This project is for educational use only.
