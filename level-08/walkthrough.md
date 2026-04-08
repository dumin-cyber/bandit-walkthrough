# Bandit Level 7 → Level 8

## 🎯 Objective
Find the password stored in a file next to a specific word.

## 🔍 Approach
Since the password was located inside a file and associated with a specific keyword, I used the `grep` command to search for that word across all files in the directory.

## 💻 Commands Used
```bash
grep "keyword" *
