# Bandit Level 1 → Level 2

## 🎯 Objective
Find the password stored in a file named `-` located in the home directory.

## 🔍 Approach
After listing the directory contents using `ls`, I identified a file named `-`.

Attempting to read the file using `cat -` did not work as expected, because `-` is interpreted as standard input (stdin) rather than a filename.

To correctly reference the file, I used a relative path using `cat ./`

## 💻 Commands Used
```bash
ls
cat ./-
