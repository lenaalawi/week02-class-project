# Ohm's Law Calculator

## Purpose: A C++ terminal program that reads a voltage and a resistance
and prints the current in amps using I = V / R.

## Input Format: Two numbers separated by whitespace: voltage, then resistance.

    12 4

## Build and Run: g++ -std=c++17 -Wall -Wextra -pedantic src/main.cpp -o build/app
    ./build/app

Run the acceptance tests:

    bash test.sh

## Example Output
    $ echo "12 4" | ./build/app
    Current: 3 A

    $ echo "12 0" | ./build/app
    Invalid input

## Limitations
- Only reads two numbers; any extra input is ignored.
- Prints "Invalid input" for non-numeric input or a resistance of zero or below,
  without saying which one was wrong.
- Output uses default C++ precision (about 6 significant digits).
- Negative voltages are accepted.

## Debugging Reflection: One issue I had was that I did not have a SSH key at first, so I was not able to connect my code to my Github. Additionally, there were a lot of small errors throughtout I had to work through, but it worked out in the end. 
