# Unexpected String Concatenation in JavaScript

This repository demonstrates a common, yet often surprising, JavaScript behavior: type coercion during arithmetic operations.

## The Bug

The `foo` function intends to add two numbers. However, when one operand is a string, JavaScript implicitly converts the number to a string and performs string concatenation instead of numerical addition. This leads to unexpected results.

## The Solution

The solution involves explicitly converting the operands to numbers before the addition using `parseInt()` or `Number()` to ensure the desired numerical addition is performed.