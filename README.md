```markdown
# Chudnovsky Algorithm for Calculating Pi using GMP

This repository contains an optimized implementation of the Chudnovsky algorithm in C programming language, using the GNU Multiple Precision Arithmetic Library (GMP) to calculate the digits of π (pi) with high precision.

## Requirements

- C compiler (e.g., GCC)
- GNU Multiple Precision Arithmetic Library (GMP)

## Installation

1. Ensure that you have a C compiler installed on your system. If not, install one suitable for your operating system.

2. Download and install the GNU Multiple Precision Arithmetic Library (GMP) from the official website or your system's package manager.

## Usage

1. Clone this repository to your local machine:

   ```
   git clone https://github.com/your-username/chudnovsky-pi-gmp.git
   ```

2. Change into the project directory:

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

   The program will compute and print the value of π (pi) with the desired number of decimal places.

## Configuration

You can adjust the precision of the calculated pi by modifying the `digits` variable in the `main` function of `chudnovsky.c`. The value represents the number of decimal places to compute.

## Optimization

The implementation of the Chudnovsky algorithm in this repository has been optimized for efficiency. Here are some key optimizations employed:

- Use of higher precision: The GMP library is initialized with a precision value twice the number of digits required. This helps avoid precision loss during calculations.

- Reduction of redundant calculations: The temporary variable `temp` is used to store the difference between `ck` and `dk` in each iteration, reducing the need to recalculate the same expression multiple times.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- The Chudnovsky algorithm is a highly efficient method for calculating pi and was developed by the Chudnovsky brothers: David Chudnovsky and Gregory Chudnovsky.

- The GNU Multiple Precision Arithmetic Library (GMP) provides a robust and efficient way to perform arithmetic operations with arbitrary precision.

- This implementation is based on the original Chudnovsky algorithm and the GMP library documentation.
```
