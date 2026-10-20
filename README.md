# Digital_Design_1_Group_2

Group Members
* **Member 1:** Ibrahim Nasser Al-Sawmhi 
* **Member 2:** Anas Hussein Babutain
* **Member 3:** 

## Project Description
# Quine-McCluskey Logic Minimizer & Verilog Generator

## Project Overview
This software application implements the **Quine-McCluskey (QM) algorithm** in C/C++ to minimize Boolean functions with up to **20 input variables**. The program parses function specifications from an input text file, identifies all Prime Implicants (PIs) and Essential Prime Implicants (EPIs), solves the PI table for minimal Sum-of-Products (SOP) expressions, converts the output to NAND-only logic, and generates corresponding Verilog structural modules using Verilog primitives.

---

## Key Features
1. **Input File Parsing & Validation:** 
   * Reads 3-line input files containing variable counts, minterms (`m`) or maxterms (`M`), and don't-care terms (`d`).
   * Performs complete input validation and error handling for up to 20 variables.
2. **Prime Implicant (PI) Generation:** 
   * Generates and prints all PIs along with their binary representations and covered minterm/don't-care indices.
3. **Essential Prime Implicant (EPI) Extraction:** 
   * Identifies EPIs, formats them as Boolean expressions, and reports un-covered minterms.
4. **PI Table Reduction & Minimization:** 
   * Solves the PI table to find all minimal Sum-of-Products (SOP) Boolean expressions.
5. **NAND Conversion:** 
   * Converts minimal SOP Boolean expressions to equivalent **NAND-only** expressions.
6. **Verilog Module Generation (Bonus):** 
   * Automatically generates a Verilog module (`.v`) implementing the minimized logic using Verilog gate primitives (`nand`, `and`, `or`, `not`).

---

## Input File Format
The program reads input from a text file with strictly **3 lines**:
1. **Line 1:** Number of input variables ($N \le 20$).
2. **Line 2:** Comma-separated minterms (e.g., `m1,m3,m6,m7`) or maxterms (e.g., `M1,M3,M6,M7`).
3. **Line 3:** Comma-separated don't-care terms (e.g., `d0,d5`).

### Example (`input.txt`)
```text
3
m1,m3,m6,m7
d0,d5
