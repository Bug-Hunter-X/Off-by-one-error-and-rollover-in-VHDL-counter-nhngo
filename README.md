# VHDL Counter Bug
This repository demonstrates a common error in VHDL code: an off-by-one error in a counter and the lack of rollover handling. The `bug.vhdl` file contains the buggy code. The `bugSolution.vhdl` file provides a corrected version.

## Bug Description
The original counter code suffers from two issues:

1. **Off-by-one error:**  The counter may not reach its maximum value before resetting.
2. **No rollover handling:** Once the counter reaches its maximum value, the behavior is undefined. 

## Solution
The corrected version addresses both issues. It ensures the counter correctly reaches the maximum value and then wraps around to zero.

## How to reproduce
1.  Synthesize and simulate both `bug.vhdl` and `bugSolution.vhdl` using your preferred VHDL simulator (e.g Modelsim).
2. Observe the differences in the counter's behavior.
