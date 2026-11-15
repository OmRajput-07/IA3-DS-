DEBUGGING LOG
Project Details
- PRN: 202602100003
- Project: Personalized Hash Table Implementation
- Language: C++
- Hashing Method: Division Method
- Collision Handling: Linear Probing
Entry 1: Selecting Table Size
Problem: Initially, a table size of 10 was considered.

Failed Approach: A table with 10 positions cannot accommodate all 20 distinct values.

Solution: Selected a table size of 23 as an implementation choice to accommodate all 20 values.

Result: The selected table size provides sufficient capacity.
Entry 2: Resolving Collision
Problem: During manual tracing, value 72 was initially assigned to index 3.

Failed Approach: The initial calculation did not account for the fact that index 3 was already occupied by 3.

Solution: Applied Linear Probing:
- Initial index = 72 % 23 = 3.
- Index 3 is occupied by 3.
- Checked index 4.
- Index 4 was empty.
- Inserted 72 at index 4.
Result: The manual trace was corrected.
Entry 3: Resolving Multiple Collisions
Problem: During manual tracing, value 98 was initially assigned to index 6.

Failed Approach: Index 6 was already occupied by 29, and index 7 was occupied by 7.

Solution: Applied Linear Probing:
- Initial index = 98 % 23 = 6.
- Index 6 is occupied by 29.
- Checked index 7; it was occupied by 7.
- Checked index 8; it was empty.
- Inserted 98 at index 8.
Result: The collision was successfully resolved.
Entry 4: Program Testing
Testing: The C++ program was executed using an online compiler.

Observation: The program generated the insertion process and final hash table.

Verification: The final table was compared with the manually calculated trace.

Result: The implementation was checked against the expected insertion positions.
Conclusion
The debugging process helped identify an unsuitable initial table-size choice and collision-handling calculation errors. These issues were corrected using Linear Probing.

The final implementation successfully inserts all 20 personalized values generated using PRN 202602100003 into a hash table of size 23.