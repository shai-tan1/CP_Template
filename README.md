<h1 align="center">⚡ The shai_tan C++ CP Template ⚡</h1>

<p align="center">
  <strong>A battle-tested, highly optimized C++ template for dominating Codeforces, CodeChef, and LeetCode.</strong>
</p>

<p align="center">
  <code>fastio()</code> • <code>PBDS</code> • <code>Sparse Table</code> • <code>Combinatorics</code>
</p>

---

## 🚀 Overview

This repository contains my personal C++ template used for competitive programming. It is built for speed, rapid prototyping, and flawless local debugging without risking Time Limit Exceeded (TLE) errors on judging servers.

## 🛠️ The Arsenal (Key Features)

### 1. Robust Local Debugging
No more polluted standard outputs. The custom `debug(x)` macro securely pipes beautifully formatted vectors, maps, sets, and pairs directly to `cerr`. 
* **Smart Detection:** Automatically disables itself on judging servers using `#ifndef ONLINE_JUDGE`.
* **Variadic Templates:** Seamlessly handles nested STL containers (e.g., `vector<pair<int, int>>`).

### 2. Policy-Based Data Structures (PBDS)
Includes GCC's `__gnu_pbds` extensions, giving you an out-of-the-box `ordered_set`.
* `find_by_order(k)`: Returns an iterator to the $k$-th smallest element.
* `order_of_key(k)`: Returns the number of items strictly smaller than $k$.

### 3. Comprehensive Math & Number Theory Library
Pre-coded, optimized functions ready to be uncommented when needed:
* **Modular Arithmetic:** Binary exponentiation (`power`) and Modular Multiplicative Inverse.
* **Combinatorics:** $O(N^2)$ precomputation for $nCr$ using Pascal's triangle to handle smaller constraints safely.
* **Primes & Factors:** $O(\sqrt{N})$ primality testing, plus pre-commented Sieve of Eratosthenes (SPF) for $O(\log N)$ prime factorization.
* **Bitwise Operations:** $O(1)$ Range Bitwise XOR and Range Bitwise AND algorithms.

### 4. Range Queries
* **Sparse Table:** Pre-commented $O(N \log N)$ build and $O(1)$ query setup for Range Maximum/Minimum Queries (RMQ).

---

## 💻 Usage

### Setup for Local Testing
To utilize the debugging tools and file I/O, ensure you compile or run your code with the local environment flag, or simply uncomment `fropen()` inside `main()` if you prefer reading from `input.txt` and writing to `output.txt`.

```cpp
// Example of local debugging
vector<int> arr = {1, 2, 3};
debug(arr); // Outputs to stderr: arr [ 1 2 3 ]
```
Activating SnippetsThe main() function contains highly useful, commented-out blocks for common CP patterns.
Simply uncomment the required block:
Need prime factors? Uncomment the spf block.
Need $O(1)$ range maximums? Uncomment the SPARSE_TABLE block and paste it into solve().

Developed by <b>Shaunak Samanta</b> (<code>shai_tan</code> / <code>shai_tan-</code> / <code>shai-tan1</code>)</p>
<i>tan(pi/2) = infinite</i>
