# Section 1

| PC | Opcode | src1_addr | src1_out   | src2_addr | src_out    |dst_addr | dst_data   |
|---:|-------:|----------:|-----------:|----------:|-----------:|--------:|-----------:|
|   0| 0x23   | 0         | 0x00000000 | 2         | 0x00000000 | 0       | 0x00000000 |
|   4| 0x23   | 0         | 0x00000000 | 2         | 0x00000000 | 0       | 0x00000000 |
|   8| 0x00   | 2         | 0x00000000 | 2         | 0x00000000 | 0       | 0x00000000 |
|  12| 0x2B   | 0         | 0x00000000 | 3         | 0x00000000 | 2       | 0x00000056 |
|  16| 0x00   | 3         | 0x00000000 | 2         | 0x00000056 | 2       | 0x00000056 |
|  20| 0x08   | 3         | 0x00000000 | 5         | 0x00000000 | 3       | 0x00000000 |
|  24| 0x00   | 5         | 0x00000000 | 3         | 0x00000000 | 3       | 0x00000084 |
|  28| 0x00   | 6         | 0x00000000 | 2         | 0x00000056 | 4       | 0xFFFFFFAA |
|  32| 0x00   | 6         | 0x00000000 | 2         | 0x00000056 | 5       | 0x0000000C |
|  36| 0x00   | 5         | 0x0000000C | 4         | 0xFFFFFFAA | 6       | 0x00000000 |
|  40| 0x04   | 5         | 0x0000000C | 0         | 0x00000000 | 7       | 0x00000056 |
|  44| 0x23   | 0         | 0x00000000 | 8         | 0x00000000 | 8       | 0xFFFFFFA9 |
|  48| 0x00   | 0         | 0x00000000 | 0         | 0x00000000 | 6       | 0x00000000 |
|  52| 0x00   | 0         | 0x00000000 | 0         | 0x00000000 | 1F      | 0x0000000C |
|  48| 0x00   | 0         | 0x00000000 | 0         | 0x00000000 | 8       | 0x00000000 |

# Section 2
The differences between the two comes from the fact that we didn't account for all pipeline hazards. Data hazards were not accounted for so data that was expected to be available was not and inccorectly used.

# Section 3
add $zero, $zero, $zero
