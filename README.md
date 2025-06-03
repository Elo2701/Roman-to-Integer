# Roman to Integer Converter

This Java program converts a Roman numeral string into its corresponding integer value.

## Overview

Roman numerals are represented by seven different symbols:

| Symbol | Value |
|--------|-------|
| I      | 1     |
| V      | 5     |
| X      | 10    |
| L      | 50    |
| C      | 100   |
| D      | 500   |
| M      | 1000  |

The program processes the Roman numeral from right to left, adding or subtracting values based on Roman numeral rules:
- If a smaller value precedes a larger value, subtract the smaller value.
- Otherwise, add the value.

## How It Works

- Uses a `HashMap` to store Roman characters and their integer values.
- Iterates over the string from the end.
- Keeps track of the previous value to decide whether to add or subtract the current value.
- Returns the total integer value.

## Usage

```java
Solution solution = new Solution();
int result = solution.romanToInt("MCMXCIV");  // Returns 1994
