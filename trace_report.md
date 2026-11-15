TRACE REPORT
1. Student Details
- PRN: 202602100003
- Subject: Data Structures
- Project: Hash Table Implementation
- Scenario: Mango Varieties
2. Personalized Dataset
Last four digits of PRN:

S = 3

Dataset formula:
\[
v[i] = (S + 13 \times i) \mod 100
\]

Personalized dataset:

3, 16, 29, 42, 55, 68, 81, 94, 7, 20, 33, 46, 59, 72, 85, 98, 11, 24, 37, 50
3. Hashing Technique
Division Method:
\[
h(key) = key \mod 23
\]

Table size = 23 (chosen implementation assumption).
4. Collision Handling
Linear Probing is used to resolve collisions.

If a calculated index is already occupied, the next available index is checked.

Formula:
\[
h_i(key) = (h(key) + i) \mod 23
\]

5. Manual Insertion Trace
Key	Initial Index	Final Index
3	3	3
16	16	16
29	6	6
42	19	19
55	9	9
68	22	22
81	12	12
94	2	2
7	7	7
20	20	20
33	10	10
46	0	0
59	13	13
72	3	4
85	16	17
98	6	8
11	11	11
24	1	1
37	14	14
50	4	5

6. Final Hash Table
Index	Value
0	46
1	24
2	94
3	3
4	72
5	50
6	29
7	7
8	98
9	55
10	33
11	11
12	81
13	59
14	37
15	EMPTY
16	16
17	85
18	EMPTY
19	42
20	20
21	EMPTY
22	68

7. Trace-Match Report
The manually calculated final hash table was compared with the actual output produced by the C++ program.
- All 20 personalized values were inserted successfully.
- The insertion positions match the Linear Probing calculations.
- The final hash table matches the expected program output.
- No values were lost or duplicated.
8. Conclusion
The program successfully inserts all 20 personalized values into the hash table. The Division Method calculates the initial index, while Linear Probing resolves collisions by checking subsequent positions.

The implementation demonstrates the working of hash functions, collision handling, and hash table operations using a personalized dataset generated from PRN 202602100003.