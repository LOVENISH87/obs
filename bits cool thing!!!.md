

- bits -> 
<h1>Set Bit </h1>
![[Pasted image 20260123191156.png]]


<h1> leetcode
<a href "https://leetcode.com/problems/power-of-two/description/" > link </a>
</h1>

[https://leetcode.com/problems/power-of-two/description/]




```
 can you tell me what the fuck was i doign wrong and what changed to get to here?!!??

✦ Of course. Let's break it down.

  What you were doing wrong

  Your original code would have returned true for any positive number, not just powers of two.

  The problem was the while loop. The expression n = n & (n - 1) clears the rightmost '1' bit. Your loop kept doing this until n inevitably became
  0. Once n was 0, your code returned true.

  Example with a non-power-of-two number (n=12, binary `1100`):

   1. 1st loop: n is 12 (1100). n-1 is 11 (1011). n & (n-1) is 1100 & 1011 which is 8 (1000). n is now 8.
   2. 2nd loop: n is 8 (1000). n-1 is 7 (0111). n & (n-1) is 1000 & 0111 which is 0. n is now 0.
   3. Result: n is 0, so your function returned true. This is wrong for 12.

  What changed to fix it

  The fix was to remove the while loop and perform the check only once.

  A number is a power of two if and only if it's positive and has exactly one 1 bit in its binary representation. The expression (n & (n - 1)) ==
  0 is a classic trick that checks for exactly that condition.

  How the fix works:

   * If `n` IS a power of two (e.g., n=8, binary `1000`):
       * n-1 is 7 (binary 0111).
       * n & (n - 1) becomes 1000 & 0111, which is 0.
       * The condition (n & (n - 1)) == 0 is true. Correct.

   * If `n` IS NOT a power of two (e.g., n=12, binary `1100`):
       * n-1 is 11 (binary 1011).
       * n & (n - 1) becomes 1100 & 1011, which is 1000 (8). This is not 0.
       * The condition (n & (n - 1)) == 0 is false. Correct.

  So, the change was from a loop that would always eventually produce 0 to a single, decisive check that gives you the right answer immediately.

 2 open files (ctrl+g to view)
```


