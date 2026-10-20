# Digital_Design_1_Group_2

Group Members
* **Member 1:** Ibrahim Nasser Al-Sawmhi 
* **Member 2:** Anas Hussein Babutain
* **Member 3:** 

# Quine-McCluskey Logic Minimization

## Project Description
A C/C++ program that implements the **Quine-McCluskey algorithm** to minimize Boolean functions with up to 20 variables. The program reads Boolean functions from a text file, validates the input, and generates minimized expressions.

## Features
- Read and validate Boolean functions from an input file.
- Support minterms, maxterms, and don't-care terms.
- Generate and display all prime implicants (PIs).
- Identify essential prime implicants (EPIs).
- Solve the prime implicant table and find all possible minimized expressions.
- Convert minimized expressions into NAND-only implementations.
- **Bonus:** Generate Verilog modules using Verilog primitives.
- Handle invalid inputs and report errors.

## Input Format
The input file must contain three lines:

1. Number of variables.
2. Minterms (`m`) or maxterms (`M`), separated by commas.
3. Don't-care terms (`d`), separated by commas.

**Example:**
```text
3
m1,m3,m6,m7
d0,d5
```

This represents a Boolean function with 3 variables, minterms 1, 3, 6, and 7, and don't-care terms 0 and 5.

## Project Structure
```text
Quine-McCluskey/
├── src/          # Source code
├── tests/        # Test cases
├── README.md     # Project documentation
└── report.pdf    # Project report
```

## Building and Running
Build instructions and usage examples will be added here.

## Testing
The program will be tested using 10 test cases covering the main features, including input validation, prime implicant generation, minimization, and NAND-only conversion.

## Team Contributions
Each group member's contributions will be documented in the project report.

## Development
The project is developed collaboratively using GitHub for version control and tracking progress.
