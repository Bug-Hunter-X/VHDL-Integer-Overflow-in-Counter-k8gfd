# VHDL Integer Overflow Bug
This repository demonstrates a common error in VHDL: integer overflow in a counter.  The `buggy_counter.vhd` file contains code for a counter that uses an `integer` type.  This type has a limited range and, if the counter exceeds this range, it results in overflow, leading to unpredictable behavior.

The `fixed_counter.vhd` file provides a corrected version using `unsigned` type, which avoids the overflow issue and provides a more robust solution.

**To reproduce the bug:**
1. Simulate `buggy_counter.vhd`. Observe the unexpected behavior when the counter reaches its maximum value.
2. Simulate `fixed_counter.vhd`. Note the correct, expected behavior.