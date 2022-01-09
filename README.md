# key-takeaways-Leetcode

![](https://leetcode.com/_next/static/images/logo-ff2b712834cf26bf50a5de58ee27bcef.png)

### No.190 [Reverse Bits](https://leetcode.com/problems/reverse-bits/)

Reverse bits of a given 32 bits unsigned integer.

Input: n = 00000010100101000001111010011100 | Output:    964176192 (00111001011110000010100101000000)

Python:
* To get last bit of n: ``n & 1``
* Left bitwise shift: ``n << 1``, right bitwise shift: ``n >> 1``
* Bit operator has lower precedence than addition: ``ans = (ans << 1) + (n&1)``   

### No.231 [Power of Two](https://leetcode.com/problems/power-of-two/)

Return if the integer is a power of two.
* Bit-wise: 100 - 1 = 011
* 100 & 011 = 000
* ``n & n-1``


### No. 258 [Add Digits](https://leetcode.com/problems/add-digits/)

38 --> 3 + 8 --> 11
* 10 -> 1, 11 -> 2, 12 -> 3, ..., 19 -> 1, 20 -> 2
* 9 value a cycle
* Special case: 0 -> 0

### No. 459 [Repeated Substring Pattern](https://leetcode.com/problems/repeated-substring-pattern/)

Given a string ``s``, check if it can be constructed by taking a substring of it and appending multiple copies of the substring together.

Input: s = "abab" | Output: true

s = P * k, s_fold = s[1:] + s[:-1], s_fold = Head + P * (2k-2) + Tail

if k = 1, no repeated pattern.

if k > 1, then 2k-2 >= k. We can find s in s_fold.

``s in (2*s)[1:-1]``




