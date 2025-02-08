# VHDL Counter Overflow Bug

This repository demonstrates a common error in VHDL code: counter overflow. The `buggy_counter.vhdl` file contains a counter that increments without checking for the upper limit of its range. This can lead to unexpected behavior and potentially incorrect results.  The solution, `fixed_counter.vhdl`, addresses this by adding an overflow check.

## Bug Description

The buggy counter increments indefinitely, even after reaching its maximum value (15). This results in counter wrap-around or unpredictable behavior.

## Solution

The fixed counter uses a `mod` operator to ensure that the counter wraps around correctly, preventing overflow.
