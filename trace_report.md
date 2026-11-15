# TRACE REPORT

## 1. Student Details

- PRN: 202602100017
- Subject: Data Structures
- Project: Hash Table Implementation
- Scenario: Mango Varieties

## 2. Personalized Dataset

Last four digits of PRN:

S = 17

Dataset formula:

`v[i] = (S + 13 × i) mod 100`

Personalized dataset:

`17, 30, 43, 56, 69, 82, 95, 8, 21, 34, 47, 60, 73, 86, 99, 12, 25, 38, 51, 64`

## 3. Hashing Technique

Division Method:

`h(key) = key mod 23`

Table size = 23 (chosen implementation assumption).

## 4. Collision Handling

Linear Probing is used to resolve collisions.

If a calculated index is already occupied, the next available index is checked.

Formula:

`hᵢ(key) = (h(key) + i) mod 23`

## 5. Manual Insertion Trace

| Key | Initial Index | Final Index |
|---:|---:|---:|
| 17 | 17 | 17 |
| 30 | 7 | 7 |
| 43 | 20 | 20 |
| 56 | 10 | 10 |
| 69 | 0 | 0 |
| 82 | 13 | 13 |
| 95 | 3 | 3 |
| 8 | 8 | 8 |
| 21 | 21 | 21 |
| 34 | 11 | 11 |
| 47 | 1 | 1 |
| 60 | 14 | 14 |
| 73 | 4 | 4 |
| 86 | 17 | 18 |
| 99 | 7 | 9 |
| 12 | 12 | 12 |
| 25 | 2 | 2 |
| 38 | 15 | 15 |
| 51 | 5 | 5 |
| 64 | 18 | 19 |

## 6. Final Hash Table

| Index | Value |
|---:|---:|
| 0 | 69 |
| 1 | 47 |
| 2 | 25 |
| 3 | 95 |
| 4 | 73 |
| 5 | 51 |
| 6 | EMPTY |
| 7 | 30 |
| 8 | 8 |
| 9 | 99 |
| 10 | 56 |
| 11 | 34 |
| 12 | 12 |
| 13 | 82 |
| 14 | 60 |
| 15 | 38 |
| 16 | EMPTY |
| 17 | 17 |
| 18 | 86 |
| 19 | 64 |
| 20 | 43 |
| 21 | 21 |
| 22 | EMPTY |

## 7. Trace-Match Report

The manually calculated final hash table was compared with the expected output produced by the C++ program.

The insertion positions and final table should match exactly.

Collision verification:

- 86: Initial index 17 was occupied, so it was inserted at index 18.
- 99: Initial index 7 was occupied. Index 8 was also occupied, so it was inserted at index 9.
- 64: Initial index 18 was occupied, so it was inserted at index 19.

All 20 values were successfully inserted without any data loss.

## 8. Conclusion

The program successfully inserts all 20 personalized values into the hash table. The Division Method calculates the initial index, while Linear Probing resolves collisions by checking subsequent positions.

The manual insertion trace and final hash table demonstrate the correct implementation of hashing and collision handling using Linear Probing in C++.