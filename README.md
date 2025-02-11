# CS341L Spring 2025 - Data Lab: Manipulating Bits

## Assigned: Feb. 10th  
## Due: Mar. 2nd, 11:59 PM

### Introduction
The goal of this assignment is to deepen your understanding of bit-level representations of integers and floating-point numbers by solving a series of programming puzzles. These puzzles will challenge you to think critically about bit manipulation in C.

### Logistics
- This is an individual assignment.
- All submissions are through Canvas.
- You may discuss strategies verbally but cannot share code.
- If you discuss solutions, document it in a `CREDITS` file.
- Any external sources consulted must be noted in `CREDITS`.

### Handout Instructions
- The source files are provided in a tarball on Canvas.
- Modify only `bits.c`.
- If you received external help, submit a `CREDITS` file.
- Using version control (GitHub, Lobogit, etc.) is recommended.

### The Puzzles
#### 1. Bit Manipulations
| Function | Description | Rating | Max Ops |
|----------|-------------|--------|---------|
| `bitCount(x)` | Counts the number of 1s in `x`. | 4 | 40 |
| `bitNor(x, y)` | Computes `~(x | y)` using only `~` and `&`. | 1 | 8 |
| `byteSwap(x, n, m)` | Swaps the `n`th and `m`th byte of `x`. | 2 | 25 |
| `isAsciiDigit(x)` | Checks if `x` is an ASCII digit. | 3 | 15 |

#### 2. Two’s Complement Arithmetic
| Function | Description | Rating | Max Ops |
|----------|-------------|--------|---------|
| `isPositive(x)` | Checks if `x > 0`. | 3 | 8 |

#### 3. Floating-Point Operations
| Function | Description | Rating | Max Ops |
|----------|-------------|--------|---------|
| `float_abs(uf)` | Computes the absolute value of `uf`. | 2 | 10 |
| `float_neg(uf)` | Computes `-f`. | 2 | 10 |
| `ezThreeFourths(x)` | Multiplies `x` by 3/4 and rounds to 0. | 3 | 12 |

### Evaluation
- **Correctness (20 pts):** Based on passing `btest`.
- **Performance (16 pts):** Must meet operator limits.
- **Explanation & Style (40 pts):** Solutions must be well-commented and clearly written.

### Autograding Tools
- `btest`: Tests functional correctness.
- `dlc`: Checks compliance with coding rules.
- `driver.pl`: Evaluates correctness and performance.

### Handin Instructions
- Submit `bits.c` and `CREDITS.pdf` via Canvas before the deadline.

### Advice
- Avoid including `<stdio.h>` in `bits.c`.
- Ensure all variable declarations appear before statements.
- Use `btest`, `dlc`, and `driver.pl` frequently to check your work.