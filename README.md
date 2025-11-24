# Python Math & Algorithms Collection

This repository contains a collection of Python scripts implementing various mathematical algorithms, number theory concepts, and sequence generators.

## Files Overview

| File Name | Function/Concept | Description |
| :--- | :--- | :--- |
| `01_q1.py` | **Lucas Sequence** | Generates the first $n$ terms of the Lucas sequence. |
| `01_q2.py` | **Perfect Power** | Checks if $n$ is a perfect power ($m^k$). |
| `01_qa.py` | **Factorial** | Calculates $n!$. |
| `01ques.py` | **Modular Inverse** | Calculates modular multiplicative inverse. |
| `01ques1.py` | **Distinct Prime Factors** | Counts distinct prime factors. |
| `02_qa.py` | **Palindrome** | Checks if a number is a palindrome. |
| `02ques.py` | **Chinese Remainder Theorem** | Solves systems of congruences. |
| `02ques2.py` | **Prime Power** | Checks if $n$ is a prime power ($p^k$). |
| `03_qa.py` | **Mean Calculation** | Calculates the arithmetic mean. |
| `03-q3.py` | **Collatz Conjecture** | Calculates Collatz sequence length. |
| `04_qa.py` | **Digital Root** | Calculates the recursive sum of digits until single digit. |
| `04-q4.py` | **Polygonal Numbers** | Computes the $n$-th $s$-gonal number (triangular, square, etc.). |
| `04ques.py` | **Multiplicative Order** | Finds the smallest $k$ such that $a^k \equiv 1 \pmod n$. |
| `04ques4.py` | **Twin Primes** | Finds all twin prime pairs up to a limit. |
| `05_q5.py` | **Carmichael Number** | Checks if $n$ is a Carmichael number (pseudoprime). |
| `05_qa.py` | **Abundant Number** | Checks if the sum of proper divisors exceeds $n$. |
| `05ques.py` | **Fibonacci Prime** | Checks if a number is both Fibonacci and Prime. |
| `05ques5.py` | **Divisor Count** | Calculates the number of divisors $d(n)$. |
| `assigment 8 py3.py` | **Riemann Zeta** | Approximates the Riemann Zeta function $\zeta(s)$. |
| `assignment 5 py2.py` | **Amicable Numbers** | Checks if two numbers form an amicable pair. |
| `assignment 5 py3.py` | **Multiplicative Persistence** | Steps to reach a single digit by multiplying digits. |
| `assignment 5 py4.py` | **Highly Composite** | Checks if $n$ has more divisors than any smaller integer. |
| `assignment 5 py5.py` | **Modular Exponentiation** | Efficiently computes $b^e \pmod m$. |
| `assignment 5.py` | **Aliquot Sum** | Calculates the sum of proper divisors $s(n)$. |
| `assignment 8 py2.py` | **Pollard's Rho** | Integer factorization algorithm. |
| `assignment 8 py4.py` | **Integer Partitions** | Computes $p(n)$, the number of ways to partition $n$. |
| `assignment 8.py` | **Miller-Rabin** | Probabilistic primality test. |
| `ques1.py` | **Deficient Number** | Checks if sum of proper divisors is less than $n$. |
| `ques2.py` | **Harshad Number** | Checks if $n$ is divisible by the sum of its digits. |
| `ques3.py` | **Automorphic Number** | Checks if $n^2$ ends with the digits of $n$. |
| `ques4.py` | **Pronic Number** | Checks if $n$ is the product of two consecutive integers. |
| `ques5.py` | **Prime Factorization** | Returns a complete list of prime factors (including duplicates). |

## Detailed Descriptions

### Number Theory & Algebra

#### 1. Modular Arithmetic & Congruences

* **Modular Inverse (`01ques.py`):** Uses Extended Euclidean Algorithm to find $x$ where $ax \equiv 1 \pmod m$.
* **Chinese Remainder Theorem (`02ques.py`):** Solves a system of linear congruences given pairwise coprime moduli.
* **Multiplicative Order (`04ques.py`):** Calculates the order of $a$ modulo $n$, the smallest positive integer $k$ such that $a^k \equiv 1 \pmod n$. Requires $\gcd(a, n) = 1$.
* **Modular Exponentiation (`assignment 5 py5.py`):** Computes $base^{exp} \pmod{modulus}$ efficiently using binary exponentiation (repeated squaring), essential for cryptography.

