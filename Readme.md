Data Structures Internal Activity 3
Project Title
Personalized Hash Table Implementation Using Mid-Square Hashing and Separate Chaining
Student Details
- PRN: 202602100003
- Subject: Data Structures
- Programming Language: C++
Project Description
This project implements a hash table using the Mid-Square hashing technique and Separate Chaining for collision handling.

The project uses a personalized dataset generated according to the student's PRN. It demonstrates how hashing maps keys to table indices and how separate chaining handles collisions.
Personalized Dataset
PRN last four digits (S) = 0003 = 3

The dataset is generated using:

v[i] = (S + 13 * i) mod 100

Dataset:
YOUR PERSONALIZED DATASET

3, 16, 29, 42, 55, 68, 81, 94, 7, 20, 33, 46, 59, 72, 85, 98, 11, 24, 37, 50
20 elements
S = 3


Hashing Details
- Hashing technique: Mid-Square Method
- Collision handling: Separate Chaining
- Table size: 10 (implementation assumption; confirm with faculty)
- Programming language: C++
For this implementation, the square is padded to four digits, the middle two digits are extracted, and the result is reduced modulo the table size.
Project Files
- README.md: Project overview and documentation.
- hash_table.cpp: C++ implementation.
- output.txt: Actual program output.
- trace_report.md: Manual trace and output comparison.
- debugging_log.md: Development and debugging records.
Expected Learning Outcomes
1. Understand the Mid-Square hashing technique.
2. Implement a hash table in C++.
3. Handle collisions using Separate Chaining.
4. Compare manual calculations with actual program output.
5. Understand incremental project development.

   Algorithm
1. Initialize all hash table positions as empty.
2. Generate the 20 personalized values using PRN 202602100003.
3. Calculate the hash index using key % 23.
4. Check whether the calculated index is empty.
5. If occupied, use Linear Probing to find the next available position.
6. Insert the value into the available position.
7. Repeat until all values are inserted.
8. Display the final hash table.
Compilation and Execution
Compile the program using:
g++ hash_table.cpp -o hash_table


Execute the program:

For Linux:
./hash_table


For Windows:
hash_table.exe


Time Complexity
- Average insertion: O(1), assuming a reasonable load factor.
- Worst-case insertion: O(n) due to Linear Probing.
- Display operation: O(m), where m is the table size.
Final Result
The project demonstrates the successful implementation of a hash table using the Division Method and Linear Probing with 20 personalized values generated according to PRN 202602100003.

The program successfully calculates hash indices, handles collisions, inserts all 20 values into a hash table of size 23, and displays the final hash table.

Personalized Dataset:

3, 16, 29, 42, 55, 68, 81, 94, 7, 20, 33, 46, 59, 72, 85, 98, 11, 24, 37, 50
