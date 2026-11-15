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
## Algorithm

1. Initialize all hash table buckets as empty.
2. Read the 20 personalized cold-drink flavour values.
3. Calculate the square of each key.
4. Extract the middle digits from the squared value according to the selected Mid-Square convention.
5. Calculate the hash index using the extracted digits modulo the table size.
6. Check whether the calculated bucket is empty.
7. If the bucket is occupied, use Separate Chaining to insert the new value into the existing linked list.
8. Repeat until all 20 values are inserted.
9. Display the final hash table with all buckets and their linked values.

## Compilation and Execution

Compile the program using:

```bash
g++ hash_table.cpp -o hash_table
```

Execute the program:

```bash
./hash_table
```

For Windows:

```bash
hash_table.exe
```

## Time Complexity

- Average insertion: O(1), assuming a reasonable distribution of keys.
- Worst-case insertion: O(n) if all keys are mapped to the same bucket.
- Display operation: O(m + n), where m is the table size and n is the number of stored values.

## Final Result

The project demonstrates the implementation of a personalized hash table using the Mid-Square hashing technique and Separate Chaining for collision handling. It stores 20 personalized cold-drink flavour values generated using PRN 202602100017.
