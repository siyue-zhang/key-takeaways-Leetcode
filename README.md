# key-takeaways-Leetcode

### No.190 [Reverse Bits](https://leetcode.com/problems/reverse-bits/)

Reverse bits of a given 32 bits unsigned integer.

Input: n = 00000010100101000001111010011100 | Output:    964176192 (00111001011110000010100101000000)

Python:
* To get last bit of n: ``n & 1``
* Left bitwise shift: ``n << 1``, right bitwise shift: ``n >> 1``
* Bit operator has lower precedence than addition: ``ans = (ans << 1) + (n&1)``   
