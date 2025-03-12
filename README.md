# ALU-Design-using-SystemC
This project implements a Multi-Function Arithmetic Logic Unit (ALU) in Verilog, designed to perform a wide range of arithmetic and logical operations. The ALU takes two operands (A and B), a function selector (func), and a carry-in (Cin) to produce a result (O) and status flags. It supports operations like addition, subtraction, bitwise logic, comparisons, shifts, multiplication, and division, among others.

Key Features:
Operations Supported:
Addition and Subtraction: Performs basic arithmetic operations (A + B, A - B), including carry-in addition (A + B + Cin).
Comparison: Compares the two inputs A and B for greater than, less than, or equality.
Bitwise Operations: AND, OR, NOT operations between A and B.
Shifts: Supports logical and arithmetic shifts (left and right).
Multiplication and Division: Performs multiplication (A * B) and division (A / B), along with modulo operation (A % B).

Flags:
Zero Flag (Z): Set if the result is zero.
Negative Flag (N): Set if the result is negative.
Carry Flag (C): Set if there’s a carry-out from the operation.
Overflow Flag (V): Always set to 0 in this design (potential for future extension).

How It Works:
The function selector (func) determines which operation to perform.
The result of the operation is computed, and based on the result, the ALU sets the appropriate flags (Z, N, C, V).
The ALU handles all operations in parallel, and the result, along with the flags, is output to the corresponding signals.
