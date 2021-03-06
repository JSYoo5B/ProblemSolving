# [Endians](https://algospot.com/judge/problem/read/ENDIANS)

| 시간 제한 | 메모리 제한 |
| :-------: | :---------: |
| 1000 ms   | 65536 kb    |

## 문제
The two island nations Lilliput and Blefuscu are severe rivals. 
They dislike each other a lot, and the most important reason was that 
they break open boiled eggs in different ways.

People from Lilliput are called little-endians, since they open eggs at the small end. 
People from Blefuscu are called big-endians, since they open eggs at the big end.

This argument was not only about their breakfasts but about their computers, too. 
Lilliput and Blefuscu's computers differed in the way they store integers; 
they stored the bytes in different orders. 
Computers from Lilliput(*little-endians*) ordered it 
from the LSB(least significant byte) to the MSB(most significant byte), 
and computers from Blefuscu was exactly the opposite.

For example, a 32-bit unsigned integer 305,419,896 (0x12345678) 
would be saved in two different ways:

    00010010 00110100 01010110 01111000 (in an Blefuscu computer)
    01111000 01010110 00110100 00010010 (in an Lilliput computer)

Therefore, if there was any need to exchange information between Blefuscu and Lilliput computers, 
some kind of conversion process was inevitable. 
Since nobody liked converting the data by himself before sending, 
recipients always had to do the conversion process.

Given some 32-bit unsigned integers retrieved in a wrong endian, 
write a program to do a conversion to find the correct value.

## 입력
The first line of the input file will contain the number of test cases, C (1 ≤ C ≤ 10, 000). 
Each test case contains a single 32-bit unsigned integer, which is the data without endian conversion.

## 출력
For each test case, print out the converted number.
