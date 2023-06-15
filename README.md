
# Chudnovsky Algorithm for Computing Pi using GMP

This repository contains an optimized implementation of the Chudnovsky algorithm in the C programming language, leveraging the GNU Multiple Precision Arithmetic Library (GMP) to compute the digits of π (pi) with high precision.

## Requirements

- C compiler (e.g., GCC)
- GNU Multiple Precision Arithmetic Library (GMP)

## Installation

1. Ensure that you have a C compiler installed on your system. If not, install a suitable one for your operating system.

2. Download and install the GNU Multiple Precision Arithmetic Library (GMP) from the official website or your system's package manager.

## Usage

1. Clone this repository to your local machine:

   ```
   git clone https://github.com/your-username/chudnovsky-pi-gmp.git
   ```

2. Navigate to the project directory:

   ```
   cd chudnovsky-pi-gmp
   ```

3. Compile the source code using GCC and link the GMP library:

   ```
   gcc chudnovsky.c -o chudnovsky -lgmp
   ```

4. Run the compiled executable:

   ```
   ./chudnovsky
   ```

   The program will calculate and print the value of π (pi) with the desired number of decimal places.

## Configuration

You can adjust the precision of the calculated pi by modifying the `digits` variable in the `main` function of `chudnovsky.c`. This value represents the number of decimal places to compute.

## Optimization

The Chudnovsky algorithm implementation in this repository has been optimized for efficiency. Here are the key optimizations applied:

- Higher precision usage: The GMP library is initialized with a precision value twice the number of digits required. This helps prevent precision loss during calculations.

- Reduction of redundant computations: The temporary variable `temp` is utilized to store the difference between `ck` and `dk` in each iteration, minimizing the need for recalculating the same expression multiple times.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- The Chudnovsky algorithm is a highly efficient method for computing pi and was developed by the Chudnovsky brothers: David Chudnovsky and Gregory Chudnovsky.

- The GNU Multiple Precision Arithmetic Library (GMP) provides a robust and efficient way to perform arithmetic operations with arbitrary precision.

- This implementation is based on the original Chudnovsky algorithm and the GMP library documentation.
