# Ohm's Law Calculator

## Purpose

This program is a simple terminal-based Ohm's Law calculator. It reads a voltage in volts and a resistance in ohms and calculates the current using:

I = V / R

## Input Format

The program expects two numeric values separated by a space.

The first value is the voltage in volts.

The second value is the resistance in ohms.

Example:

12 4

## Output

For valid input:

Current: 3 A

For invalid input or a resistance that is zero or negative:

Invalid input

## Build

Compile the program with:

g++ -std=c++17 -Wall -Wextra -pedantic src/main.cpp -o build/app

## Run

Run the program with:

./build/app

Then enter the voltage and resistance.

Example:

12 4

Output:

Current: 3 A

## Testing

Run all acceptance tests with:

bash test.sh

A successful test should print:

All acceptance tests passed

## Limitations

The program only calculates current using Ohm's Law. Resistance must be greater than zero, and both inputs must be numeric.

## Debugging Reflection

One important part of debugging was making sure invalid input was handled correctly. The program checks whether both values can be read and whether resistance is greater than zero before performing the division. This prevents division by zero and prevents invalid text input from being used in the calculation.
