# Day22-50-days-coding-challenge
Problem 1: Minimum Remove to Make Valid Parentheses

Problem Statement:
Given a string s of '(', ')' and lowercase characters, remove the minimum number of parentheses to make the resulting string valid.

Constraints:
1 ≤ s.length ≤ 100000
s[i] is '(' or ')' or a lowercase English letter.

Approach:
Use a stack to store indices of unmatched '('.
Traverse the string and track unmatched ')' directly.
Mark all invalid parentheses positions, then reconstruct the string skipping them.

Examples:
Input: "lee(t(c)o)de)"
Output: "lee(t(c)o)de"
Input: "a)b(c)d"
Output: "ab(c)d"
Input: "))(("
Output: ""

Problem 2: Majority Element

Problem Statement:
Given an array nums of size n, return the element that appears more than ⌊n / 2⌋ times.

Constraints:
1 ≤ n ≤ 50000
-10^9 ≤ nums[i] ≤ 10^9
The majority element always exists.

Approach:
Use the Boyer-Moore Voting Algorithm.
Track a candidate and count. Reset candidate when count reaches zero.
In the end, the candidate is guaranteed to be the majority.

Examples:
Input: [3,2,3]
Output: 3
Input: [2,2,1,1,1,2,2]
Output: 2