#### 2. Primes & Factorization

* **Miller-Rabin Primality Test (`assignment 8.py`):** A probabilistic algorithm to determine if a number is composite or probably prime. Faster than trial division for large numbers.
* **Pollard's Rho Algorithm (`assignment 8 py2.py`):** A probabilistic algorithm for integer factorization. Effective for finding small non-trivial factors of composite numbers.
* **Prime Factorization (`ques5.py`):** Decomposes an integer into its constituent prime factors (e.g., $24 \to [2, 2, 2, 3]$).
* **Distinct Prime Factors (`01ques1.py`):** Counts unique prime factors of an integer.
* **Prime Power Checker (`02ques2.py`):** Determines if $n = p^k$ for prime $p$.
* **Twin Primes (`04ques4.py`):** Uses the Sieve of Eratosthenes to find pairs of primes $(p, p+2)$.
* **Carmichael Number (`05_q5.py`):** Identifies Carmichael numbers (composite numbers $n$ that satisfy $b^{n-1} \equiv 1 \pmod n$ for all $b$ coprime to $n$).

#### 3. Divisors & Special Integers

* **Divisor Count (`05ques5.py`):** Calculates total number of divisors $d(n)$.
* **Aliquot Sum (`assignment 5.py`):** Computes $s(n)$, the sum of proper divisors of $n$. Used to classify numbers as perfect, abundant, or deficient.
* **Highly Composite Numbers (`assignment 5 py4.py`):** Determines if $n$ is a highly composite number (a number having more divisors than any positive integer smaller than it).
* **Abundant Number (`05_qa.py`):** Checks if $s(n) > n$.
* **Deficient Number (`ques1.py`):** Checks if $s(n) < n$ (the sum of proper divisors is less than the number itself).
* **Amicable Numbers (`assignment 5 py2.py`):** Checks if two numbers form a pair where $s(a) = b$ and $s(b) = a$.
* **Pronic Number (`ques4.py`):** Checks if $n$ can be expressed as the product of two consecutive integers, $n = k(k+1)$ (also called rectangular numbers).

### Sequences & Combinatorics

#### 4. Classical Sequences & Properties

* **Lucas Sequence (`01_q1.py`):** Generates terms where $L_n = L_{n-1} + L_{n-2}$ starting with 2, 1.
* **Fibonacci Prime (`05ques.py`):** Determines if a number exists in the Fibonacci sequence AND is a prime number.
* **Collatz Sequence (`03-q3.py`):** Calculates the stopping time (steps to reach 1) for the Collatz map $n \to n/2$ (even) or $3n+1$ (odd).
* **Integer Partitions (`assignment 8 py4.py`):** Calculates $p(n)$, the number of distinct ways $n$ can be represented as a sum of natural numbers, using Euler's pentagonal number theorem recurrence.

#### 5. Geometric & Analytic

* **Polygonal Numbers (`04-q4.py`):** Computes the $n$-th number for an $s$-sided polygon (e.g., $s=3$ is triangular). Formula: $\frac{(s-2)n^2 - (s-4)n}{2}$.
* **Riemann Zeta Approximation (`assigment 8 py3.py`):** Approximates the value of the Riemann Zeta function $\zeta(s) = \sum_{n=1}^{\infty} \frac{1}{n^s}$ using a partial sum.

### Basic Utilities & Digits

* **Harshad Number (`ques2.py`):** Checks if a number is divisible by the sum of its digits (also known as Niven numbers).
* **Automorphic Number (`ques3.py`):** Checks if the square of a number ends with the digits of the number itself (e.g., $5^2 = 25$).
* **Multiplicative Persistence (`assignment 5 py3.py`):** Calculates the number of steps required to reduce a number to a single digit by multiplying its digits repeatedly.
* **Digital Root (`04_qa.py`):** Recursively sums the digits of a number until a single digit remains (equivalent to $n \pmod 9$, with exception for 0).
* **Palindrome Checker (`02_qa.py`):** Checks if a number reads the same backwards.
* **Factorial (`01_qa.py`):** Computes $n!$.
* **Mean of Digits (`03_qa.py`):** Computes the arithmetic mean of a list of numbers.

## Requirements

* Python 3.x

## How to Run

Run any file individually via the command line:

```bash
python "assignment 8.py"
python ques2.py
