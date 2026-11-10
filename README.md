# Ohm's Law and Power Calculator

## What it does
The program finds voltage, current, resistance or power from two known values. The user picks what to find, types the known values, and gets the answer with its unit. It keeps running until the user quits, and it rejects bad input such as letters or a zero divisor. After every power calculation, it checks the result against the standard resistor ratings (0.25 W, 0.5 W, 1 W, 2 W) and tells the user the smallest safe rating to use.

## How to run it
Install Python 3, then run: python ohms_law.py

## Sample output
```
=== Ohm's Law and Power Calculator ===

What do you want to find?
  1. Voltage (V)
  2. Current (A)
  3. Resistance (ohm)
  4. Power (W)
  h. Show history
  q. Quit
Choose an option: 4
Enter voltage in volts (V): 4
Enter current in amps (A): 0.2

Answer: Power = 0.8 W
Use at least a 1 W resistor.
...
Goodbye.

--- Calculation history ---
  1. Power = 0.8 W
```

## My own twist
After every power calculation, the program compares the power with the standard resistor ratings and tells the user which rating is safe to use. For example, 0.8 W needs a 1 W resistor, and anything above 2 W gets a warning to use a higher-rated resistor or check the circuit. The history of answers is also shown when the user chooses h and when the program closes.

## What I learned
Checking input before using it stops the program from crashing. Splitting the code into small functions made it easier to test each calculation on its own. Resistors are rated for power, not just resistance, so an overheated resistor can fail even when the value is correct.

## Author
Boluwatife Oyeyiola, ND1 Mechatronics Engineering, YabaTech.
