# DEBUGGING LOG

## Project Details

- PRN: 202602100017
- Project: Personalized Hash Table Implementation
- Language: C++
- Hashing Method: Division Method
- Collision Handling: Linear Probing

### Entry 1: Selecting Table Size

**Problem:** Initially, a table size of 10 was considered.

**Failed Approach:** A table with 10 positions cannot accommodate all 20 distinct values.

**Solution:** Selected a table size of 23 as an implementation choice to accommodate all 20 values.

**Result:** The selected table size provides sufficient capacity.

### Entry 2: Resolving Collision

**Problem:** During manual tracing, value 86 was initially assigned to index 17.

**Failed Approach:** The initial calculation did not account for the fact that index 17 was already occupied by 17.

**Solution:** Applied Linear Probing:

- Initial index = 86 % 23 = 17.
- Index 17 is occupied.
- Checked index 18.
- Index 18 was empty.
- Inserted 86 at index 18.

**Result:** The manual trace was corrected.

### Entry 3: Resolving Multiple Collisions

**Problem:** During manual tracing, value 99 was initially assigned to index 7.

**Failed Approach:** The initial calculation did not account for the fact that indices 7 and 8 were already occupied.

**Solution:** Applied Linear Probing:

- Initial index = 99 % 23 = 7.
- Index 7 is occupied by 30.
- Checked index 8.
- Index 8 is occupied by 8.
- Checked index 9.
- Index 9 was empty.
- Inserted 99 at index 9.

**Result:** The collision was successfully resolved using Linear Probing.

### Entry 4: Program Testing

**Testing:** The C++ program was executed using an online compiler.

**Observation:** The program generated the insertion process and final hash table.

**Verification:** The final table was compared with the manually calculated trace.

**Result:** The implementation was checked against the expected insertion positions.

## Conclusion

The debugging process helped identify an unsuitable initial table-size choice and collision-handling calculation errors. These issues were corrected using Linear Probing.

The final implementation successfully inserts all 20 personalized values into the hash table and produces the expected output.