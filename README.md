# 5. Longest Palindromic Substring

![LeetCode](https://img.shields.io/badge/LeetCode-5-Medium-orange)
![Java](https://img.shields.io/badge/Language-Java-blue)
![Time](https://img.shields.io/badge/Time-O(n²)-green)
![Space](https://img.shields.io/badge/Space-O(1)-green)

## 📌 Problem Statement
Given a string `s`, return the **longest palindromic substring** in `s`.  
A palindrome is a string that reads the same forwards and backwards.

## 📝 Examples

**Example 1:**
Input: s = "babad"
Output: "bab"


**Example 2:**
Input: s = "cbbd"
Output: "bb"


## 🔒 Constraints
- `1 <= s.length <= 1000`
- `s` consists of only digits and English letters.

## 💡 Approach: Expand Around Center
Treat every index as center of palindrome and expand left + right.

We check 2 cases for each `i`:
1. **Odd length**: center `i, i` → "bab"
2. **Even length**: center `i, i+1` → "bb"

Keep track of the longest one.

### Complexity
- **Time**: `O(n²)`
- **Space**: `O(1)`

## 💻 Java Solution
See `Solution.java`

## 🏃 How to Run
```bash
javac Solution.java
java Solution
