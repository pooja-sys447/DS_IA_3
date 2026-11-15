# Data Structures Internal Activity 3

## Project Title
Personalized Hash Table Implementation Using Division Method and Linear Probing

## Student Details
- **PRN:** 202602100017
- **Subject:** Data Structures
- **Programming Language:** C++

## Project Description

This project implements a hash table using the Division Method and Linear Probing for collision handling.

The project uses a personalized dataset generated according to the student's PRN. It demonstrates how hashing maps keys to table indices and how linear probing resolves collisions.

## Personalized Dataset

PRN last four digits (S) = **17**

The dataset is generated using:

`v[i] = (S + 13 * i) mod 100`

**Dataset:**

`17, 30, 43, 56, 69, 82, 95, 8, 21, 34, 47, 60, 73, 86, 99, 12, 25, 38, 51, 64`

## Hashing Details

- **Hashing technique:** Division Method
- **Collision handling:** Linear Probing
- **Table size:** 10 (implementation assumption; confirm with faculty)
- **Programming language:** C++

**Hash function:**

`h(key) = key mod 10`

## Project Files

- `README.md`: Project overview and documentation.
- `hash_table.cpp`: C++ implementation.
- `output.txt`: Actual program output.
- `trace_report.md`: Manual trace and output comparison.
- `debugging_log.md`: Development and debugging records.

## Expected Learning Outcomes

1. Understand the Division Method of hashing.
2. Implement a hash table in C++.
3. Handle collisions using Linear Probing.
4. Compare manual calculations with actual program output.
5. Understand incremental project development.