# Mutation Testing in Python

## Overview
This project demonstrates the concept of **mutation testing**, a software testing technique that deliberately introduces small changes (mutants) into source code to evaluate how well a test suite can detect faults. The goal is to assess and improve test quality by measuring how effectively tests “kill” the introduced mutants.

## What It Does
- Applies defined mutation operators to the `Polynomial` class
- Generates mutant versions of code (e.g., modified coefficients, altered logic)
- Runs the test suite against each mutant
- Reports which mutations were detected (“killed”) and which survived

## Files & Structure
- `original/` — Original `Polynomial` implementation
- `mutants/` — Mutated versions of the original code
- `tests/` — Unit tests to check behavior against different mutations
- `README.md` — This documentation

## Skills Demonstrated
- Understanding of mutation testing as a technique in software quality assurance
- Python programming and test automation
- Designing mutation operators to simulate realistic faults
- Evaluating test suite effectiveness

## Running It
1. Clone the repo  
   ```bash
   git clone https://github.com/chazdj/MutationTesting.git
   ```
2. Navigate into the directory  
   ```bash
   cd MutationTesting
   ```
3. Run the provided tests (e.g., using pytest) 
   ```bash
   pytest
   ```

## What I Learned
- Mutation testing reveals weaknesses in tests that code coverage alone might miss.
- Designing meaningful mutation operators requires understanding of both code logic and test assumptions.
- Interpreting mutant survival vs. killing helps plan stronger test cases
   
## Recommendations for Improving the Test Suite
1. **Edge Case Testing**: Implement tests for extreme values of polynomial coefficients, including very large/small integers, to catch edge logic faults.

2. **Parameter Sensitivity Testing**: Test changes to parameters like `epsilon` across a wide range of values to ensure fault detection.

3. **Increase Redundancy Detection**: Introduce targeted test cases that check for side effects caused by redundant operations or logic missteps.

4. **Expand Test Scenarios for Arithmetic Logic**: Test additional combinations of operations and sequences in polynomial addition, subtraction, and multiplication.

5. **Improve Input-Output Coverage**: Enhance testing to explore all input combinations, particularly ones near boundary values or undefined inputs.

## Author
Created by **Chastidy Joanem**  
GitHub: [@chazdj](https://github.com/chazdj)
