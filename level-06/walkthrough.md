# Bandit Level 5 → Level 6

## 🎯 Objective
Find the password stored in a file within the `inhere` directory with the following properties:
- human-readable
- exactly 1033 bytes in size
- not executable

## 🔍 Approach
After identifying the `inhere` directory, I navigated into it and observed multiple subdirectories and files.

To efficiently locate the correct file, I used the `find` command with filters based on the given conditions.

I searched for:
- files (`-type f`)
- with a size of 1033 bytes (`-size 1033c`)

This led me to the file `.file2` inside the `maybehere07` directory and find the password.

## 💻 Commands Used
```bash
ls
cd inhere
find . -type f -size 1033c
cat ./maybehere07/.file2
