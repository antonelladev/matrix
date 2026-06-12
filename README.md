# Computational Mathematics Program (MatComp)

A robust, terminal-based modular C++ application tailored for computational mathematics. This project was collaboratively developed as a final project to demonstrate foundational concepts in Linear Algebra and Discrete Mathematics, implementing all algorithms entirely from scratch.

---

## Project Overview

The primary objective of this program is to compute core mathematical structures without relying on external specialized libraries (such as Eigen, NumPy, or even standard advanced algebraic libraries). Every single row-column operations, matrix property analysis, transposition, and sequence summation loop was written manually to ensure deep algorithmic comprehension.

## Core Features

### 1. Matrix & Linear Algebra Module
* **Matrix Arithmetic:** Safe addition and subtraction checking for structural compatibility, alongside standard cross-product matrix multiplication.
* **Property Analyzer:** Evaluates square matrices to identify specific mathematical structures:
  * Square Matrices
  * Diagonal Matrices
  * Identity Matrices
  * Upper and Lower Triangular Matrices
* **Determinant Calculator:** Manual computational implementation of determinants for $2 \times 2$ and $3 \times 3$ matrices using explicit algorithmic definitions.
* **Transposition:** Fast in-place index inversion to transpose asymmetrical matrices.

### 2. Sequences and Series Module
Generates $N$ arbitrary terms, computes partial sums ($S_n$), and runs an automated behavioral trend analysis for:
* **Arithmetic Sequences:** $a_n = a_1 + (n-1)d$
* **Geometric Sequences:** $a_n = a_1 \cdot r^{n-1}$
* **Fibonacci Series:** Custom initialization with dynamic seed parameters.
* **Perfect Squares:** Perfect integer $n^2$ sequence testing.
* **Harmonic Series:** Sequential fraction generation ($1/n$).
* **Exponential Sequences:** Function structures tracking $a \cdot b^n$.

> **💡 Trend Intelligence:** The program includes basic mathematical evaluation algorithms that read final term differentials to predict whether a sequence converges, diverges to infinity, or remains in an oscillating pattern.

---

## 🎛️ Architecture & Constraints

* **Strictly Native Algebra:** No external solvers. `<cmath>` is intentionally restricted exclusively to absolute value mapping (`fabs()`) and specific base exponents (`pow()`) within sequences.
* **Bulletproof Inputs:** Built-in console stream parsing utility (`limpiarBuffer`) that clears invalid characters and inputs to eliminate infinite looping bugs in the terminal environment.
* **Memory Optimization:** Matrices are handled via memory-efficient dynamic dimensional vectors (`std::vector<std::vector<double>>`).

---

## 📦 Getting Started

### Prerequisites
A working C++ compiler matching standard specifications (GCC, Clang, or MSVC).

### Installation & Execution
1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
   cd YOUR_REPOSITORY_NAME
